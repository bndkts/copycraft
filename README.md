# copycraft

**A bilingual (English + German) copywriting toolkit for Claude.** Brand voice,
conversion copy, editing, headlines & CTAs, landing pages, SEO, de-AI humanizing — and
the thing the off-the-shelf ecosystem is missing: **native German marketing copy that
doesn't read translated.**

The German flagship skills are authored *in German*, so Claude stays in the right
language context instead of translating English sentence-by-sentence. They encode the
craft that kills "translationese": calqued idioms, Denglisch, Floskeln, du/Sie
consistency, and German typography.

> **No executable scripts.** copycraft is pure markdown — skills are instructions, not
> code. There is nothing to run and nothing that runs itself. As with any plugin, you
> should still review what you install; here that means reading the markdown, which is
> the whole point of the format.

---

## What's inside

Fifteen self-contained skills:

| Skill | Lang | What it does |
|---|---|---|
| `brand-voice` | neutral | Define your brand voice; create & maintain the shared `brand-brief.md` (du/Sie, glossary, proof points, banned words, voice samples). |
| `copy-polish` | EN + DE | Improve existing copy without rewriting it. Detects language: EN "Seven Sweeps"; DE anti-translationese "Lektorat". |
| `copywriting-en` | EN | Generate English conversion copy from scratch. |
| `texten-de` | DE | Generate German conversion copy from scratch (German Werbetexter voice). |
| `lokalisieren-de` | DE | **Flagship.** Turn English copy (or a brief) into *native* German written from meaning. |
| `du-sie-check` | DE | Audit and enforce consistent du/Sie usage. |
| `typografie-de` | DE | Fix German typography, numbers, dates, currency, compounds. |
| `headlines-and-ctas` | EN + DE | Headline formulas and native CTAs per language. |
| `humanizer-en` | EN | Strip English AI-tells; voice-calibrate to your own writing. |
| `humanizer-de` | DE | Strip German AI-tells (built natively, not translated from the EN list). |
| `landing-page` | EN + DE | Full landing-page structure and section-by-section copy. |
| `seo-copy` | EN + DE | Search-intent-aligned copy, with German keyword/compound handling. |
| `email-copy` | EN + DE | Marketing & lifecycle emails: subjects, preheaders, welcome/trial-end/win-back sequences, newsletters. |
| `ads-copy` | EN + DE | Paid ad copy inside real character limits: Google RSA, Meta, LinkedIn — with message match to the landing page. |
| `microcopy-ux` | EN + DE | Interface strings: buttons, errors, empty states, forms, dialogs — where du/Sie mixing actually creeps in. |

All skills read one shared, user-maintained `brand-brief.md` so they stay consistent and
never re-ask the basics. The `brand-voice` skill creates it; the rest read it.

---

## Install

**As a plugin (recommended):**

```
/plugin marketplace add bndkts/copycraft
/plugin install copycraft@copycraft
```

The first command registers this repo as a marketplace; the second installs the plugin.
All fifteen skills become available and auto-invoke when relevant.

**A single skill (copy one folder):**

Every skill is a self-contained folder. To use just one — say the German localizer —
copy it into your skills directory:

```
# personal (all projects)
cp -r skills/lokalisieren-de ~/.claude/skills/

# or project-scoped
cp -r skills/lokalisieren-de <your-project>/.claude/skills/
```

It works immediately, no plugin install required.

**Local testing (from a clone):**

```
/plugin marketplace add .
/plugin install copycraft@copycraft
```

---

## Quickstart (3 steps)

1. **Install** (above).
2. **Create your brand brief.** Ask Claude: *"Use brand-voice to set up my brand brief."*
   It walks you through positioning, audience, voice, your du/Sie decision, proof points,
   a terminology glossary, and 3–5 approved voice samples (the strongest voice control),
   then writes `.claude/brand-brief.md` in your project.
3. **Polish a page.** Paste a hero or landing section and ask: *"Polish this"* (or, in
   German, *"Mach diesen Text besser"* / *"Das klingt übersetzt — bitte idiomatisch"*).
   `copy-polish` detects the language and applies the right editorial passes.

To bring English copy into German, ask: *"Localize this into German"* — `lokalisieren-de`
writes native German from the meaning, not word-for-word.

---

## Language support

English and German are both first-class. The German flagship skills
(`lokalisieren-de`, `texten-de`, `du-sie-check`, `typografie-de`, `humanizer-de`) have
their instruction bodies written in German. Every skill's *trigger description* is
bilingual, so the skills fire whether you're working in English or German. Target dialect
is **de-DE** (Germany); Austria/Switzerland differ in currency placement and quotation
marks — add a variant if you need one.

---

## Trust & safety

- **MIT licensed.** Example copy in `examples/` is original and constructed, not scraped.
- **No code execution.** Pure-markdown skills; nothing runs.
- **No copyrighted copy committed.** Reference sites are listed by URL for runtime study,
  never reproduced. See `shared/references/reference-sites.md`.
- Sources and attributions: [SOURCES.md](SOURCES.md). License: [LICENSE](LICENSE).

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) — how to add a skill, the bilingual-description and
German-body rules, and the PR checklist.
