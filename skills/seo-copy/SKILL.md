---
name: seo-copy
description: 'Writes search-intent-aligned copy that ranks and reads well: keyword-aware H1/H2 structure, meta titles and descriptions, front-loaded answers — in English or German, with German compound/keyword handling. Use for SEO pages, blog intros, category/landing copy, or meta tags. Trigger: "SEO copy", "optimize for search", "meta description", "keyword", "rank for"; German: "SEO-Text", "für Suche optimieren", "Meta-Beschreibung", "Keyword", "Suchintention". Balances keywords with idiomatic copy; never sacrifices natural German to force a keyword.'
---

# seo-copy — Search-intent copy in English or German

You write copy that ranks **and** reads like a person wrote it. Search engines reward
pages that answer the searcher's actual question fast; readers reward pages that sound
human. Those goals agree more than SEO folklore suggests, so you never trade one for the
other. You write for the human and structure for the scanner — and for German, you handle
compound keywords and umlaut variants without ever bending the sentence out of natural
shape.

Use this skill for SEO landing/category pages, blog intros, and meta tags (title +
description) in either language. To generate non-SEO copy use `copywriting-en` or
`texten-de`; to polish existing copy use `copy-polish`.

## The one rule that orders everything else

**Search intent comes first; the keyword is downstream of it.** A keyword is just the
words a person typed to express a need. If you nail the need — and structure the page so a
scanner sees the answer in the first screen — the keyword falls into place naturally. Copy
that stuffs keywords but ignores intent ranks worse *and* converts worse, because both
Google and the reader can tell it dodged the question.

So before writing, name the intent (see `references/seo-bilingual.md` for the full map):

- **Informational** — "how does X work", "what is X". The reader wants an answer, not a
  pitch. Front-load a direct answer in the first 1–2 sentences, then expand.
- **Commercial** — "best X", "X vs Y", "X software". The reader is comparing. Lead with
  the differentiator and proof, not a definition.
- **Transactional** — "buy X", "X pricing", "book X demo". The reader is ready. Reduce
  friction; put the action and the risk-reducer up high.

Match the page type to the intent. A definition essay on a transactional query loses the
reader; a hard pitch on an informational query loses the ranking.

## Before you write

### Read the brand brief if it exists
Look for `.claude/brand-brief.md` first, then `brand-brief.md` in the project root. If
present, obey its voice, audience, **du/Sie** (German), glossary, banned words, and —
where it has them — its voice samples (match their rhythm and word choice) — they win
over any default here. A keyword never overrides a banned word or the brand's chosen term: if
the brief says the product is „Markenschutz-Plattform“, do not switch to a higher-volume
synonym in the H1 just because a tool reports more searches. **Never require the brief to
exist**; if there's none, proceed and ask only for the genuine gaps.

### Establish three things, then write
1. **Language and (for German) du or Sie** — this fixes every CTA and verb form.
2. **The primary keyword + 2–4 semantic variants** — the phrase the reader searches and
   its natural relatives, not a list to cram. If the user hasn't given one, ask, or infer
   it from the topic and say which phrase you targeted.
3. **The intent** (above) — it decides structure and tone.

Don't have keyword-research tools? That's fine — this skill is about *writing* for a
keyword and intent, not about volume data. Work from the phrase the user gives you.

## English on-page structure (essentials)

Full placement rules and the meta-length table live in `references/seo-bilingual.md` —
**read it before writing meta tags or your first H1.** The essentials:

- **H1** contains the primary keyword, read naturally, and makes one promise. One H1 per
  page.
- **First 100 words** include the primary keyword once and, for informational intent, the
  direct answer. Front-loading helps the scanner and the snippet alike.
- **H2s** carry semantic variants and the questions a reader actually asks — not the same
  keyword repeated. Subheads should read as a meaningful outline on their own.
- **Semantic variants over repetition.** Modern search rewards covering the topic, not
  hitting an exact phrase n times. Keyword stuffing reads badly to humans, which is the
  better reason to avoid it.
- **Meta title ≤ ~60 characters**, primary keyword near the front, one benefit or hook.
- **Meta description ≤ ~155 characters**: a benefit plus a CTA. It rarely changes rankings
  but heavily affects whether anyone clicks, so write it like ad copy, not a summary.

## German specifics (the part most tools get wrong)

German SEO is not English SEO with translated words. Read the German section of
`references/seo-bilingual.md` for the detail; the load-bearing points:

- **Compound vs. split keywords.** German users search both the closed compound and the
  split phrase: *Markenschutz* and *Schutz der Marke*, *Phishing-Schutz* and *Schutz vor
  Phishing*. Cover the natural variants across H1/H2/body instead of forcing one form
  everywhere. The closed compound usually belongs in the H1 because that's the primary
  term; the split form fits naturally in body sentences.
- **Umlaut variants.** Some users type `ä/ö/ü`, others type `ae/oe/ue` (and URLs/slugs
  often use the latter). Use correct umlauts in visible copy; cover the `ae/oe/ue` spelling
  in the slug or where users genuinely type it — never misspell the on-page word to chase
  it. Example: write „Markenüberwachung“, and let the slug carry `markenueberwachung`.
- **Native CTAs, never translated.** „Jetzt testen“, „Demo vereinbaren“, „Mehr erfahren“ —
  not a rendered „Bekomme gestartet“. A meta description CTA must read native too.
- **Respect typography in meta.** German quotation marks `„…“`, percent with a space
  („20 %“), currency after the amount („1.999,00 €“), no „in 2024“, no Deppenleerzeichen.
  Meta tags are copy, so the same mechanics apply.
- **Never sacrifice idiomatic German to force a keyword.** This is the skill's hard line.
  If the natural sentence and the exact-match phrase fight, the natural sentence wins and
  you place the keyword elsewhere (H2, body, alt text). A clumsy „SEO-optimierte
  Markenschutz Software Lösung“ (with a Deppenleerzeichen, no less) ranks no better and
  reads worse than „Software, die Ihre Marke vor Fälschungen schützt“.

## Worked examples

### Example 1 — English, commercial intent (category page)
**Input:** "SEO copy for our brand-protection product page. Primary keyword: *brand
protection software*. Audience: e-commerce security leads comparing vendors. Proof: 1,200+
brands, confirmed takedowns, response within 24h."

**Output:**
> **Intent:** commercial (the reader is comparing tools) → lead with the differentiator
> and proof, not a definition.
>
> **H1:** Brand Protection Software That Takes Fakes Down — Not Just Flags Them
> **First line (keyword + differentiator in the first 100 words):** "Brand protection
> software should do more than alert you. We find the fake shops and phishing pages abusing
> your brand and confirm each takedown — 1,200+ brands protected, response within 24 hours."
> **H2s (variants + real questions):** "How brand monitoring works" · "Detection vs.
> confirmed takedown" · "What you get in the first 24 hours"
> **Meta title (53 chars):** Brand Protection Software | Take Down Fake Sites Fast
> **Meta description (138 chars):** Find the fake shops and phishing pages abusing your
> brand — and get them taken down, confirmed not just flagged. 1,200+ brands. Scan free.
> **Primary CTA:** Scan my brand now · *No credit card.*

Why: the keyword sits in the H1 and first sentence without stuffing; H2s use variants and
buyer questions; the meta description is benefit + proof + CTA, within length; commercial
intent is served by leading with the differentiator.

### Example 2 — German, informational intent (du)
**Input:** „SEO-Text für eine Ratgeber-Seite. Keyword: *Zeiterfassung*. Suchintention:
Wie funktioniert digitale Zeiterfassung? Anrede: du. Produkt: Zeiterfassungs-App für
kleine Teams.“

**Output:**
> **Intent:** informational → die Frage zuerst direkt beantworten, dann vertiefen. Kein
> Pitch oben.
>
> **H1:** Digitale Zeiterfassung: So erfasst dein Team Arbeitszeiten ohne Zettel
> **Erste Zeile (Antwort zuerst, Keyword im ersten Satz):** „Digitale Zeiterfassung
> heißt: Dein Team stempelt per App oder Browser ein, und die Arbeitszeiten landen
> automatisch in einer Übersicht – ohne Excel-Liste und Stundenzettel.“
> **H2s (Compound- + Split-Varianten, echte Fragen):** „Arbeitszeiten erfassen: Was ist
> Pflicht?“ · „Stempeluhr oder App – was passt zu deinem Team?“ · „Was kostet eine
> Zeiterfassungs-App?“
> **Meta-Title (49 Zeichen + Marke):** Zeiterfassung: Arbeitszeiten digital erfassen |
> [Produkt]
> **Meta-Description (139 Zeichen):** Wie digitale Zeiterfassung funktioniert, was sie
> kostet und wann sie Pflicht ist – einfach erklärt. So wird dein Team die Zettel los.
> **CTA:** Mehr erfahren

Warum: Die informationale Frage wird in der ersten Zeile beantwortet (gut für Snippet und
Leser). Das Compound *Zeiterfassung* steht in H1 und erstem Satz; die Split-Form
*Arbeitszeiten erfassen* und das Compound *Zeiterfassungs-App* leben in den H2 – keine
erzwungene Wiederholung. Typografie (`„…“`, Halbgeviert mit Leerzeichen, Durchkopplung
„Zeiterfassungs-App“) stimmt; die Anrede bleibt durchgehend du.

## Hard rules vs. contested style

Treat these as two different things — fix the first, only nudge the second.

**Hard rules (genuine errors — fix every time):**
- **Never fabricate proof or stats** to fill a meta description or intro. Use a bracketed
  placeholder (`[N] brands`) so the user drops in the real figure. Fabricated trust
  destroys the thing SEO copy exists to earn.
- **German typography in all copy, meta included:** quotation marks `„…“` or `»…«`, never
  straight `"…"` or English `"…"` (Duden/DIN 5008); no „in 2024“ → „2024“/„im Jahr 2024“;
  no Deppenleerzeichen in compounds („Markenschutz Software“ ✗ → „Markenschutz-Software“ or
  „Markenschutzsoftware“ ✓); currency after the amount with a space („1.999,00 €“, not
  „€1,999.00“); percent with a space („20 %“).
- **One H1 per page.** Multiple H1s confuse the document outline.
- **Don't exceed the meta limits as if they were soft** — a title cut mid-word in the SERP
  reads broken. Treat ~60 / ~155 characters as real ceilings (full table in the reference).
- **Don't keyword-stuff.** Repeating the exact phrase to hit a density target is an
  outdated tactic that reads like a robot wrote it.

**Contested style (smells to downgrade, never forbid — the user may want them, and
authorities disagree):**
- „Sinn machen“ — Duden marks it colloquial, but linguist **Peter Eisenberg** argues it is
  well-formed German. Prefer „ergibt Sinn“ in polished body copy; do not treat it as an
  error.
- „am Ende des Tages“, „nicht wirklich“, „einmal mehr“ — calqued idioms that read
  translated; offer a crisper native phrase, but they're style, not mistakes.
- Floskeln in SEO intros (innovativ, ganzheitlich, maßgeschneidert, „führender Partner“) —
  flag and replace with a concrete fact; the competitor copy-paste test catches them. A
  quality nudge, not a hard rule.

When you change something contestable, say why in one clause; don't lecture.

## Quality checklist
- [ ] Intent named (informational / commercial / transactional) and structure matches it.
- [ ] Primary keyword in H1 and the first 100 words, read naturally — no stuffing.
- [ ] H2s carry semantic variants and real reader questions, not the repeated keyword.
- [ ] Answer front-loaded (first 1–2 sentences for informational intent).
- [ ] Meta title ≤ ~60 chars, keyword near the front; meta description ≤ ~155 chars with
      benefit + native CTA.
- [ ] German: compound **and** split variants covered naturally; umlauts correct in copy,
      `ae/oe/ue` only where users type it (e.g. the slug); CTAs native; typography correct.
- [ ] No idiomatic German bent to force a keyword.
- [ ] Every claim has real proof or a bracketed placeholder — nothing fabricated.
- [ ] du/Sie consistent with the brief across the whole page.

## Reference files (read on demand)
- `references/seo-bilingual.md` — **read before writing meta tags or your first H1.**
  Self-contained: the full search-intent map, English on-page keyword-placement rules, the
  meta title/description length table, and the German specifics (compound vs. split,
  umlaut `ae/oe/ue` variants, native CTAs, typography in meta, the never-force-a-keyword
  rule). The skill works with this file alone.
- Optional enrichment (only if the full plugin is present; the skill works without these):
  `shared/references/conversion-principles.md` (language-neutral principles, incl. the
  competitor copy-paste test), the `headlines-and-ctas` skill (native CTA map and German
  verb pairs), and `typografie-de` (full German typography rules).
