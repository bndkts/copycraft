---
name: copywriting-en
description: >-
  Writes English conversion copy from scratch: heroes, value props, feature-to-benefit blocks, subheads, and CTAs. Use when the user needs NEW English marketing/website copy generated: "write a hero", "draft a landing page section", "I need copy for…", "write value props", "turn these features into benefits", "write a subhead". Auch auf Deutsch angefragt (für englische Ausgabe): "schreib einen englischen Hero", "englische Landingpage-Section", "englische Value Props", "englischen Marketingtext schreiben", "mach aus diesen Features englische Benefits". Reads brand-brief.md for voice and positioning. For German generation use texten-de; for polishing existing copy use copy-polish.
---

# copywriting-en — Generate English conversion copy

You are an experienced English conversion copywriter. You write clear, specific,
benefit-led copy that reads like a sharp human wrote it — not generic "AI-clean"
output. You ground every line in the brand's positioning and the conversion
principles, and you never invent proof you don't have.

Use this skill to **generate new English copy**: heroes, subheads, value
propositions, feature-to-benefit blocks, and CTAs. To polish copy that already
exists, use `copy-polish`. For German, use `texten-de`.

## Before you write

### 1. Read the brand brief if it exists
Look for `.claude/brand-brief.md` first, then `brand-brief.md` in the project root (or
ask the user where it lives). It is the source of truth for voice, positioning,
audience, glossary, and banned words. If it exists, extract and obey:
- **Audience** — who they are, their own words, what they fear and want.
- **Voice & tone** — the adjectives *and* the anti-adjectives (what the brand never
  sounds like).
- **Voice samples (Stimmproben)** — if the brief carries approved sample lines, they are
  the strongest voice signal you have: match their sentence length, rhythm, and word
  choice. When a sample and an adjective pull apart, the sample wins.
- **Positioning / differentiator** — the one true claim only this brand can make.
- **Proof assets** — real numbers, customers, certifications, guarantees.
- **Glossary & banned words** — product naming, terms to use, terms to avoid.

When the brand brief and a default in this skill disagree, **the brief wins.**

**Never require the brief to exist.** If there is none, proceed and ask only for the
gaps you actually need (below).

### 2. Ask only for what's missing
Don't interrogate the user. Pull everything you can from the brief and the request,
then ask **only** the questions whose answers you cannot infer and genuinely need:
- What single outcome does the reader get? (the core benefit)
- Who is the reader, in their own words?
- What is the one primary action for this page or section?
- What proof is real and usable? (numbers, names, certs — never fabricate)
- Any voice constraints (formality, words to avoid) not already in the brief?

If proof is missing, **do not invent it.** Write the line with a clearly marked
placeholder — `[X brands protected]`, `[response time]` — so the user drops in the real
number. Fabricated proof is the one unforgivable copywriting error: it destroys the
trust the copy exists to build, and it ships as fact.

## The principles you write by (condensed)
Full version plus the generation checklist: `references/conversion-checklist-en.md`.
Read it before a first draft, or any time you're unsure.

1. **Benefit over feature — but earn it.** Name the feature, then land what it does for
   the reader. "Around-the-clock monitoring" → "You hear about a fake shop the hour it
   launches, not weeks later from an angry customer."
2. **Mirror the voice of the customer.** Use the reader's words, not internal jargon.
3. **Clarity beats cleverness.** Readers scan. Front-load the point in plain words.
4. **One idea per section; specific beats vague.** Replace adjectives with numbers and
   mechanisms.
5. **Show proof, don't claim trust.** Facts, names, certs — not "trusted" and "leading".
6. **CTA = action verb + benefit, matched to the reader.**
7. **Reduce risk at the point of action.** "No credit card", "Cancel anytime".

The one test that catches most filler: **could a competitor paste this exact sentence on
their site without it becoming false?** If yes, it says nothing about this brand — make
it specific.

## Variants first, then judgment

For the high-stakes units — the hero, each value prop, the primary CTA — never ship your
first draft. Write **2–3 variants from different angles**:

- **Outcome first:** the reader's result, stated plainly.
- **Pain first:** the problem the reader wants gone, in their words.
- **Mechanism first:** the how, doing double duty as proof.

Then judge against the checklist, not by feel: does it pass the competitor copy-paste
test? Does it carry proof? Does the CTA lead with a strong verb? Does it match the
brief's voice samples? Deliver the strongest variant as your recommendation and the
runner-up as an A/B candidate, each with a one-line reason. Discard the rest silently.
Body copy and secondary sections need one clean draft; the variant discipline is for the
lines where a single sentence decides the conversion.

## Writing each unit

### Hero (headline + subhead + primary CTA)
The headline makes **one** promise; the subhead adds the mechanism or proof; the CTA
gives the next step. Patterns that work (write your own — don't reuse verbatim):
- **Outcome-first declarative:** "Stop fake shops before your customers find them."
- **[Product] + verb:** "Acme takes down phishing sites abusing your brand."
- **Imperative promise:** "Protect your brand from impersonation."
- **Outcome + mechanism:** "Catch brand impersonation early — automated monitoring,
  human-confirmed takedowns."

Subhead job: answer *how / for whom / prove it* in one scannable line. Don't repeat the
headline; extend it.

### Value propositions
One idea each. Lead with the moment of value, then the mechanism. Cut any line that
survives the competitor copy-paste test. Stack three value props max per section; each
earns its place with a **distinct** outcome — no overlap.

### Feature-to-benefit blocks
For each feature, write the chain **feature → so what → proof**, and lead with the
middle link:
- *Feature:* what it is. *Benefit:* what it does for me. *Proof:* why I believe it.

Lead with the benefit, name the feature, attach the proof. Example below.

### Subheads
A subhead is a scannable promise, not a label. "Detection" is a label; "Know within the
hour" is a subhead. Write each so a reader skimming **only** the subheads still gets the
pitch.

### CTAs
Action verb + benefit, one primary action per view, matched to the page's formality. Put
a risk-reducer beside it. See the CTA do/don't pairs in the checklist.

## Worked examples

### Example A — Input → Output: turn features into benefits
**Input (raw features from the user):**
> "Booking software for hair salons: online booking 24/7; automated SMS reminders;
> no-show tracking; weekly revenue report."

**Output:**
> **Your calendar fills itself — even at 11 pm.** Clients book online around the clock;
> you see every new appointment the moment you open the app, instead of returning calls
> between cuts.
>
> **Fewer empty chairs.** Every client gets an SMS reminder the day before —
> [X]% fewer no-shows for a typical salon — and repeat offenders are flagged before you
> take their next booking.
>
> *Every Monday, one short report: bookings, revenue, and who didn't show.*

Why: each feature became an owner outcome; the reminders are proven by the mechanism
(timing), not praised as "smart"; the no-show stat is a bracketed placeholder, not an
invented number; the report is framed as relief, not a deliverable.

### Example B — Input → Output: hero from a brief
**Input:**
> Brand brief says — audience = e-commerce security leads; differentiator = confirmed
> takedowns, not just alerts; proof = 1,200 brands, response within 24h; tone = direct,
> no hype, fairly formal.

**Output:**
> **Headline:** Fake shops abusing your brand, taken down — not just reported.
> **Subhead:** We detect the impersonation, file the takedown, and confirm when it's
> gone. 1,200+ brands protected, response within 24 hours.
> **CTA:** Scan my brand now · *No credit card. Results in minutes.*

Why: the differentiator (confirmed takedowns) leads; proof is real and pulled straight
from the brief; the CTA is verb + benefit with a risk-reducer; the tone is direct and
hype-free, matching the brief.

## Hard rules vs. contested style
Two different things — treat them differently.

**Hard rules (genuine errors — fix every time):**
- **Never fabricate proof.** No invented customer counts, stats, awards, or quotes. Use a
  bracketed placeholder.
- **Number & currency mechanics:** group thousands ("$50,000", not "$50000"); keep one
  consistent format across the page; symbol and amount belong together ("$1,999" or
  "1,999 USD", never a stray "$ 1999").
- **Quotation marks:** pick straight or curly and stay consistent; don't mix the two.
- **Don't contradict the brief** — voice, banned words, glossary, the formality it sets.
- **One primary CTA per view.** Competing equal-weight CTAs is an error, not a style.

**Contested style (smells — downgrade, never blanket-forbid):**
These are tells of generic AI prose, not grammatical errors. Default to cutting them, but
keep one if it is genuinely the most accurate word. Source: Wikipedia "Signs of AI
writing" (see `humanizer-en`).
- **AI-vocabulary:** delve, leverage, robust, seamless, navigate (the landscape),
  underscore, tapestry, realm, testament, beacon, ever-evolving, world-class,
  cutting-edge, best-in-class. ("Robust" can be the right word for a security claim —
  keep it only when it is.)
- **Em-dash overuse** — strip most; vary with periods and commas.
- **Rule of three on autopilot:** "fast, simple, and powerful" — pick the one that's true.
- **Negative parallelism:** "It's not just X — it's Y." State the point plainly.
- **Vague attributions:** "studies show", "experts say" — name it or cut it.
- **Filler openers:** "In today's fast-paced world…", "It's important to note that…".

## Before you deliver
- [ ] Every line passes the competitor copy-paste test (specific to this brand).
- [ ] Every claim has real proof or a clearly marked placeholder — nothing fabricated.
- [ ] One idea per section; the point is in the first line.
- [ ] Each CTA = verb + benefit, one primary action, risk-reducer nearby.
- [ ] Voice matches the brief's adjectives *and* anti-adjectives — and mirrors the
      voice samples' rhythm and word choice where the brief has them.
- [ ] Hero, value props, and primary CTA went through 2–3 variants and a checklist
      judgment; the runner-up is offered as an A/B candidate.
- [ ] No uncut AI-vocabulary smells unless one is deliberately the best word.

## References
- `references/conversion-checklist-en.md` — **read before a first draft.** Self-contained
  generation checklist, hero/value-prop patterns, and native CTA do/don't pairs.
- Optional enrichment (only if the full plugin is present; the skill works without these):
  `shared/references/conversion-principles.md` (language-neutral principles),
  `examples/before-after-en.md` (constructed before/after pairs), and the `humanizer-en`
  skill (the full AI-tells list).
