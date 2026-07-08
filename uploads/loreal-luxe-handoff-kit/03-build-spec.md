# BUILD SPEC — engineering requirements for the HTML artifact

## Delivery format
- **One self-contained HTML file** (inline CSS + vanilla JS). No React, no build step, no external JS libraries.
- Fonts: Google Fonts `<link>` for Cormorant Garamond + Jost with full local fallback stacks (the page must look correct if the fonts fail to load — artifact sandboxes sometimes block external requests).
- **No localStorage / sessionStorage** (unsupported in claude.ai artifacts). Quiz state lives in JS variables only.
- No external images required for v1: logos are typographic wordmarks, decoration is CSS/SVG. Screenshot slots are empty placeholders (hairline boxes) with visible captions, each carrying an `id` (see naming in 04-assets.md) so images can be dropped in later by replacing the placeholder with an `<img>`.

## Architecture
- Semantic sections with ids: `hero, about, work, luxe, channels, trends, journey, vision, contribution, quiz, contact`.
- Sticky nav: hidden at top, slides in after hero (IntersectionObserver on hero exit). Active link tracking via IntersectionObserver (threshold 0.4). Smooth scroll (`scroll-behavior: smooth`; JS offset for sticky bar height).
- Scroll animations: one IntersectionObserver adding `.in-view`; CSS handles transitions (`opacity 0→1, translateY 16px→0`). Stagger children with `transition-delay` steps of 80ms. Respect `prefers-reduced-motion`.

## Components

### Company chips (About)
Flip interaction: wrapper with `perspective`; front = wordmark, back = role text (11px). Desktop: flip on hover. Mobile/touch: flip on tap (toggle class); tapping another chip closes the previous.

### Brand banners (About)
`filter: grayscale(1); opacity:.75` default for non-luxury; hover/touch → grayscale(0). Luxury four: no filter + subtle gold hairline underline. `BEAUTY` tag = absolutely positioned 9px uppercase gold label on Wella/Schwarzkopf.

### Project modals (Work)
- Open on tile click; template per 01-content.md (Summary / Assessed / Done / Delivered / Results / screenshots row).
- Close: ✕ button, ESC, backdrop click. `overflow:hidden` on body while open. Focus trap basic: focus ✕ on open, return focus to tile on close.

### Luxe carousel
- Track = duplicated list for seamless infinite loop, CSS `transform: translateX` animation via JS rAF or CSS keyframes (pause on hover/touch).
- Manual arrows advance one disc with 400ms ease; auto-resume after 5s idle.
- Disc: 96px circle, porcelain bg, brand wordmark in Cormorant 11–13px centered, `letter-spacing:.06em`. Active (center) disc scale 1.15.

### Channel weight bars
Animate `width: 0 → N%` when scrolled into view (600ms, 100ms stagger). Percent label counts up in JS (integer only).

### Journey wave
Inline SVG: one `path` (gentle sine) with `stroke: var(--gold); stroke-width:1.5`, drawn on scroll via `stroke-dasharray/dashoffset` animation. Node dots = `circle` elements appearing after the path passes them. Below 900px: replace SVG wave with vertical layout (CSS only, wave hidden).

## Quiz engine (vanilla JS)

### Data model
```js
const QUIZ = [
 {
   id: 1, type: 'single', weight: 1,
   q: 'E-commerce accounts for what share of L'Oréal Group sales in 2025?',
   options: ['10%','20%','More than 30%','50%'],
   correct: [2],
   reasoning: '…' // verbatim from 01-content.md
 },
 { id: 2, type: 'duel',  weight: 1, options: ['Mecca','Sephora'], correct: [0], … },
 { id: 3, type: 'multi', weight: 2, correct: [0,1,2], … },
 { id: 5, type: 'rank',  weight: 2, options: ['Discovery','Consideration','Purchase','Retention'],
   correctOrder: [0,1,2,3], … },
 …9 items, content verbatim from 01-content.md Block 9
]
```
Weights: single/duel = 1, multi/rank = 2 (difficulty-weighted, 1door style). Max score = Σ weights = 12.

### Types & scoring
- `single` / `duel`: click one option → immediate lock → mark correct/incorrect → show reasoning → `NEXT` button appears.
- `multi`: checkboxes + `CONFIRM` button. Score full weight only if selection set === correct set (partial: half weight if ≥1 correct picked and 0 wrong — round down at the end).
- `rank`: desktop drag (HTML5 draggable or pointer-events reorder), mobile tap-to-order (tap items in intended sequence; each tap assigns next index; `RESET` link). Full weight for exact order; half if ≤1 adjacent swap.
- Progress: 9 gold ticks, filled as answered.

### Result
`pct = earned / 12`. Tiers per 01-content.md Block 9 (0–39 / 40–69 / 70–89 / 90–100). Result card: tier name (Cormorant italic, huge), tier line, score `X / 12`, per-question recap row of ✓/✕ ticks, CTA `mailto:michael.bgty@gmail.com?subject=Let's compare notes — L'Oréal Luxe`. `PLAY AGAIN` resets state (no storage).

## QA checklist (run before delivering)
1. All 9 quiz questions playable on desktop AND touch; rank question usable with taps.
2. Modals ✕/ESC/backdrop close; body scroll restores.
3. Carousel loops with no visible jump; pauses on hover.
4. Nav highlights correct section while scrolling; smooth scroll lands with correct offset.
5. 375px, 768px, 1440px layouts checked; no horizontal scroll anywhere.
6. Fonts blocked ⇒ page still elegant (fallback serif visible).
7. Copy diff against 01-content.md ⇒ verbatim.
