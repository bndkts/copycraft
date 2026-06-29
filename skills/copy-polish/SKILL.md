---
name: copy-polish
description: 'Polishes and tightens existing marketing/website copy without rewriting it: sharpens clarity, voice, proof, specificity, and CTAs. Detects the language and applies the right passes — English "Seven Sweeps", German "Lektorat" that removes translationese. Use whenever the user wants to improve, edit, tighten, "make better", review, lektorieren, or fix existing copy (heroes, landing pages, feature blurbs, emails) in English or German. German triggers: "mach den Text besser", "lektorieren", "Text überarbeiten", "klingt übersetzt", "Copy verbessern", "entkrampfen". English triggers: "polish this", "tighten this copy", "edit my landing page", "improve this hero".'
---

# Copy Polish

Improve copy the author already wrote — without taking it away from them. The job is to
sharpen clarity, voice, proof, specificity, and the call to action while keeping the
author's intent and rhythm. You change only what earns the change. A polish that returns
unrecognizable copy has failed, even if the new copy is "better."

This skill is bilingual. English copy gets the **Seven Sweeps** editorial passes. German
copy gets the **Lektorat** pass, which additionally hunts translationese (calques,
Denglisch, Nominalstil, Floskeln) that an English-tuned edit would miss. Detect the
language first, then run the matching engine.

## When to use this vs. a rewrite skill

Use `copy-polish` to **improve existing copy**. If the user has no copy yet and wants
something written from scratch, that is a job for `copywriting-en` or `texten-de`. If the
copy is fine but reads AI-generated, `humanizer-en` / `humanizer-de` are the sharper tools.
Polish overlaps with all of these and will borrow their rules, but its discipline is
**minimal, voice-preserving edits**, not generation.

## Workflow

Run these steps in order. Do not skip step 2 — naming the job out loud is what keeps you
from rewriting copy that only needed a trim.

### 1. Detect the language and load the right engine

- **English copy** → apply the Seven Sweeps. Read `references/seven-sweeps-en.md`.
- **German copy** → apply the Lektorat pass. Read `references/lektorat-de.md` (it is
  written in German). The German reference is the anti-translationese engine and is the
  half most likely to be needed, because German marketing copy is so often translated
  from English.
- **Mixed / bilingual page** → polish each language with its own engine; never let English
  edits leak into the German (or vice versa). Flag any inconsistency between the two
  versions.

If the brief or the user names a target locale (de-AT, de-CH), note that currency
placement, `ß`/`ss`, and quotation marks differ; flag it rather than silently applying
de-DE rules.

### 2. Decide refresh vs. rewrite — and say which, explicitly

State the decision before you touch a word. This single sentence prevents the two classic
failures: polishing copy that needed a rethink, or rewriting copy that only needed a trim.

- **Refresh** (the default): the structure and message are sound. Tighten clarity, voice,
  proof, specificity, and CTAs in place. Most "make this better" requests are refreshes.
- **Rewrite**: the copy targets the wrong reader, leads with the wrong message, or has no
  proof to build on. The structure is broken, not just the words. Only escalate to a
  rewrite when a refresh genuinely can't fix the underlying problem — and **flag it to the
  user first** rather than quietly replacing their page.

Write the verdict like: *"This is a refresh — the message is right, I'll tighten the hero
and add proof to the trust line"* or *"I'd recommend a rewrite here: the page is all about
you, not the reader, and there's no proof to build on. Want me to go ahead?"*

### 3. Read the brand brief if it exists

Look for a `brand-brief.md` in the project (voice adjectives and anti-adjectives, du/Sie,
glossary, banned words, proof points). If present, it **overrides** these defaults — match
its voice and respect its banned-words list and glossary. If absent, infer the voice from
the copy itself and from any 2–3 paragraphs of the author's writing the user supplies, and
proceed. **Never block on a missing brief.**

### 4. Run the passes, one focused sweep at a time

Make one pass per dimension rather than fixing everything at once — separating the passes
keeps each one sharp. The two engines map onto the same conversion goals:

| Goal | English (Seven Sweeps) | German (Lektorat) |
|---|---|---|
| Read it in one scan | Clarity, front-load | Satzlänge, kein Schachtelsatz, Aktiv |
| Sound like the brand | Voice & Tone | Register, kein Amtsdeutsch, du/Sie konsistent |
| Earn each claim | "So what?" + "Prove it" | Nutzen statt Floskel, prüfbare Fakten |
| Say something specific | Specificity | Floskeln/Worthülsen raus, Zahlen rein |
| Sound native | (n/a) | Calques & Denglisch raus (Verbalstil, Idiom) |
| Make the next step easy | Zero risk | starke CTA + Risiko-Reduzierer |

Full detail, examples, and the named anti-patterns live in the two reference files. Read
the one that matches the copy's language before editing.

### 5. Present the result so the author can accept or reject each change

Default output:

1. **The verdict** — refresh or rewrite, in one line.
2. **The polished copy** — clean, ready to paste.
3. **What changed and why** — a short list keyed to the passes (e.g., "Hero: cut
   'innovative, end-to-end' (filler) → led with the reader's outcome"). Keep the *why*
   tied to a pass or anti-pattern so the edit is defensible, not just an opinion.

Surface anything you deliberately **left alone** ("kept your headline — it already passes
the competitor test"), and flag claims you couldn't verify rather than inventing proof.
Never fabricate numbers, customer names, or certifications to fill a "Prove it" gap — mark
the gap and ask the author for the real figure.

## The one test that catches the most filler

Apply the **competitor copy-paste test** to every hero line, value prop, and trust
statement, in both languages: *could a competitor paste this exact sentence onto their own
site without it becoming false?* If yes, the line says nothing specific to you — replace it
with a number, a named capability, a mechanism, or a proof point. (German: *„Könnte ein
Mitbewerber den Satz 1:1 übernehmen?“* → ja = Floskel = streichen.)

## Examples

> Both examples are original and constructed (domain: brand protection); they are not
> copied from any live site.

### Example A — English refresh (hero + trust line)

**Input**
> "Our innovative, end-to-end platform empowers organizations to holistically safeguard
> their brand in today's fast-paced digital landscape. We are a trusted, reliable partner
> committed to delivering world-class security for businesses of all sizes."

**Verdict:** Refresh. The offer is sound; the copy is all filler and no proof.

**Output**
> "We find the fake websites, phishing pages, and impostor profiles abusing your brand —
> and get them taken down. GDPR-compliant, data hosted in Germany, incident response
> within 24 hours, 1,200+ brands protected."

**Why:** *Clarity/Voice* cut the AI-corporate tells ("innovative," "holistically," "in
today's fast-paced landscape," "world-class," "of all sizes"). *So what?/Specificity* led
with the reader's concrete outcome and named the threats. *Prove it* swapped "trusted,
reliable partner" — which any competitor could paste verbatim — for four checkable facts.
The author's plain, declarative rhythm is preserved.

### Example B — German Lektorat (translationese removed)

**Input**
> „Unsere innovative, ganzheitliche Plattform ermöglicht die Realisierung von umfassendem
> Markenschutz und macht am Ende des Tages den Unterschied.“

**Verdict:** Refresh (Lektorat). Aussage tragfähig; Text ist übersetzt und floskelhaft.

**Output**
> „Wir schützen Ihre Marke vor gefälschten Websites, Phishing und Fake-Profilen – und
> nehmen Betrugsseiten für Sie vom Netz.“

**Why:** *Verbalstil* statt Nominalstil („Realisierung“ → „schützen“, „nehmen … vom Netz“).
*Floskeln raus* („innovativ“, „ganzheitlich“). *Calque* „am Ende des Tages“ gestrichen;
„realisieren“ als Bedeutungslehnwort vermieden. Konkreter Nutzen statt Abstraktion,
Gedankenstrich „–“ mit Leerzeichen. Anrede konsequent Sie.

## What to preserve

- The author's **sentence rhythm and word choice** where they already work. If they write
  short and punchy, don't smooth it into corporate cadence.
- **A working headline.** If it passes the competitor test and matches the voice, leave it.
- **Person and register.** Don't flip du↔Sie or formal↔casual unless the brief or an
  inconsistency demands it; if you do change it, make it consistent everywhere and say so.

## Reference files

- `references/seven-sweeps-en.md` — the seven English editorial passes in depth, each with
  a before/after; the refresh-vs-rewrite decision; the named anti-patterns (Wall of
  Features, Corporate Speak, Buried CTA, No Proof, Me-First); the competitor copy-paste
  test. Read it before polishing English copy.
- `references/lektorat-de.md` — the German anti-translationese engine (in German, with a
  table of contents): the calque table (hard rules vs. contested style), the anglicism
  test + Scheinanglizismen, Verbalstil over Nominalstil, sentence-length / active-voice
  rules, and the Floskeln blacklist + trust vocabulary. Read it before polishing German copy.

Optional enrichment (not required; this skill works without them): `shared/references/
conversion-principles.md` for the language-neutral seven core principles, and the
`humanizer-en` / `humanizer-de` skills when the copy reads machine-generated.
