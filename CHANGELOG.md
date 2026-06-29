# Changelog

All notable changes to **copycraft** are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

When you cut a release, bump the version in three places: `.claude-plugin/plugin.json`,
`.claude-plugin/marketplace.json`, and this file.

## [Unreleased]

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
