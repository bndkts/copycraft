---
name: brand-voice
description: >-
  Defines a brand's voice and creates the shared brand-brief.md that every other
  copycraft skill reads. Use when setting up brand copy guidelines, defining tone of
  voice, positioning, target audience, proof points, a terminology glossary, banned
  words, or approved voice samples (Stimmproben) — or deciding du vs. Sie for German.
  Trigger phrases: "set up my brand", "define brand voice", "brand brief", "tone of
  voice", "create brand guidelines", "voice samples"; German: "Markenstimme festlegen",
  "Markenbrief erstellen", "Tonalität definieren", "Anrede du oder Sie festlegen",
  "Marken-Wording", "Stimmproben". Run this first.
---

# Brand Voice

Define a brand's voice and write the single file every other copycraft skill reads:
`.claude/brand-brief.md` in the user's project. This is the foundation skill. Run it
first; `copy-polish`, `texten-de`, `lokalisieren-de`, `du-sie-check`, `landing-page`,
`seo-copy`, and the rest all consult the brand brief so they stay consistent and never
re-ask the basics.

Your job here is not to write marketing copy. It is to **interview the user, make the
hard decisions explicit, and record them** in a brief that downstream skills can obey.

## When to use

- The user is setting up a brand, a product, or a new copy project.
- The user asks for tone of voice, positioning, target audience, proof points, a
  terminology glossary, or a banned-words list.
- The user needs to decide **du or Sie** for German copy (and have it stick).
- Any other skill notices there is no `.claude/brand-brief.md` and the work needs one.

## First, check for an existing brief

Before interviewing, look for `.claude/brand-brief.md` in the user's project.

- **If it exists:** read it. Summarize what's already decided (voice, du/Sie, glossary,
  banned words) and ask what they want to change or fill in. Update in place — don't
  silently overwrite a working brief.
- **If it doesn't exist:** start from `references/brand-brief-template.md` and run the
  interview below.

Never *require* the brief to exist to start — you are the skill that creates it.

## The output and why it's one file

Everything lands in **`.claude/brand-brief.md`** in the user's project root. One file,
checked into their repo, human-editable. The reason for a single source of truth: voice
drift is the most common failure in multi-author (and multi-prompt) copy. If each skill
guessed the tone, every page would sound slightly different. The brief makes the brand's
decisions binding so the other skills don't re-litigate them.

## The interview

Walk the user through the sections below **conversationally** — a few questions at a
time, not a 30-question wall. Reflect their answers back in their own words. Where they're
vague ("we want to sound professional"), push for the specific (see Examples). Use the
fill-in structure and the one filled example in `references/brand-brief-template.md` as
your scaffold.

**1. Company / product one-liner.** What is it, for whom, in one sentence — no adjectives,
no hype. If they can't say it plainly, that's the first thing to fix.

**2. ICP & buyer.** Who reads the copy? Capture the role(s), their **fears**, and their
**wants**. Buyer and user can differ (a CISO signs, an analyst uses). Fears matter as much
as wants: the more a market fears being burned (security, finance, health), the more the
copy must lead with proof, not promises.

**3. Positioning & primary value prop.** What does this brand do better/differently, and
what's the one outcome the reader gets? Apply the competitor copy-paste test: *could a
competitor paste this onto their site without it becoming false?* If yes, it's filler —
push for something only this brand can say.

**4. Voice: 3–5 adjectives + 1–2 anti-adjectives.** The anti-adjectives matter as much as
the adjectives — "warm, plain, confident, but never hypey, never jargon-heavy" tells you
where the line is. If the user gives generic words ("professional, trustworthy"), read
`references/voice-dimensions.md` and walk them through the adjective↔anti-adjective pairs
to land something specific. Record the difference between **voice** (constant) and **tone**
(shifts by context — an error page vs. a launch headline).

**5. The Anrede decision (German): du OR Sie — stated once, binding.** This is the section
users most often get wrong, so make the call explicit and record it. See the next heading.

**6. Proof points / trust signals.** The checkable facts that make claims believable:
certifications, customer counts, response times, named clients, guarantees, hosting
location. These replace adjectives like "leading" and "trusted." Seed the conversation
from the trust vocabulary in `references/brand-brief-template.md` (GDPR-compliant,
ISO-certified, data hosted in Germany, response within 24 hours, 1,200+ customers, fixed
point of contact, transparent pricing). Record only facts the user can actually back.

**7. Terminology glossary (bilingual).** The words this brand uses and how it spells them —
especially which English tech terms stay English in German copy (das Feature, das
Dashboard, Takedown, Phishing) and which get a German word (Meeting → Sitzung if that's
the brand's choice). Capture canonical spelling and the EN↔DE equivalent so translation
and localization stay consistent. Use the glossary table in the template.

**8. Banned words.** Seed from the Floskeln / filler blacklist in the template (innovativ,
ganzheitlich, maßgeschneidert, "Lösungen aus einer Hand", world-class, cutting-edge,
seamless, "Ihr starker Partner" …) and invite the user to extend it with their own pet
peeves. Each banned word should be replaced by a concrete fact, number, or mechanism — not
just deleted.

**9. Voice samples (Stimmproben) — the strongest voice control in the brief.** Adjectives
*describe* the voice; samples *demonstrate* it — and downstream skills imitate a sample far
more faithfully than they obey an adjective. Collect 3–5 real, **approved** lines of
on-brand copy, each labeled with its surface (hero, feature blurb, email opener, CTA +
friction-reducer). Source them from existing copy the user is proud of. If nothing usable
exists yet, **co-draft them right here**: propose one on-voice line from the answers so
far, refine it with the user until they say "yes, that's us," and record that. Also capture
**one counter-example** — a sentence that is exactly what the brand must never sound like
(ideally a real rejected draft) — with a one-line *why it's off*. Tell the user the
generation skills will match the samples' sentence length, rhythm, and word choice; when a
sample and an adjective pull apart, the sample wins.

## The du/Sie decision (German), made binding

Record **one** choice — du or Sie — and the verb forms that follow from it. The single
worst error is **mixing du and Sie within one journey** (hero siezt, the form duzt); for a
trust-sensitive brand that reads as carelessness. The brief exists to prevent exactly that;
`du-sie-check` later enforces it.

Decide by **audience and channel, not by how "techy" the product is**:

- **Sie** fits formal B2B, HR, sales, enterprise, and trust-sensitive buyers
  (security, compliance, finance, insurance). Modern, warm Sie — not Amtsdeutsch.
- **du** fits tools for individuals, small teams, freelancers, consumer, and fintech —
  *if* du runs through every surface consistently.
- Channels may differ (Sie on the website, du on Instagram) **only** if each channel is
  internally consistent end to end.

Useful asymmetry when unsure: directional studies (Appinio 2019, n≈4,877 — 61% read Siezen
as respect, only 8% want it abolished; Kundenmonitor Assekuranz 2022 — 53% prefer "Sie" in
advisory contexts) suggest **a wrong Sie costs less than a wrong du**. These figures are
directional, not fresh-2026 SaaS data — let audience judgment govern. Note: Anrede is *not*
tonality; you can be warm with Sie and stiff with du. Closeness comes from phrasing, not the
pronoun.

Once chosen, record the verb pairs the brand will use so copy never drifts — e.g.
**Sie:** Testen Sie · Holen Sie sich · Sichern Sie sich · Ihr/Ihre · Ihnen; or
**du:** Teste · Hol dir · Sichere dir · Dein/Deine · dir. The template has the full pair
list with one column for the brand's choice.

## Hard rules vs. contested style (so the brief doesn't overreach)

When seeding the banned-words and glossary sections, keep two categories separate, because
a brief that forbids legitimate phrasing makes downstream skills wrong:

- **Hard rules** — genuine errors, safe to ban outright: `in 2024` (use `2024` /
  `im Jahr 2024`); the Deppenleerzeichen (`Social Media Plattform` → `Social-Media-Plattform`);
  straight or English quotation marks (use `„…“`); glued/mis-ordered currency
  (`1,99€` → `1,99 €`). Source: Duden / DIN 5008.
- **Contested style** — "smells" to discourage, **never** forbid: `Sinn machen`
  (linguist Peter Eisenberg argues it is not provably an anglicism; Duden lists it as
  *umgangssprachlich*), `am Ende des Tages`, `nicht wirklich`, `es braucht`,
  `die Extrameile`. If the user wants one of these banned anyway, that's their brand
  choice — record it as a *brand preference*, not as a correctness rule, so the reason is
  honest.

Filler Floskeln (innovativ, ganzheitlich, world-class) are fair to ban: they say nothing a
competitor couldn't say. That's a content judgment, not a grammar claim.

## Examples

**Example 1 — Vague voice → specific voice (Input → Output)**

> **Input (user):** "We want to sound professional and trustworthy."
>
> **Output (you):** "Professional and trustworthy" is where every competitor lands, so it
> won't guide a single sentence. Let's make it specific. From the pairs in
> `voice-dimensions.md`: are you **warm** or **formal**? **plain** or **technical**?
> **calm** or **urgent**? Based on a security buyer, I'd propose:
> *Voice: clear, calm, precise, quietly confident. Anti-voice: hypey, jargon-heavy, alarmist.*
> Quick test — a status line. Generic: "We deliver trusted, world-class protection."
> On-voice: "We found 14 fake shops using your logo last month and took down 12."
> Want me to lock those four adjectives and two anti-adjectives into the brief?

*Why:* generic adjectives can't be obeyed; specific pairs plus a sample line make the voice
checkable. Proof replaces the puffery.

**Example 2 — du/Sie decision recorded (Input → Output)**

> **Input (user):** "We're a B2B brand-protection tool for compliance teams in DACH.
> We're modern, though — not stiff."
>
> **Output (you):** Recommendation: **Sie**, in a modern, warm register (no Amtsdeutsch).
> Your buyers are compliance and security teams — a market where a wrong *du* reads as
> careless, and a *Sie* costs nothing. "Modern" lives in the phrasing, not the pronoun.
> I'll record it as binding and set the verb forms: *Testen Sie · Sichern Sie sich ·
> Holen Sie sich · Ihr/Ihre · Ihnen.* One rule on top: never mix — if the hero siezt, the
> signup form, tooltips, and emails all siezen too. `du-sie-check` will enforce this later.

*Why:* the decision is stated once, justified by audience and the asymmetric cost, and the
verb forms are captured so no surface drifts.

**Example 3 — Glossary + banned word (Input → Output)**

> **Input (user):** "In German, do we write 'Takedown' or translate it? And please kill
> 'maßgeschneidert', I hate it."
>
> **Output (you):** "Takedown" stays English in your field (it's an established term with
> no clean German equivalent) — capitalized as a noun: *der Takedown, den Takedown
> beauftragen.* I'll add a glossary row: `Takedown | stays English: yes | — | "Takedown"
> | EN takedown ↔ DE Takedown`. And I'll add **maßgeschneidert** to banned words with the
> reason "filler — say what's actually configurable instead," so the replacement is a fact,
> not a deletion.

*Why:* the glossary fixes spelling and the EN↔DE mapping once; the banned word carries a
replacement instruction so copy improves rather than just shrinking.

## Write the file

Assemble answers into `.claude/brand-brief.md` using `references/brand-brief-template.md`.
Fill every section you have answers for; leave a clearly marked `TODO` for the ones the
user skipped, so the gap is visible rather than invented. Show the user the result and
confirm the du/Sie line, the proof points, and the voice samples especially — those are
the highest-leverage, most-misremembered fields. Tell them the other skills will now read
this file automatically.

## References — read these when relevant

| File | When to read it |
|---|---|
| `references/brand-brief-template.md` | Always — it's the structure you fill in, with the verb-pair list, trust-vocabulary seeds, glossary columns, the Floskeln banned-words seed, the voice-samples (Stimmproben) section, and one filled example (nebty, B2B security, Sie). |
| `references/voice-dimensions.md` | When the user's voice words are vague or they want help choosing — adjective↔anti-adjective pairs, a menu of dimensions, and the voice-vs-tone distinction. |

**Optional enrichment (not required):** if working inside the full copycraft plugin,
`shared/references/conversion-principles.md` covers the language-neutral conversion
principles (benefits over features, show proof, the competitor copy-paste test) that the
positioning and proof-point sections draw on. The brand-voice skill works without it.
