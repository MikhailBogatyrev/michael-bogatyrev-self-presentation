# MIKHAIL BOGATYREV × L'ORÉAL LUXE
## Self-Presentation Site — Content Document & Mockups
### Online Shopper & Experience Lead, L'Oréal Luxe Australia

**Format:** One-page scroll, sticky anchor navigation, HTML artifact
**Language:** English
**Status:** DRAFT for confirmation — mockups + full copy. Design instruction file follows after sign-off.

---

## GLOBAL STRUCTURE & NAVIGATION

Sticky top bar (appears after hero scroll):

```
MB — MIKHAIL BOGATYREV          About · Work · L'Oréal Luxe · Channels · Trends · Journey · Vision · Contribution · Quiz
```

Section order:

| # | Section ID | Nav label | Height |
|---|-----------|-----------|--------|
| 0 | `#hero` | — | 1 screen |
| 1 | `#about` | About | 1.5 screens (incl. brands) |
| 2 | `#work` | Work | 1.5 screens + modals |
| 3 | `#luxe` | L'Oréal Luxe | 1 screen |
| 4 | `#channels` | Channels | 1.5 screens |
| 5 | `#trends` | Trends | 1 screen |
| 6 | `#journey` | Journey | 1 screen |
| 7 | `#vision` | Vision | 1 screen |
| 8 | `#contribution` | Contribution | 1 screen |
| 9 | `#quiz` | Quiz | 1 screen (interactive) |
| 10 | `#contact` | — | footer |

---

# BLOCK 0 — HERO

## Mockup
Full-viewport. Ivory/near-black split. Left 60%: oversized serif headline, kicker above, sub below, one CTA. Right 40%: restrained abstract gold-line motif (no stock photos, no AI faces). Thin gold rule under kicker. Scroll cue at bottom center.

```
┌────────────────────────────────────────────────────────────┐
│  FOR L'ORÉAL LUXE AUSTRALIA          [small gold kicker]    │
│                                                             │
│  Every click should                                         │
│  feel like couture.                  [abstract gold lines]  │
│                                                             │
│  Mikhail Bogatyrev — Online Shopper & Experience Lead       │
│  candidate. 10+ years of digital experience across brand,   │
│  product and performance development.                       │
│                                                             │
│  [ EXPLORE THE THINKING ↓ ]                                 │
└────────────────────────────────────────────────────────────┘
```

## Copy
- Kicker: `A SELF-PRESENTATION FOR L'ORÉAL LUXE AUSTRALIA`
- H1: `Every click here should feel like couture.`
- Sub: `I'm Mikhail Bogatyrev — a digital commerce and experience leader with 10+ years building premium brands' digital presence, products and performance. This page is my answer to your role description — and to the question hidden behind it: what does the Online Shopper & Experience Lead role truly demand, and how would I deliver it? It's also an attempt to flip the interview itself — to let you get to know a candidate in a way none of us are quite used to.`
- CTA: `Explore the thinking ↓`

---

# BLOCK 1 — ABOUT: INTRODUCTION & BRANDS (1.5 screens)

## Mockup
Two stacked layers.

**Layer A — self-presentation (0.5 screen):** left column portrait-free intro paragraph + 4 stat counters in a gold-ruled row.

```
  WHO I AM
  [intro paragraph, 3 lines max]

  10+ yrs      5 regions      3 P&Ls owned      Full D2C built
  digital      AU·EU·ME·      eCom & digital    from the ground up
  commerce     APAC·CIS       marketing         at De'Longhi CIS
```

**Layer B — brands (1 screen):** Two distinct rows.
1. **"Companies I worked in"** — interactive logo chips (from CV). Hover/tap: chip flips to show role + one-line achievement.
2. **"Brands I worked for"** — tag cloud of brand banners. **Luxury-contributing brands render in full colour; all others in black & white.** Hover: subtle lift + colour bleed-in on B&W.

```
  COMPANIES I WORKED IN
  [Toshi] [ASBIS·iSpace] [TreasureHunter] [Prospekt] [Midea] [De'Longhi] [LEGO] [Ferrero] [MARS] [JTI]

  BRANDS I WORKED FOR                    ● colour = luxury & premium experience
  ◉Apple ◉Bang&Olufsen ◉Devialet ◉Dyson       ← COLOUR banners
  ○Schwarzkopf ○Wella ○De'Longhi ○Kenwood ○Toshi ○Toshiba ○Midea ○Oshee ○Ferrero   ← B&W banners
```

> ✓ CONFIRMED: **Apple, Bang & Olufsen, Devialet, Dyson** in colour; Wella & Schwarzkopf B&W with a gold `BEAUTY` corner-tag.

## Copy

**Section kicker:** `01 — WHO I AM`
**H2:** `Premium is my home turf.`

**Intro paragraph:**
`I've spent 10+ years where brand desirability meets commercial discipline: building and running e-commerce and digital marketing for premium and luxury brands across Australia, Europe, the Middle East, APAC and CIS. I've owned P&Ls, led cross-functional teams, and shipped everything from D2C platforms to marketplace strategies — always with the same conviction: the experience is the product.`

**Stat counters:**
1. `10+ years in digital commerce & marketing`
2. `5 regions — AU, EU, ME, APAC, CIS`
3. `3 e-commerce P&Ls owned end-to-end`
4. `Full D2C built from the ground up at De'Longhi Group CIS`

**Company chip flip-side copy (role + proof):**
| Chip | Flip text |
|---|---|
| Toshi (AU) | eCommerce & Marketing Manager — CRO, channel development (Iconic, Amazon, Baby Bunting), BigQuery/GA4/AI analytics stack |
| ASBIS · iSpace | Senior Digital Marketing Manager — Apple Premium Partner, 31 stores; YoY: SEO +17%, PPC +116%, Social +73%, CRM +28%; net margin +1.76pp |
| TreasureHunter | Digital Marketing Operations Manager — scaled 3→12 eCom sites; organic +87%, bounce −10% |
| Prospekt (UK) | Marketing Manager — GTM, UX/UI & CJM for Beauty, Food & Beverage clients (Wella, Schwarzkopf) |
| Midea | Senior eCommerce Manager — triple-digit online growth across D2C & marketplaces |
| De'Longhi Group | Digital Marketing Manager — built D2C platform for 3 brands × 6 countries; D2C share to 50% |
| LEGO | Account Manager (Omni) — premium retail experiences, shop-in-shops, 360° campaigns |
| Ferrero / MARS / JTI | Key account & field foundations — negotiation, share of shelf, trade execution |

---

# BLOCK 2 — WORK: SKILLS & 3 PROJECTS (1.5 screens + modals)

## Mockup
**Row 1 — skills as tags** (pill chips, mono/uppercase, same taxonomy as portfolio):

```
● ECOMMERCE  ● DIGITAL MARKETING  ● PERFORMANCE MARKETING  ● UX/UI AUDIT  ● ANALYTICS & BI
● CRM / EMAIL MARKETING  ● BRAND STRATEGY  ● STRATEGY & CONSULTING  ● CUSTOMER EXPERIENCE
● AI & AUTOMATION  ● PRODUCT DELIVERY  ● OPERATIONS  ● TEAM BUILDING & DEVELOPMENT
```

Tags relevant to the vacancy glow gold on load (ECOMMERCE, UX/UI AUDIT, ANALYTICS & BI, CUSTOMER EXPERIENCE, PERFORMANCE MARKETING, AI & AUTOMATION).

**Row 2 — three project tiles**, editorial cards: brand wordmark, title, 2-line summary, "what was assessed" micro-tags, `OPEN CASE +`. Click/tap → full-screen modal (dimmed backdrop, luxury lightbox) with structured case + screenshot slots.

```
┌──────────────┐  ┌──────────────┐  ┌──────────────┐
│ DYSON        │  │ BANG&OLUFSEN │  │ WELLA        │
│ eCommerce    │  │ Luxury launch│  │ CJM & digital│
│ turnaround   │  │ & media      │  │ go-to-market │
│ strategy     │  │ strategy     │  │              │
│ [tags]       │  │ [tags]       │  │ [tags]       │
│ OPEN CASE +  │  │ OPEN CASE +  │  │ OPEN CASE +  │
└──────────────┘  └──────────────┘  └──────────────┘
```

Modal template: `Summary → What was assessed & how → What was done → What was delivered → Results → [screenshot gallery]`.

## Copy

**Section kicker:** `02 — SELECTED WORK`
**H2:** `Three cases. One discipline: experience that sells.`

### Tile 1 — DYSON
- **Title:** `Dyson — eCommerce strategy & experience turnaround`
- **Summary (tile):** `A premium brand with a fragmented web estate, counterfeit-riddled marketplaces and a leaking funnel. Rebuilt the entire online journey — and the P&L followed.`
- **Assessed micro-tags:** `SITE PERFORMANCE · SEO · CJM · MARKETPLACES · MEDIA EFFICIENCY · ANALYTICS`

**Modal:**
- **What was assessed & how:** `Full digital audit: multi-domain architecture (3 competing domains), page-speed and UX benchmarks, SEO visibility, customer journey mapping across every touchpoint, marketplace presence vs. counterfeit listings on the fastest-growing platforms (+93% / +144% YoY), media spend efficiency and CAC by channel.`
- **What was done:** `Consolidated domains into one authoritative store; rebuilt product pages around premium storytelling; redesigned pain-point touchpoints from the CJM (callbacks, stock alerts, abandoned-cart recovery); launched official brand stores with brand-protection monitoring on key marketplaces; shifted budget from inefficient paid search to organic and content; stood up end-to-end analytics with attribution and KPI dashboards.`
- **What was delivered:** `A single consolidated D2C platform, marketplace flagship stores, a CJM-driven experience backlog, media reallocation plan, and a live analytics/reporting framework.`
- **Results:** `+35% online sales in 12 months · CAC −28% · conversion +18% · marketplace sales share +65% · NPS +12 pts.`
- Screenshot slots: 3 (Miro board: uXjVItYJA70=)

### Tile 2 — BANG & OLUFSEN
- **Title:** `Bang & Olufsen — luxury launch & precision media strategy`
- **Summary (tile):** `Taking a €10k+ AV icon to the right living rooms: an audience, media and measurement architecture built for high-net-worth buyers — not mass reach.`
- **Assessed micro-tags:** `LUXURY AUDIENCES · MEDIA MIX · GEO-TARGETING · KPI DESIGN · COMMERCIAL MODEL`

**Modal:**
- **What was assessed & how:** `Mapped where luxury buyers actually live and read: premium editorial (Robb Report, Luxuo, Luxury Daily), authority tech media (The Verge, What Hi-Fi), and high-intent communities (Head-Fi, AVS Forum, r/audiophile). Modelled audience segments, price-point psychology and channel economics for ultra-premium AV.`
- **What was done:** `Built the full launch architecture: audience & channels framework, media plan with narrow geo-targeting on affluent districts and workplaces, content & production scoping, KPI and effectiveness model tied to commercial outcomes, and a campaign calendar with clear roles & responsibilities.`
- **What was delivered:** `Launch media plan, audience playbook, budget & production framework, measurement model — the full strategy pack a luxury brand runs on.`
- **Results:** `A repeatable luxury-launch playbook: precision over reach, editorial authority over volume, measurable commercial KPIs over vanity metrics.`
- Screenshot slots: 3 (Miro board: uXjVKdAQQpQ=)

### Tile 3 — WELLA
- **Title:** `Wella — customer journey mapping & digital go-to-market`
- **Summary (tile):** `Beauty-category work at agency pace: journey mapping from first impression to repeat purchase, with concrete interventions at every stage of the funnel.`
- **Assessed micro-tags:** `BEAUTY CATEGORY · CJM · FUNNEL DESIGN · CONTENT STRATEGY · RETENTION LOOPS`

**Modal:**
- **What was assessed & how:** `End-to-end journey mapping across five stages — Interest, Search, Purchase, Recommend, Repeat — auditing every touchpoint: OLV and social at awareness, paid search and reputation at consideration, packaging and BTL at purchase, e-mail, loyalty and referral at retention.`
- **What was done:** `Identified where the funnel leaked and designed the fixes: landing pages, educational and product video content at the search stage, referral mechanics and web development at advocacy, subscription and look-a-like activation for repeat purchase.`
- **What was delivered:** `A complete CJM with channel roles per stage, a prioritised intervention map, and content/production briefs — the blueprint for the brand's digital GTM.`
- **Results:** `A journey architecture the client could execute immediately — the same discipline I'd bring to a Luxe brand's shopper experience.`
- Screenshot slots: 3 (CJM slide available; Miro board: uXjVPTobbb8=)

> NOTE: Results lines for B&O and Wella are framed qualitatively — give me numbers if you have them and I'll harden the copy.

---

# BLOCK 3 — L'ORÉAL LUXE (1 screen)

## Mockup
Three stacked elements:

1. **Brand carousel — faithful reproduction of loreal.com/en/luxe-division:** circular white logo discs on a soft blurred background band, horizontal auto-scroll, arrow buttons left/right in white circles, active disc slightly enlarged with a thin frame. All 27 published Luxe brands as logo discs (text wordmark fallback where no logo asset).
2. **Categories row:** three editorial category cards — `FRAGRANCE / SKINCARE / MAKEUP` — each with 2-3 representative brand names.
3. **Pillars strip:** four numbered pillars of luxury shopper experience (these four terms recur throughout the rest of the site — they are the spine of the argument).

```
  ← ○ ○ ◉ VIKTOR&ROLF · YTTP · YSL · YUESAI · LANCÔME ○ ○ →   [carousel band]

  FRAGRANCE            SKINCARE              MAKEUP
  YSL·Margiela·Mugler  Lancôme·Kiehl's·HR    YSL·Armani·Urban Decay

  I. DESIRE     II. INTELLIGENCE     III. SEAMLESSNESS     IV. DEVOTION
```

## Copy

**Section kicker:** `03 — THE WORLD I'M APPLYING TO`
**H2:** `30 icons. One Culture de l'Écart.`

**Intro line:** `L'Oréal Luxe is the world leader in luxury beauty — €15.6B in 2025, growth accelerating, and market leadership now held in every region. In Australia, the battleground is experience: the market's most sophisticated prestige shoppers, served by the world's best beauty retailers.`

**Carousel brands (order as on loreal.com):** Lancôme · Yves Saint Laurent · Armani · Valentino · Kiehl's · Youth To The People · Aesop · Atelier Cologne · Jacquemus · Medik8 · Miu Miu · Prada · Urban Decay · Helena Rubinstein · Carita · Biotherm · Maison Margiela · Viktor&Rolf · Mugler · Ralph Lauren · Azzaro · Cacharel · Diesel · Yue Sai · IT Cosmetics · Shu Uemura · Takami

**Category cards:**
- `FRAGRANCE — the growth engine. YSL MYSLF, Prada Paradigme, Miu Miu Miutine: fine fragrance is driving Luxe's acceleration, and it's the hardest category to sell online — scent doesn't ship through a screen. Experience has to do that work.`
- `SKINCARE — the science story. Lancôme longevity science, Kiehl's dermatological heritage, Medik8's clinical edge: high-consideration purchases that reward diagnostics, education and consultation.`
- `MAKEUP — the play category. YSL, Armani, Urban Decay: shade-match anxiety meets impulse energy. Virtual try-on and social proof convert here.`

**The four pillars (spine of the site):**
1. `I. DESIRE — luxury is storytelling, which is exactly what you're experiencing right now. Every impression must carry the brand's world: editorial content, immersive PDPs, elevated visual merchandising.`
2. `II. INTELLIGENCE — luxury is personal. Diagnostics, AI advisory, data-driven personalisation: the online version of the counter consultation.`
3. `III. SEAMLESSNESS — luxury is effortless. One journey across D2C, retailers, marketplaces and social; flawless UX; zero friction from discovery to unboxing.`
4. `IV. DEVOTION — luxury is a relationship. Loyalty, replenishment, refills, services: the second purchase is the real KPI.`

---

# BLOCK 4 — CHANNELS & THEIR ROLES (1.5 screens)

## Mockup
Editorial table-as-cards: each channel = one horizontal row card with: channel name, ROLE (one phrase), weight bar (assumed share of Luxe-relevant online business), growth-potential arrow (▲▲▲/▲▲/▲), and a one-liner strategy note. TikTok Shop row visually distinct (dashed border = "pre-launch").

```
  CHANNEL          ROLE                      WEIGHT      POTENTIAL
  D2C brand sites  Brand temple & data       ████░░ 20%   ▲▲
  Mecca            Prestige gatekeeper       ██████ 35%   ▲▲
  Sephora AU       Global prestige stage     ███░░░ 12%   ▲▲
  Adore Beauty     Pure-play + retail media  ███░░░ 10%   ▲▲
  Amazon AU        The white space           ██░░░░ 8%    ▲▲▲
  DJ / Myer        Heritage counters         ██░░░░ 8%    ▲
  CW Ultra Beauty  Reach disruptor           ██░░░░ 7%    ▲▲
  TikTok Shop      The day-one advantage     ░░░░░░ 0%    ▲▲▲  [PRE-LAUNCH]
```

> Weights are labelled on-site as "indicative share of Luxe-relevant online opportunity — my working assumption, to be validated with internal data." This shows judgement without pretending to have internal numbers.

## Copy

**Section kicker:** `04 — THE AUSTRALIAN CHESSBOARD`
**H2:** `Every channel has a role. None of them is "just a shop."`

**Intro:** `Australia's luxury beauty market is ~US$1.6B and its online share grew ~22% last year. It is also one of the most retailer-concentrated prestige markets in the world — which makes channel-role clarity the single most valuable strategic asset. Here's how I read the board.`

**Channel rows:**

| Channel | Role | Note copy |
|---|---|---|
| **D2C brand sites** (lancome.com.au, yslbeauty.com.au, kiehls.com.au…) | `Brand temple & first-party data engine` | `Where the full brand world lives: services, refills, engraving, GWP, replenishment. Never the discount channel — the standard-setter every retailer is measured against. E-commerce is already >30% of group sales; D2C is where experience compounds into data.` |
| **Mecca** | `The prestige gatekeeper` | `~25% of Australian prestige beauty, A$1.43B revenue, 3M Beauty Loop members and the world's largest beauty store on Bourke St. Mecca defines luxury beauty CX in AU — win the digital shelf, the sampling programs and the retail media placements here, and the market follows.` |
| **Sephora AU** | `The global prestige stage` | `33 doors, +9% growth, and the global launch machine. The channel for exclusives, launch moments and Gen Z prestige recruitment.` |
| **Adore Beauty** | `Pure-play performance + retail media lab` | `A$199M revenue, record EBITDA, a fast-scaling store network and a retail media network that doubled in a year. The cleanest test-and-learn environment in the market.` |
| **Amazon AU** | `The white space` | `Beauty growing +45% YoY, a gated Premium Beauty store — and Luxe brands largely absent. The US precedent is written: Lancôme and YSL entered Amazon Premium Beauty in 2023, Kiehl's followed in 2024, and L'Oréal called it "a winning strategy for L'Oréal Luxe." Australia is the natural next chapter — done on luxury's terms: gated, full-price, brand-controlled.` |
| **David Jones / Myer** | `Heritage counters, services & gifting` | `Structurally pressured but still meaningful for gifting occasions, services and an older prestige shopper. Defend efficiently; innovate via services (DJ's Beauty Cycle shows the appetite).` |
| **Chemist Warehouse Ultra Beauty** | `The reach disruptor` | `Prestige-at-mass-prices format stocking YSL and Clarins. Handle with care: reach and recruitment upside vs. brand-equity dilution risk. Strict assortment and content governance.` |
| **TikTok Shop** | `The day-one advantage` | `Not yet launched in Australia — and that's exactly the point. In the US it did $15.1B GMV in 2025 (+68%), with beauty its #1 category; in the UK it's already the 4th-largest beauty retailer, growing +60% YoY. L'Oréal was a first-mover in every European launch. My play: build AU social-commerce readiness now — shoppable content library, creator-affiliate bench, live-shopping formats — so Luxe is live on day one, not year two.` |

---

# BLOCK 5 — TRENDS & TECHNOLOGIES (1 screen)

## Mockup
Grid of 7 trend cards: two rows of three + one full-width "spotlight" card beneath (Adaptive PDP). Each card: trend name, what it is (1 line), L'Oréal proof-point (1 line), and **pillar chips** (I/II/III/IV) showing which experience pillar it feeds. Pillar chips reuse Block 3 styling — this stitches the narrative together.

```
┌─────────────┐ ┌─────────────┐ ┌─────────────┐
│ AGENTIC AI  │ │ DIAGNOSTICS │ │ VIRTUAL     │
│ ADVISORY    │ │ & LONGEVITY │ │ TRY-ON      │
│ [II][III]   │ │ [II][I]     │ │ [II][III]   │
└─────────────┘ └─────────────┘ └─────────────┘
┌─────────────┐ ┌─────────────┐ ┌─────────────┐
│ SOCIAL &    │ │ RETAIL MEDIA│ │ CIRCULAR    │
│ LIVE COMMERCE│ │ NETWORKS   │ │ LUXURY      │
│ [I][III]    │ │ [I][III]    │ │ [IV][I]     │
└─────────────┘ └─────────────┘ └─────────────┘
┌───────────────────────────────────────────────┐
│ ADAPTIVE PDP & GEO-INTELLIGENT CONTENT        │
│ [II][III][I]                    [full-width]  │
└───────────────────────────────────────────────┘
```

## Copy

**Section kicker:** `05 — WHAT'S CHANGING THE GAME`
**H2:** `The technologies rewriting the luxury shopper journey.`

**Cards:**

1. **AGENTIC AI ADVISORY** — `The counter consultation, at scale. L'Oréal's Beauty Genius relaunched on agentic AI (CES 2026 keynote), 1.2M+ consumer conversations in the US, arriving on WhatsApp via the Meta partnership. Pillars: II · III`
2. **DIAGNOSTICS & LONGEVITY** — `Skin science as a service. Cell BioPrint reads your skin's biological age from a 5-minute proteomic test; Lancôme × Timeline brings cellular longevity to prestige skincare. High-consideration categories won by intelligence. Pillars: II · I`
3. **VIRTUAL TRY-ON & AR** — `ModiFace ended shade-match anxiety. Table stakes on D2C, differentiator on retailer sites and social — everywhere a shopper hesitates. Pillars: II · III`
4. **SOCIAL & LIVE COMMERCE** — `The funnel collapsed into the feed. Beauty is TikTok Shop's #1 category; live shopping and creator affiliates turn discovery into purchase in one session. Pillars: I · III`
5. **RETAIL MEDIA NETWORKS** — `The new trade spend. Mecca, Adore (+112% network growth) and Amazon all monetise their audiences — Luxe brands must buy the digital shelf as deliberately as they once bought counters. Pillars: I · III`
6. **CIRCULAR LUXURY** — `Refills as ritual. L'Oréal Luxe's refill movement turns sustainability into a repeat-purchase mechanic and a reason to return to D2C. Pillars: IV · I`
7. **ADAPTIVE PDP & GEO-INTELLIGENT CONTENT** *(full-width spotlight)* — `The product page stops being static. Content that adapts to who's looking and where: geo-specific product data and claims, clinical trial results and research evidence surfaced by market, routines and ingredient stories assembled to the shopper's context and climate. The digital shelf becomes as considered as the counter — and it's measurable, testable and always improving. Pillars: II · III · I`

---

# BLOCK 6 — SHOPPER JOURNEY MAP (1 screen)

## Mockup
Horizontal infographic in the style of my Wella CJM (wave line across stages), rebuilt in luxury styling: a thin gold sine-wave across four stage columns. Above/below the wave: technology & pillar nodes placed at the stage where they act. Pillar chips (I–IV) colour-coded; trend nodes reuse Block 5 names. Desktop: full wave; mobile: vertical stacked stages.

```
  DISCOVERY          CONSIDERATION        PURCHASE           RETENTION
  ~~~~~●~~~~~~~~~~~~~~~~●~~~~~~~~~~~~~~~~~●~~~~~~~~~~~~~~~~~●~~~~~
  Social & live      AI advisory          Seamless checkout  Refills & loyalty
  commerce [I]       Diagnostics [II]     VTO assist [III]   Replenishment [IV]
  Retail media [I]   Adaptive PDP &       Sampling/GWP [I]   Services & O2O [IV]
  Editorial [I]      geo content [II]     Delivery promise   Advocacy loop [I]
                     Ratings/UGC [II]     [III]
```

## Copy

**Section kicker:** `06 — THE JOURNEY, MAPPED`
**H2:** `Four stages. Four pillars. One continuous experience.`

**Intro:** `This is the same journey-mapping discipline I used for Wella and Dyson, applied to a Luxe brand in Australia. Every technology from the previous section lands at a precise stage — nothing is deployed for its own sake.`

**Stage columns:**

- **DISCOVERY** — `Where desire is born. Editorial content and immersive brand worlds (I); social & live commerce and creator affiliates (I); retail media on Mecca, Adore and Amazon buying the first impression (I). KPI: qualified traffic, new-to-brand reach, content engagement.`
- **CONSIDERATION** — `Where intelligence converts hesitation. AI advisory answering at 2am (II); diagnostics and skin analysis personalising the recommendation (II); adaptive PDPs surfacing geo-specific data, trial results and research evidence (II); ratings, UGC and education carrying the proof (II). KPI: PDP engagement, consultation usage, add-to-cart rate.`
- **PURCHASE** — `Where seamlessness earns the sale. Frictionless checkout and payment options (III); virtual try-on at the moment of doubt (III); sampling and GWP sweetening the leap (I); a delivery promise worthy of the box it arrives in (III). KPI: conversion rate, AOV, cart abandonment.`
- **RETENTION** — `Where devotion compounds. Replenishment and refill programs (IV); loyalty and services bridging online to counter (IV); the advocacy loop feeding Discovery again — UGC, referrals, reviews (I). KPI: repeat rate, LTV, retention cohorts, referral share.`

**Closing line:** `The wave doesn't end — retention feeds discovery. That's the loop luxury brands live on.`

---

# BLOCK 7 — VISION: THE BLUE-SKY JOURNEY (1 screen)

## Mockup
Full-width dark section ("the cinema moment" of the page). A single narrated scenario in elegant large serif, staged as a 5-step vertical timeline with a gold thread. Minimal decoration; this block is pure copy.

## Copy

**Section kicker:** `07 — THE BLUE SKY`
**H2:** `What perfect looks like.`

**Intro:** `Meet Chloé, 32, Melbourne. She doesn't know it yet, but she's about to buy her first Lancôme serum. Here's the journey as it should be:`

**Timeline steps:**

1. **THE SPARK** — `A creator she trusts wears a look in a TikTok live. The product is shoppable in-feed, but Chloé does what luxury shoppers do — she taps through to the brand world instead. The handover is seamless: same campaign, same story, no dead ends.`
2. **THE CONSULTATION** — `On lancome.com.au, an AI advisor picks up the conversation. A 3-minute skin diagnostic — camera-based, private, genuinely useful — recommends a routine of two products, not ten. It remembers her next visit. It feels like the counter at Le Bon Marché, not a chatbot.`
3. **THE DECISION** — `She checks Mecca — of course she does. The brand's digital shelf there is flawless: same story, rich content, 4.8 stars, her shade in stock at Bourke St with 2-hour click & collect. Whichever door she chooses, the brand wins.`
4. **THE ARRIVAL** — `The box is an event. A handwritten-feel card, a fragrance sample chosen from her diagnostic profile — not a random sachet. Unboxing is the first loyalty touchpoint, not the last delivery step.`
5. **THE RETURN** — `Six weeks later, a quiet nudge: "Your serum has about two weeks left." One tap to a refill — lighter footprint, member pricing, points toward a masterclass at the flagship. Chloé posts her routine. The loop closes; her content becomes someone else's Step 1.`

**Closing line:** `No channel conflict. No friction. No generic moment anywhere in the chain. Every touchpoint — owned, retail or social — plays its role in one orchestrated experience. That's the standard I build toward.`

---

# BLOCK 8 — MY CONTRIBUTION (1 screen)

## Mockup
Six workstream cards in a 3×2 grid, each numbered in oversized thin serif (01–06), with title + 3-line description + "first 90 days" micro-line. This block maps 1:1 to the job description bullets — recruiters should recognise their own JD.

## Copy

**Section kicker:** `08 — HOW I MAKE IT REAL`
**H2:** `Six workstreams. Day one to day ninety.`

**Cards:**

1. **AUDIT & CX JOURNEY OPTIMISATION** — `A full-funnel experience audit across D2C, retailer digital shelves and marketplaces — benchmarked against the four pillars. Output: a prioritised CX optimisation map with effort/impact scoring, exactly as I built for Dyson. First 90 days: audit complete, top-10 fixes in flight.`
2. **DATA DISCOVERY & INSIGHT MODELS** — `Stand up the analytical spine: sales, traffic, conversion and acquisition-cost dashboards; cohort and dependency models that show where growth actually comes from. I've built this stack (GA4, BigQuery, Looker, AI-assisted analysis) at three companies. First 90 days: single source of truth live.`
3. **STAKEHOLDER FEEDBACK LOOPS** — `Structured listening: brand teams, retail partners, media leads, customer service. Insights are worthless in a drawer — I run cadenced feedback rituals and convert them into the backlog. First 90 days: cross-functional CX council running monthly.`
4. **TECH BRIEFS & DELIVERY FACILITATION** — `Translate strategy into buildable briefs — VTO placements, advisory integrations, PDP modules — and facilitate delivery with dev teams and agencies. I've shipped platforms end-to-end (De'Longhi: 3 brands × 6 countries). First 90 days: 2-3 briefs scoped and in development.`
5. **MARKETING & TRADE MARKETING AGENDA** — `Make the trade tools work harder: retail media across Mecca/Adore/Amazon, joint activation calendars with channel partners, promo mechanics that protect prestige. LEGO and Ferrero taught me trade; ASBIS taught me digital trading. First 90 days: joint calendar agreed with top 3 channels.`
6. **EXPERTISE SHARING & TEAM ENABLEMENT** — `Expertise only counts when the team digests it. Workshops, playbooks — and yes, games: the quiz below is the same framework I built for 1door.cc's competence game. Learning should be as engaging as the brands we sell. First 90 days: first masterclass delivered.`

---

# BLOCK 9 — THE QUIZ (1 screen, interactive)

## Mockup
Same mechanics as the 1door.cc Competence Game, restyled to luxury: dark section, gold accents.

- Intro card → `START` → 9 questions, one at a time (progress dots) → result card.
- Question types: single-select, multi-select, A/B duel, drag-to-rank (tap-to-order on mobile).
- Every answer reveals **the reasoning** — right or wrong, you learn why (the 1door signature).
- Difficulty-weighted scoring. Result tiers (luxury remix of Garage→SpaceX):
  - 0–39%: `COUNTER CURIOUS` — "You browse beautifully. Let's talk."
  - 40–69%: `CLIENTELING APPRENTICE` — "Solid instincts — the détails need polish."
  - 70–89%: `FLAGSHIP DIRECTOR` — "You run a tight maison."
  - 90–100%: `LA CULTURE DE L'ÉCART` — "You defy the rules. We should work together."
- Result card CTA: `Let's compare notes over coffee → [email link]`

## Copy

**Section kicker:** `09 — PROVE YOU READ IT`
**H2:** `The Shopper Experience Game.`
**Intro:** `Nine questions. Everything you need is on this page. Built on the same engine I designed for 1door.cc's competence game — because sharing expertise should never be boring.`

**Questions (answer key ✓, reasoning included):**

1. *(single)* `E-commerce accounts for what share of L'Oréal Group sales in 2025?` — 10% / 20% / **>30% ✓** / 50%. *Reasoning: E-commerce passed 30% of group sales in 2025 and was named the group's primary growth engine — which is why this role exists.*
2. *(A/B duel)* `Who holds ~25% of Australian prestige beauty?` — **Mecca ✓** / Sephora. *Reasoning: Mecca is the market's gatekeeper — A$1.43B revenue, 3M Beauty Loop members, and the world's largest beauty store on Bourke St.*
3. *(multi)* `Which Luxe brands pioneered Amazon US Premium Beauty?` — **Lancôme ✓** / **YSL ✓** / **Kiehl's ✓** / La Roche-Posay. *Reasoning: Lancôme and YSL entered in 2023, Kiehl's in 2024 — L'Oréal called it "a winning strategy for L'Oréal Luxe." (La Roche-Posay is Dermatological Beauty, not Luxe.)*
4. *(single)* `TikTok Shop's position in UK beauty retail today?` — Niche experiment / Top 10 / **4th-largest beauty retailer ✓** / Market leader. *Reasoning: Beauty is TikTok Shop's #1 category. It isn't in Australia yet — which is why readiness now equals advantage later.*
5. *(drag-to-rank)* `Order the journey stages:` — **Discovery → Consideration → Purchase → Retention ✓**. *Reasoning: And retention feeds discovery — the loop luxury lives on.*
6. *(single)* `What does Cell BioPrint deliver in 5 minutes?` — A fragrance match / **A proteomic skin analysis incl. biological skin age ✓** / A foundation shade / A routine video. *Reasoning: CES 2025-announced diagnostics — intelligence (Pillar II) turning consideration into conviction.*
7. *(A/B duel)* `The stronger luxury acquisition lever online:` — Deeper discounts / **Experience: diagnostics, services, sampling, storytelling ✓**. *Reasoning: Discounting buys transactions and erodes equity; experience buys relationships. In luxury, the second purchase is the real KPI.*
8. *(multi)* `Which are pillars of luxury shopper experience on this page?` — **Desire ✓** / **Intelligence ✓** / Maximum SKU count / **Seamlessness ✓** / Permanent promotion / **Devotion ✓**. *Reasoning: Assortment breadth and promo depth are mass-market weapons. Luxury wins on the other four.*
9. *(single)* `"La Culture de l'Écart" means…` — A discount policy / French for compliance / **The culture of defying convention — creative tension that reinvents luxury codes ✓** / A logistics standard. *Reasoning: L'Oréal Luxe's guiding principle. This page tried to practise it.*

---

# BLOCK 10 — CONTACT (footer)

## Copy
- H2: `Let's build the journey.`
- Line: `Mikhail Bogatyrev · Melbourne, VIC · Available immediately for the 8-month contract — and ambitious beyond it.`
- Links: `michael.bgty@gmail.com · +61 436 658 807 · linkedin.com/in/mikhail-bogatyrev · michael-bogatyrev.lovable.app`
- Micro-footer: `Designed and written by a human. Assembled with care, not templates.`

---

# OPEN QUESTIONS BEFORE I WRITE THE DESIGN INSTRUCTION

1. ~~Luxury colour set~~ — ✓ CONFIRMED (Apple, B&O, Devialet, Dyson in colour; Wella/Schwarzkopf B&W + gold BEAUTY tag).
2. **Channel weights (Block 4):** my working assumptions (Mecca 35 / D2C 20 / Sephora 12 / Adore 10 / Amazon 8 / DJ-Myer 8 / CW 7). Adjust?
3. **TikTok framing:** research shows TikTok Shop has NOT launched in AU (confirmed by TikTok ANZ, March 2026). I reframed your ask as "day-one readiness advantage" — factually safe and arguably stronger. OK?
4. **B&O and Wella results:** any real numbers to harden the two case tiles?
5. **Screenshots for modals:** you add them after the artifact is built, or send them to me now and I embed placeholders with exact filenames?
6. **Quiz length:** 9 questions (one per section). Keep, or cut to 6 for pace?
7. **Stat check (Block 1):** "3 P&Ls owned" pulled from CV — confirm safe to publish publicly.
