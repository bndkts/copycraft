---
name: headlines-and-ctas
description: 'Generates headlines and calls-to-action per language: English headline formulas and German native CTAs, never translated "Get started"/"Learn more". Use when the user needs headline options, a hero line, button copy, or CTA wording in English or German. Trigger: "write headlines", "CTA options", "button copy", "hero headline"; German: "Überschriften", "Schlagzeile", "CTA auf Deutsch", "Button-Text", "Handlungsaufforderung". Matches du/Sie from brand-brief.md and maps English CTAs to native German equivalents.'
---

# Headlines & CTAs

Generate headline options, hero lines, and button copy in English or German. The one
rule that separates this skill from a generic translator: a German CTA is **written
native**, never a word-for-word rendering of "Get started" or "Learn more." German
buttons say "Jetzt starten" and „Mehr erfahren“ because that is what German products
actually use — not "Bekomme gestartet" and not a stiff "Lernen Sie mehr."

You produce *options*, not a single answer. Headlines and CTAs are cheap to draft and
expensive to get wrong, so give the user 3–5 to choose from, each with a one-line reason,
and a recommended pick.

## Before you start: read the brand brief

If `.claude/brand-brief.md` (or a brand brief the user pastes) exists, read it first and
let it win over any default here. Pull four things:

- **du or Sie** (German only) — this fixes every pronoun and verb form in your CTAs. The
  worst error in German copy is mixing the two inside one journey, which reads as careless
  on a trust-sensitive brand. Never guess: if the brief is silent and the user hasn't
  said, ask once, then stay consistent.
- **Voice / register** — punchy and informal, or measured B2B? This sets how bold a
  headline can be.
- **Glossary** — product and feature names to use verbatim (and their gender/article in
  German, e.g. *das Dashboard*).
- **Banned words** — honor them in every option.

The skill must still work with no brief: fall back to the craft below, and for German
default to **Sie** when the audience is formal B2B (a wrong Sie costs less than a wrong
du; Strzelecki/CleverReach: „Ein 'Sie' tut niemandem weh“).

## What good headlines and CTAs share

These principles are language-neutral; the *execution* differs by language, so always
finish in the language-specific reference.

- **Benefit first, but earn it with the feature.** Lead with the outcome the reader gets,
  then name the mechanism that makes it true. "Automated monitoring" is a feature; "You
  hear about a fake shop the moment it goes live" is the benefit.
- **One promise per headline.** Two ideas fight; the reader remembers neither. Split a
  double headline into a headline + subhead.
- **Specific beats clever.** A number, a name, or a concrete mechanism beats an adjective.
  "Trusted by many" → "Used by 1,200 security teams." Clarity wins; a headline that needs
  a second read has already lost the scanning reader.
- **CTA = action verb + benefit, matched to the reader.** Lead with the verb, attach the
  payoff, and match the page's pronoun and formality. "Get started" is weaker than "Start
  protecting your brand." One primary action per view.
- **Reduce risk at the button.** A friction-reducer next to the CTA ("No credit card,"
  „Keine Kreditkarte nötig,“ „Jederzeit kündbar“) lowers the cost of saying yes.
- **Competitor copy-paste test.** Could a competitor paste this exact headline onto their
  site without it becoming false? If yes, it says nothing specific — rewrite it.

Optional enrichment if present: `shared/references/conversion-principles.md` (the seven
core principles). This skill does not depend on it.

## Route by language

After you know the language and (for German) du/Sie, read the matching reference for
formulas, the full CTA map, and worked patterns:

| You are writing… | Read |
|---|---|
| English headlines, hero lines, or CTAs | `references/headlines-en.md` |
| German headlines, hero lines, or CTAs (any du/Sie) | `references/headlines-ctas-de.md` |

For a bilingual request, produce each language from its own reference. Do **not** write
the English version and translate it — write the German fresh from the meaning.

## The native-CTA rule (the heart of this skill)

English CTAs do not translate; they **map** to the phrase a native German product would
use. A few from the full table in `references/headlines-ctas-de.md`:

| English origin | Native German |
|---|---|
| Get started / now | Jetzt starten · Jetzt loslegen · Los geht's |
| Learn more | Mehr erfahren · Mehr dazu |
| Start free trial | Kostenlos testen · 30 Tage kostenlos testen |
| Book a demo | Demo vereinbaren · Demo anfragen · Live-Demo ansehen |
| Contact sales | Vertrieb kontaktieren · Kontakt aufnehmen |

Then apply the craft: **action verb first** (Hol dir, Starte, Teste, Sichere dir, Buche);
**attach the benefit** ("Jetzt starten & 20 % sparen" beats a bare "Jetzt starten"); no
weak passive ("Hier können Informationen erhalten werden" → "Hol dir jetzt alle Infos");
and never a vague „Klicken Sie hier“ or „Weiter,“ which say nothing about what happens
next. Match the CTA's pronoun to the page's du/Sie (verb pairs are in the German
reference).

The same instinct applies in reverse for English: a German-thought CTA translated to
English ("Make a request," "Inform yourself") reads foreign. Use native English —
"Get a quote," "See it in action."

## Hard rules vs. contested style

**Hard rules** (genuine errors — fix silently, every time):

- German quotation marks are `„…“` or `»…«`, never straight `"…"` or English `"…"`
  (Duden / DIN 5008).
- No „in“ before a bare year: "in 2024" ✗ → "2024" / "im Jahr 2024" ✓.
- No Deppenleerzeichen in compounds: "Social Media Plattform" ✗ →
  "Social-Media-Plattform" ✓; "Marketing Strategie" ✗ → "Marketing-Strategie" ✓.
- Currency symbol *after* the amount with a space: "1.999,00 €" ✓, not "€1,999.00" or
  "1,99€." Percent with a space: "20 %," not "20%."

**Contested style** (smells to downgrade, never forbid — the user may want them, and
authorities disagree):

- "Sinn machen" — Duden marks it colloquial; **Eisenberg defends it as well-formed German**.
  In polished copy prefer "ergibt Sinn," but do not treat it as an error.
- "am Ende des Tages," "nicht wirklich," "einmal mehr" — calqued idioms that read
  translated; offer a crisper native phrase, but they are style, not mistakes.
- Floskeln (innovativ, ganzheitlich, maßgeschneidert, „führender Partner“) — flag and
  replace with a concrete fact, but this is a quality nudge, not a hard rule.

When you change something contestable, say why in one clause; do not lecture.

## Worked examples

### Example 1 — English hero + CTA

**Input:** "Hero headline for our brand-protection product. Audience: security teams.
Core feature: we get fake sites taken down automatically. We need a button too."

**Output:**
> Headline options (benefit-first, one promise each):
> 1. "Fake sites impersonating your brand, taken down — usually within hours." *(lead
>    benefit + a concrete speed claim as proof)*
> 2. "Stop brand impersonation before your customers get burned." *(stakes-led; agitates
>    the real fear)*
> 3. "Find the phishing sites abusing your brand. Get them offline." *(plain, two verbs,
>    no adjectives)*
>
> **Recommended:** #1 — it pairs the outcome with a specific, checkable time-to-value.
>
> CTA: **"Scan my brand now"** (primary) · friction-reducer: "No credit card."
> Avoid "Learn more" / "Submit" — they hide what the reader gets.

### Example 2 — German button copy from an English mockup (Sie)

**Input:** "Brand brief says Sie, formal B2B security buyer. The Figma mockup has two
buttons: 'Get started' and 'Learn more'. Localize them."

**Output:**
> - "Get started" → **„Kostenlos starten“** or **„Jetzt loslegen“** (action verb first;
>   native, not a translation of *get*).
> - "Learn more" → **„Mehr erfahren“** (the standard native phrase; „Mehr dazu“ as a
>   shorter variant).
>
> Pronoun check: both are imperative and register-neutral, so they read clean in a Sie
> context. If you add a benefit clause, keep Sie: „Mehr erfahren – in 2 Minuten.“ Do
> **not** mix in a du form like „Hol dir mehr Infos“ on a Sie page.

### Example 3 — German hero, du register

**Input:** "Hero line for a self-serve accounting tool, du, founders. Feature: bookkeeping
runs mostly on its own."

**Output:**
> 1. „Mit [Produkt] läuft deine Buchhaltung fast von allein.“ *(Mit + Produkt + Verb;
>    concrete outcome, no Hype)*
> 2. „Buchhaltung für Gründer, die keine Buchhaltung machen wollen.“ *(segment + plain
>    noun + the real job)*
> 3. „Weniger Buchhaltung. Mehr [Kerngeschäft].“ *(contrast pattern, punchy)*
>
> CTA: **„Kostenlos testen“** · friction-reducer: „Keine Kreditkarte nötig.“

## Output format

For each request return: 3–5 labelled options, a one-line reason per option, and a
recommended pick. For CTAs, give a primary action plus a friction-reducer, and flag the
matched du/Sie. If you fixed a hard-rule error (quotes, spacing, currency) in supplied
text, note it briefly. Keep the options native to the target language — never present a
German option that reads like a rendered English string.

## Quality checklist

- [ ] Benefit-first; one promise per headline.
- [ ] CTA = action verb + benefit; one primary action; friction-reducer offered.
- [ ] German CTA is native (mapped via `references/headlines-ctas-de.md`), not translated.
- [ ] du/Sie matches the brief and is consistent across every option.
- [ ] Passes the competitor copy-paste test (no line a rival could reuse verbatim).
- [ ] German typography correct: `„…“`, "20 %", "1.999,00 €", no „in 2024“, no
      Deppenleerzeichen.
- [ ] Contested smells downgraded with a reason, not forbidden.

## Reference files (read on demand)

- `references/headlines-en.md` — English headline formulas (benefit-first, PAS/AIDA as
  scaffolding, specificity, one promise), hero-line patterns, native English CTA examples,
  do/don't pairs. Read when writing English.
- `references/headlines-ctas-de.md` — Auf Deutsch: native CTA-Map, du/Sie-Verbpaare, and
  idiomatic German hero/headline patterns. Read when writing German.
