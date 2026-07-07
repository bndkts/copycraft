# Changelog

All notable changes to **copycraft** are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

When you cut a release, bump the version in three places: `.claude-plugin/plugin.json`,
`.claude-plugin/marketplace.json`, and this file.

## [Unreleased]

### Added

- **Three new skills** (fifteen total): `email-copy` (marketing & lifecycle emails —
  subjects, preheaders, welcome/trial-end/win-back, newsletters, German legal basics),
  `ads-copy` (Google RSA / Meta / LinkedIn inside real character limits, message match,
  RSA combinability, German character economics), `microcopy-ux` (buttons, errors,
  empty states, forms, dialogs — the surfaces where du/Sie mixing actually creeps in).
- **Voice samples (Stimmproben)** in the brand brief: section 9 of the template plus a
  brand-voice interview step. Generation skills now match the samples' rhythm and word
  choice — samples beat adjectives.
- **Variants-then-judgment** in `texten-de` and `copywriting-en`: high-stakes units
  (hero, value props, primary CTA) are drafted 2–3 ways from distinct angles, judged
  against the checklist, delivered as winner + A/B runner-up.
- **Awareness stage** in `landing-page`: problem-/solution-/product-aware decides the
  section weights (mirrors `seo-copy`'s search-intent move).
- **Whole-page cohesion pass** in `landing-page`: varied section openings and shapes,
  no word echoes, heading-skim check — the page-level AI tell no sentence check catches.
- **Machine pre-scan** in `typografie-de`: eight tested grep patterns plus the
  U+201E/U+201C count check for the visually-invisible wrong closing quote.
- **Length limits** in `headlines-and-ctas`: buttons ≤ ~25 chars, mobile-wrap check,
  the 20–30% German-growth rule for localized mockups.
- `evals/test-briefs.md`: five fixed briefs + rubric to benchmark skill changes
  before/after instead of judging anecdotally.

### Changed

- **Brand-brief lookup standardized everywhere**: `.claude/brand-brief.md`, then
  project root — previously four different wordings meant a skill could silently miss
  the brief and drift off-voice.
- **Worked examples de-anchored from brand protection**: one example per skill moved to
  a new domain (salon booking, restaurant scheduling, Zeiterfassung, HR, email
  marketing, fitness, Steuer-App, team workspace) so the security-B2B register doesn't
  bleed into every output; `examples/before-after-{de,en}.md` gained second-domain
  sections; `reference-sites.md`'s brand-specific competitor section generalized.

## [0.1.0] - 2026-06-29

Initial release — a bilingual (English + German) copywriting toolkit for Claude.
Twelve self-contained skills, installable as one plugin or copied folder-by-folder.
Pure markdown: **no executable scripts**.

### Added

**Foundation**
- `brand-voice` — defines brand voice and creates/maintains the shared `brand-brief.md`
  (du/Sie decision, terminology glossary, banned-word list, proof points).

**Bilingual (auto-route by detected language)**
- `copy-polish` — improves existing copy without rewriting it (EN "Seven Sweeps";
  DE "Lektorat" anti-translationese pass).
- `headlines-and-ctas` — headline formulas and native CTAs per language.
- `landing-page` — full landing-page structure and section-by-section copy.
- `seo-copy` — search-intent-aligned copy, with German keyword/compound handling.

**English**
- `copywriting-en` — generate English conversion copy from scratch.
- `humanizer-en` — strip English AI-tells; voice-calibrate to the user's own writing.

**German (SKILL.md body authored in German)**
- `lokalisieren-de` — flagship: write native German from meaning, not word-for-word.
- `texten-de` — generate German conversion copy from scratch.
- `humanizer-de` — strip German AI-tells (natively built, not a translation of the EN list).
- `du-sie-check` — audit and enforce consistent du/Sie usage.
- `typografie-de` — fix German typography, numbers, dates, currency, and compounds.

**Shared & support**
- `shared/references/conversion-principles.md`, `shared/references/reference-sites.md`.
- `examples/before-after-en.md`, `examples/before-after-de.md` (original, constructed copy).
- README, CONTRIBUTING, SOURCES, LICENSE (MIT).

[Unreleased]: https://github.com/bndkts/copycraft/compare/v0.1.0...HEAD
[0.1.0]: https://github.com/bndkts/copycraft/releases/tag/v0.1.0
