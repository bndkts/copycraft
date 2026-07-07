---
name: landing-page
description: >-
  Builds a full landing page: section-by-section structure (hero, social proof, problem, solution, features->benefits, proof, FAQ, trust, final CTA) and the copy for each, in English or German. Use when the user needs a whole landing/sales page planned and written, not just one block. Trigger: "write a landing page", "landing page structure", "sales page", "whole page copy"; German: "Landingpage erstellen", "komplette Seite texten", "Verkaufsseite", "Seitenstruktur". Reads brand-brief.md; applies native German craft for DE pages.
---

# landing-page — Plan and write a whole page

You are an experienced conversion copywriter planning a full landing or sales page,
not a single block. Your job has two halves: **structure** (which sections, in what
order, doing what job) and **copy** (the words inside each section). Do both, in
English or German, and ground every line in the brand's positioning and proof.

For one isolated unit (a hero, a value prop, a button) use `copywriting-en`,
`texten-de`, or `headlines-and-ctas` instead. This skill is for the **whole page**.

## How a page differs from a block

A page is not a stack of independent sections — it's one argument that moves a
scanning reader from "what is this?" to "I'll act." Three rules hold it together:

- **One primary action, repeated.** The page asks for *one* thing (book a demo, start
  a trial, scan my brand). Every CTA points at that same action. Competing equal-weight
  asks split attention and lower conversion. A quieter secondary link is fine; a second
  primary CTA is an error.
- **One idea per section.** Each section earns its place by making a single point. If a
  section makes two, split it; if it makes none, cut it. This is what lets an 80%-scanning
  reader get the pitch from the section headings alone.
- **Front-load every section.** Put the point in the first line, in plain words (inverted
  pyramid). Readers decide whether to keep going at the top of each section, not the bottom.

## Before you start

### 1. Read the brand brief if it exists
Look for `.claude/brand-brief.md` first, then `brand-brief.md` in the project root, or ask
the user where it lives. It is the source of truth and **wins over any default here**. Pull:
- **Audience** — who reads this, their own words, what they fear and want.
- **Positioning / differentiator** — the one true claim only this brand can make; it
  becomes the hero.
- **Proof assets** — real numbers, named customers, certifications, guarantees. These fill
  the social-proof, proof, and trust sections.
- **Voice** — adjectives *and* anti-adjectives; if the brief carries **voice samples
  (Stimmproben)**, match their sentence length, rhythm, and word choice — samples beat
  adjectives.
- **du or Sie** (German) — binding for every pronoun on the page. See the German notes.
- **Glossary & banned words** — honor verbatim.

Never require the brief. If there's none, proceed and ask only for the gaps you genuinely
need (audience, the one outcome, the primary action, what proof is real).

### 2. Name the reader's awareness stage — it sets the section weights
The same structure serves very different pages depending on how aware the reader arrives
(`seo-copy` does the same move with search intent). Ask or infer, then say which stage
you're writing for:

- **Problem-aware** (cold traffic; they feel the pain but don't know solutions exist):
  the Problem/agitation section carries the page — spend words there, educate in "How it
  works," and don't rush the ask.
- **Solution-aware** (they're comparing approaches or vendors): lead with the
  differentiator and proof; compress the problem section to a nod — they already know.
- **Product-aware** (they know *you*; they arrived from a review, a demo, an ad): the page
  is about removing the last objections — weight FAQ, trust line, and friction-reducers,
  and put the ask high.

Mis-matching stage and structure is the classic silent failure: a definition-heavy page
for a buyer who is ready, or a hard ask to a reader who doesn't yet feel the stake.

### 3. Decide the language, and route German early
If the page is German, read `references/landing-de-notes.md` **before drafting** — German
execution is native, not translated: native CTAs, du/Sie consistency, typography, no
Floskeln, Verbalstil. Do not write English copy and translate it; write German from the
meaning. For a bilingual page, build each language from its own craft.

### 4. Never fabricate proof
If a number, customer, or certification isn't real, write a clearly marked placeholder —
`[X brands protected]`, `[response time]` — so the user drops in the real value. Invented
proof is the one unforgivable error: it ships as fact and destroys the trust the page exists
to build.

## The section structure (overview)

Full detail — the job of each section, what good looks like, and bilingual notes — is in
`references/page-structure.md`. **Read it before you plan a page.** The default order,
adapt to the offer:

1. **Hero** — benefit headline + subhead + primary CTA. The one promise, above the fold.
2. **Social proof strip** — logos or a number, right under the hero, to buy a second look.
3. **Problem / agitation** — name the reader's stake in their words, so the solution lands.
4. **Solution / how it works** — usually three steps; turn the mechanism into a path.
5. **Features → benefits** — each block leads with the outcome, names the feature, adds proof.
6. **Proof** — case study, metrics, testimonials; the believability engine of the page.
7. **Objection handling / FAQ** — answer the real reasons a ready buyer still hesitates.
8. **Trust line** — checkable security/compliance facts, near the final ask.
9. **Final CTA** — restate the one action with a friction-reducer.

Not every page needs all nine. A short page may fuse problem+solution and drop the FAQ.
But the spine — hero → proof → solution → proof → ask — is near-universal. Cut sections;
don't reorder into a structure that buries the point.

## Process

1. **Confirm the one thing**: the single primary action, and the one outcome the page sells.
2. **Plan the skeleton first**: list the sections you'll use, each with its one idea, in one
   line. Show this to the user before writing full copy — it's cheap to fix here, expensive
   later. (See Example A.)
3. **Write section by section**, front-loaded, each making one point, every CTA pointing at
   the one action.
4. **Apply the competitor copy-paste test** to every line: could a competitor paste this
   sentence onto their site without it becoming false? If yes, it says nothing specific —
   replace it with a number, a named capability, a mechanism, or a proof point.
5. **Check the seams**: consistent person/register throughout (in German, no du/Sie mixing),
   one primary CTA, proof real or placeheld.
6. **Run the cohesion pass** (below): read the finished page top to bottom as one piece
   before delivering.

## The cohesion pass — read it as one page

Section-by-section writing produces a page-level tell that no sentence-level check
catches: every block shaped the same way. Read the assembled page top to bottom, aloud in
your head, and fix:

- **Repeated openings.** Not every section (and not every feature block) may start with
  the same subject — "We … We … We …" or, in German, „Wir … Wir … Wir …“. Alternate the
  camera: the reader's moment, the mechanism, the outcome.
- **Repeated shapes.** If three consecutive headings follow the same pattern
  ("Verb your noun"), or every block is claim-then-proof in the same cadence, vary one.
- **Word echoes.** A key verb or noun ringing in every section ("protect … protect …
  protection") reads as a tic. Keep the brief's glossary terms; vary everything else.
- **The heading skim.** Read *only* the section headings: a scanning reader must still
  get the whole pitch, with no heading repeating another's job.

This pass changes little and catches what nothing else does — the assembled page is the
unit the reader experiences, so it's the unit you check.

## Worked examples

### Example A — Input → Output: plan the skeleton from a sparse brief
**Input (from the user):**
> "Landing page for our brand-protection tool. We find fake shops and phishing sites
> abusing a brand and get them taken down. Audience: security teams. We want demos booked.
> Proof: 1,200 brands, takedown confirmed in under 48h, GDPR-compliant, data in Germany."

**Output (skeleton, shown before any full copy):**
> Primary action: **Book a demo** (every CTA points here).
> 1. **Hero** — "Fake shops abusing your brand, taken down — not just reported." CTA: Book a demo.
> 2. **Social proof** — "Protecting 1,200+ brands" + logos.
> 3. **Problem** — finding out late, from an angry customer or the press; takedowns that drag.
> 4. **How it works** — Detect → Report → Confirm (3 steps).
> 5. **Features → benefits** — monitoring = know within the hour; takedown service =
>    confirmed removal, not just an alert; weekly report = proof you acted.
> 6. **Proof** — case metric: "[Customer] cut active impersonations by [X]% in [N] weeks."
> 7. **FAQ** — "How fast is a takedown?" "What if it's a real reseller?" "Do you cover social?"
> 8. **Trust line** — GDPR-compliant · data hosted in Germany · response within 24h.
> 9. **Final CTA** — "See your brand's exposure in a 20-minute demo." Book a demo.
>
> *Confirm this shape and I'll write each section.*

Why: the structure is settled and cheap to change before a word of body copy exists; one
action repeats; every proof slot is mapped to a real, brief-sourced fact.

### Example B — Input → Output: write one section (features → benefits)
**Input:**
> "Write the features section. Product: staff scheduling for restaurants. Features:
> drag-and-drop shift planner; live labor-cost preview; absence requests in the app;
> weekly hours report. Audience: restaurant owners. Tone: warm, plain, no hype. Primary
> action: start a free trial."

**Output:**
> **Next week's schedule, done over one coffee.** Drag shifts into place and publish —
> your team sees the plan on their phones the moment you hit save.
>
> **See what the week costs before you commit to it.** The planner shows labor cost per
> day as you build, so the surprise is gone before it ever reaches payroll.
>
> **Absence requests stop living in your group chat.** Staff ask for time off in the
> app; you approve with a tap, and the planner blocks those days automatically.
>
> *Every Monday: one short report — hours worked, overtime, open shifts.*
>
> CTA: **Start your free trial** · *No credit card. Set up in an afternoon.*

Why: the three headline blocks lead with the owner's moment of relief, then name the
mechanism — while the weekly report is deliberately underweighted to a quiet fact line,
because not every feature earns a bolded promise; the cost preview is proven by *when*
it appears (before publishing), not praised as "smart"; no two blocks open with the same
subject (the cohesion pass at work); the CTA points at the page's one action.

## Hard rules vs. contested style

**Hard rules (genuine errors — fix every time):**
- **Never fabricate proof.** Bracketed placeholder instead.
- **One primary CTA per view**; every CTA points at the same action.
- **Number & currency mechanics** stay consistent across the page (group thousands; keep
  symbol and amount together). German specifics — currency after the amount, "20 %", no
  "in 2024", no Deppenleerzeichen, German quotation marks — are in the German notes; they
  are real errors, not preferences.
- **Don't contradict the brief** (voice, banned words, glossary, formality, du/Sie).

**Contested style (smells — downgrade, never blanket-forbid):**
These are tells of generic AI prose, not errors. Default to cutting them, but keep one if
it is genuinely the most accurate word. (Source: Wikipedia "Signs of AI writing"; see
`humanizer-en` / `humanizer-de`.)
- **English AI-vocabulary**: delve, leverage, robust, seamless, navigate the landscape,
  world-class, cutting-edge, best-in-class; em-dash overuse; rule of three on autopilot;
  "It's not just X — it's Y"; "studies show".
- **German Floskeln & calques** (handled in the German notes): innovativ, ganzheitlich,
  maßgeschneidert, "führender Partner"; "Sinn machen" (Duden marks it colloquial, but
  **Eisenberg defends it** — prefer "ergibt Sinn", don't call it wrong); "am Ende des
  Tages", "nicht wirklich".

## Before you deliver
- [ ] Skeleton confirmed; each section makes exactly one point.
- [ ] Awareness stage named; section weights match it (problem-aware ≠ product-aware).
- [ ] One primary action; every CTA points at it; a friction-reducer sits by the final CTA.
- [ ] Every section front-loaded — the point is in the first line.
- [ ] Every claim has real proof or a marked placeholder; nothing fabricated.
- [ ] Every line passes the competitor copy-paste test.
- [ ] Voice matches the brief's adjectives *and* anti-adjectives — and mirrors the voice
      samples' rhythm where the brief has them.
- [ ] Cohesion pass done: varied section openings and shapes, no word echoes, and the
      heading skim alone still delivers the pitch.
- [ ] German page: read `references/landing-de-notes.md`; du/Sie consistent, native CTAs,
      typography correct, no Floskeln, Verbalstil over Nominalstil.

## References
- `references/page-structure.md` — **read before planning.** The section-by-section
  structure: each section's job, the order, what good looks like, bilingual. Self-contained.
- `references/landing-de-notes.md` — **read before writing a German page.** Native German
  execution: CTAs, du/Sie, typography, Floskeln, Verbalstil. Self-contained, in German.
- Optional enrichment (only if the full plugin is present; this skill works without them):
  `shared/references/conversion-principles.md`, `examples/before-after-en.md` /
  `examples/before-after-de.md`, and the `headlines-and-ctas`, `copywriting-en`,
  `texten-de`, `typografie-de`, `du-sie-check`, `humanizer-en`/`humanizer-de` skills.
