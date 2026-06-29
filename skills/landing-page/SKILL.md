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
Look for `brand-brief.md` (often in `.claude/`), or ask the user where it lives. It is the
source of truth and **wins over any default here**. Pull:
- **Audience** — who reads this, their own words, what they fear and want.
- **Positioning / differentiator** — the one true claim only this brand can make; it
  becomes the hero.
- **Proof assets** — real numbers, named customers, certifications, guarantees. These fill
  the social-proof, proof, and trust sections.
- **Voice** — adjectives *and* anti-adjectives.
- **du or Sie** (German) — binding for every pronoun on the page. See the German notes.
- **Glossary & banned words** — honor verbatim.

Never require the brief. If there's none, proceed and ask only for the gaps you genuinely
need (audience, the one outcome, the primary action, what proof is real).

### 2. Decide the language, and route German early
If the page is German, read `references/landing-de-notes.md` **before drafting** — German
execution is native, not translated: native CTAs, du/Sie consistency, typography, no
Floskeln, Verbalstil. Do not write English copy and translate it; write German from the
meaning. For a bilingual page, build each language from its own craft.

### 3. Never fabricate proof
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
> "Write the features section. Features: 24/7 monitoring; automated detection; managed
> takedown; weekly report. Audience: security teams. Tone: direct, no hype."

**Output:**
> **Know the moment someone clones your brand.** We watch the web and social platforms
> around the clock and flag impersonations automatically — usually within the hour, not at
> the next quarterly review.
>
> **We don't just spot it — we get it removed.** Our team files the takedown and confirms
> when the fake is gone, so you're not chasing platforms yourself.
>
> **Proof you acted, every Monday.** One short report: what we found, what we removed,
> what's still open. *[Tie to a real metric if you have one.]*
>
> CTA: **Book a demo** · *20 minutes, no prep needed.*

Why: each feature leads with the reader's outcome, then names the mechanism; "automated
detection" is proven by the speed rather than dropped as a buzzword; the CTA still points
at the page's one action.

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
- [ ] One primary action; every CTA points at it; a friction-reducer sits by the final CTA.
- [ ] Every section front-loaded — the point is in the first line.
- [ ] Every claim has real proof or a marked placeholder; nothing fabricated.
- [ ] Every line passes the competitor copy-paste test.
- [ ] Voice matches the brief's adjectives *and* anti-adjectives.
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
