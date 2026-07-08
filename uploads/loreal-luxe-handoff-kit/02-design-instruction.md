# DESIGN INSTRUCTION — Mikhail Bogatyrev × L'Oréal Luxe Self-Presentation
### For: Claude (design/build agent) · Deliverable: single-file HTML artifact
### Read together with: 01-content.md (all copy — use verbatim), 03-build-spec.md (engineering), 04-assets.md (links & logos)

---

## 1. THE ONE-SENTENCE BRIEF

A one-page scroll self-presentation site that reads like an editorial from a luxury maison — restrained, typographic, confident — and never, at any pixel, looks like an AI-generated template.

## 2. AUDIENCE & STAKES

CMO and hiring team at L'Oréal Luxe Australia. They live inside the world's best luxury brand systems (Lancôme, YSL, Armani). They will detect a generic template in 2 seconds. The page itself is the work sample: it must demonstrate Pillar I (Desire — storytelling) from 01-content.md by existing.

## 3. ZERO-AI-FEELING RULES (hard constraints)

DON'T — these instantly read as AI/template:
- No purple/indigo/teal gradients, no glassmorphism, no neon glows
- No emoji anywhere
- No uniform rounded-corner card grids with drop shadows ("SaaS card soup")
- No stock photos, no AI-generated faces or hands, no illustration packs
- No centered-everything layouts; no equal-height everything
- No default Tailwind/shadcn look, no bootstrap blues
- No exclamation marks in UI copy

DO — these read as crafted:
- Asymmetry: offset headlines, staggered grids, one element intentionally breaking the column
- Hairline rules (1px) as the primary structural device, not boxes
- Numbered section kickers in letter-spaced small caps: `01 — WHO I AM`
- Sharp corners everywhere (border-radius: 0), except the carousel discs (perfect circles)
- Generous negative space — sections breathe; padding is a luxury statement
- Oversized display serif numerals as graphic elements (01–06 in Contribution block)
- Restrained motion: things fade and rise 12–20px, 500–700ms, cubic-bezier(0.16,1,0.3,1); nothing bounces, spins or pulses

## 4. DESIGN SYSTEM (derived from L'Oréal corporate + Luxe brand codes)

L'Oréal's Luxe web language (loreal.com/en/luxe-division, Lancôme, YSL Beauté): near-monochrome palettes, high-contrast serif display type, thin rules, circular logo discs on soft blurred bands, editorial numbered stats (1st / 30 / 30,000), quote blocks with oversized serifs. Reproduce that system, not any single brand's livery (no YSL logo lockups, no Lancôme rose — we reference the division, we don't cosplay a brand).

### Colour tokens
```
--ivory:      #F6F4EF   /* light section background */
--porcelain:  #FFFFFF   /* cards, carousel discs */
--noir:       #111111   /* dark sections, primary text on light */
--charcoal:   #1C1C1C   /* dark section cards */
--gold:       #A8873B   /* accents ONLY: rules, kickers, chips, quiz highlights */
--gold-soft:  #C9AE7C   /* hover state of gold */
--hairline:   #E3DED3   /* 1px rules on light */
--hairline-d: #2E2E2E   /* 1px rules on dark */
--mist:       #8A8578   /* secondary text on light */
--stone:      #B9B4A6   /* secondary text on dark */
```
Gold is a seasoning, not a sauce: ≤5% of any viewport should be gold.

### Section background rhythm
hero(ivory) → about(porcelain) → work(ivory) → luxe(porcelain, carousel band = blurred warm image strip or soft gradient band in beige tones) → channels(ivory) → trends(porcelain) → journey(ivory) → vision(NOIR — the cinema moment) → contribution(porcelain) → quiz(NOIR) → footer(noir, hairline-d top rule)

### Typography
- Display serif: **Cormorant Garamond** (Google Fonts; weights 300/400/500 + italic). Fallback stack: `Didot, "Playfair Display", Georgia, serif`. Used for H1/H2, big numerals, vision narrative, quiz result titles.
- Body/UI: **Jost** (300/400/500). Fallback: `"Helvetica Neue", Arial, sans-serif`. L'Oréal's own geometric sans vibe.
- Kickers/labels/tags: Jost 400, uppercase, letter-spacing 0.18em, 11–12px, gold or mist.
- Scale: H1 `clamp(2.8rem, 6.5vw, 6rem)` weight 400 (never bold — luxury serifs are light); H2 `clamp(2rem, 4vw, 3.4rem)`; body 16–17px/1.7; stat numerals `clamp(2.5rem,4vw,3.5rem)` Cormorant 300.
- Punctuation: use real em-dashes and curly quotes in rendered text.

### Components
- **Buttons:** text + 1px border, sharp corners, uppercase letter-spaced 12px, padding 16px 32px; hover: background noir/text ivory (on light) — 250ms.
- **Pillar chips (I–IV):** small circles 28px, 1px gold border, serif numeral inside; used identically in blocks 3, 5, 6 — this repetition is the visual thread.
- **Tags/skill pills:** 1px hairline border, uppercase 11px, padding 8px 16px; "relevant" ones get gold border + gold text.
- **Weight bars (channels):** 4px tall, noir fill on hairline track, animated width on scroll-into-view; potential arrows as `▲▲▲` in gold.
- **Modals:** full-screen overlay rgba(17,17,17,0.92), content panel porcelain, max-width 880px, close = thin `✕` top right, ESC + backdrop close, body scroll locked.

## 5. SECTION-SPECIFIC DESIGN NOTES

- **Hero:** ivory. Kicker top-left, gold hairline under it. H1 spans ~60%. Right 40%: a restrained generative-geometry motif drawn in CSS/SVG — thin gold concentric arcs or a single elegant line-wave, almost invisible (opacity ~0.35). Scroll cue: thin vertical line 48px + `SCROLL` in 10px letters.
- **About / brands:** company chips = monochrome wordmark text chips (see 04-assets.md), flip on hover via 3D rotateY or crossfade to show role text (tap on mobile). "Brands I worked for" banners: wordmark text set in each brand's typographic flavour; non-luxury ones `filter: grayscale(1)` with colour bleeding in on hover; luxury four always full colour; Wella/Schwarzkopf carry a 9px gold `BEAUTY` corner-tag.
- **Work:** 3 editorial cards, top hairline + oversized serif index (1/2/3), NOT boxed — separated by rules and whitespace. `OPEN CASE +` as text-button. Modal follows template in 01-content.md, with a 3-slot screenshot row (empty slots = hairline rectangles with `SCREENSHOT — [name]` caption, ready for later image drop-in).
- **L'Oréal Luxe carousel:** faithful to loreal.com/en/luxe-division — horizontal band with soft blurred warm-toned background, white circular discs (~96px) carrying brand wordmarks (serif, tiny), arrows in white circles left/right, auto-advance ~3s pause on hover, active disc scaled 1.15 with 1px frame. Loop infinitely. Brand order in 01-content.md.
- **Channels:** row-cards separated by hairlines (a "table as editorial layout"). TikTok row: dashed hairline border + gold `PRE-LAUNCH` tag. Include the italic caveat line under the table: weights are working assumptions.
- **Trends:** 6 cards in 3×2 + 1 full-width spotlight (Adaptive PDP) — spotlight gets noir background with ivory text to make it feel like the "editor's pick".
- **Journey:** the gold sine-wave is an inline SVG path across 4 columns; nodes = small gold dots on the wave; labels above/below alternating; pillar chips reused. Mobile: vertical timeline instead of wave.
- **Vision (noir):** the most typographic section. Steps set in large Cormorant (~22–24px) with gold step labels (`THE SPARK`), connected by a 1px gold vertical thread. Slow fade-in per step on scroll.
- **Contribution:** 3×2 grid, oversized ghost numerals (01–06) in Cormorant 300 at ~120px, 12% opacity, behind each card's text.
- **Quiz (noir):** see 03-build-spec.md for logic. Visual: progress = 9 thin gold ticks; answer options = full-width hairline-bordered rows, hover gold border; correct = gold fill flash, wrong = subtle strikethrough; reasoning slides open under the options in italic serif. Result card: tier name in huge Cormorant italic + one-liner + CTA button (mailto).
- **Footer (noir):** single row, hairline top, links in stone with gold hover. Include the human-made micro-line.

## 6. RESPONSIVE

Breakpoints: 1200 / 900 / 600. Mobile: nav collapses to `MENU` text-button opening full-screen noir overlay with big serif links; grids stack to 1 col; carousel becomes swipeable; drag-to-rank quiz question becomes tap-to-order (tap items in sequence, numbers appear).

## 7. ACCEPTANCE CHECKLIST

1. Squint test: page silhouette looks like a Lancôme editorial, not a dashboard.
2. Zero purple. Zero emoji. Zero rounded cards. Gold ≤5%.
3. All copy verbatim from 01-content.md — no paraphrasing, no added exclamation marks.
4. Pillar chips appear identically in blocks 3, 5, 6.
5. Quiz fully playable, reasoning shown for every answer, tiers correct.
6. All 27 carousel brands present, loop seamless.
7. Modals: open/close via click, ESC, backdrop; scroll locked.
8. Lighthouse-sane: no layout shift on font load (font-display: swap + matched fallback metrics).
