# Contributing to copycraft

Thanks for helping make copycraft better. The bar is simple: skills should be useful,
honest, idiomatic, and self-contained.

## Adding a skill

Each skill is a leaf folder under `skills/` so it works **both** as part of the plugin
and when copied out on its own:

```
skills/<kebab-case-name>/
├── SKILL.md            # frontmatter + instructions
└── references/         # heavy tables, progressively disclosed
    └── *.md
```

1. **Name** the folder in `kebab-case`. The folder name is the invocation name.
2. **Frontmatter** needs `name` (matching the folder) and `description`. Nothing else
   is required. Keep the description **under ~1,400 characters** (the hard cap is 1,536,
   including any `when_to_use`).
3. **Self-contained.** A user must be able to copy this one folder into
   `~/.claude/skills/` and have it work. Put everything the skill critically needs in its
   own `references/`. You may *mention* `shared/references/…` as enrichment, but the skill
   must not break without it.
4. **Body under ~500 lines.** Push long tables into `references/*.md`. For any reference
   file over ~300 lines, add a table of contents.

## The bilingual-description rule

Triggering happens in the orchestrator context, which may be operating in **either**
language. So every skill `description` must contain **both German and English trigger
phrases** — even for a German-bodied skill. The body can be monolingual; the description
is the bilingual doormat. Be a little "pushy": list concrete trigger phrases and contexts,
because Claude tends to *under*-trigger skills.

✗ "Improves German copy."
✓ "Rewrites German marketing copy to sound native and idiomatic, removing translationese
and Denglisch. Use whenever the user wants to polish, fix, lektorieren, or 'entkrampfen'
German copy, says it 'klingt übersetzt', or asks to turn English copy into natural German."

## The German-body rule

German flagship skills (`lokalisieren-de`, `texten-de`, `du-sie-check`, `typografie-de`,
`humanizer-de`) have their **SKILL.md body written in German**, opening with a German
role-anchor so the model stays in language context, e.g.:

> „Du bist eine erfahrene deutsche Werbetexterin. Du schreibst klar, idiomatisch und ohne
> Denglisch oder Floskeln. Du orientierst dich am Markenbrief (`brand-brief.md`) und an
> den Regeln in `references/`.“

## The cite-contestable-rules rule

Mark **hard rules** separately from **contested style**:

- **Hard rules** (errors): `in 2024` ✗, Deppenleerzeichen ✗, wrong quotation marks ✗,
  glued currency ✗. State them as rules.
- **Contested style** (smells, not errors): `Sinn machen`, `am Ende des Tages`,
  `nicht wirklich`. Downgrade them, don't forbid them — and note the disagreement
  (e.g., Eisenberg defends "Sinn machen"). Cite the source where a rule is contestable.

## Honesty & hygiene

- **No copyrighted copy.** Never commit scraped website text. Reference sites by URL;
  fetch or paraphrase at runtime. Examples in `examples/` must be **original and
  constructed**, and labeled as such.
- **No executable scripts.** copycraft is pure markdown. Don't add code to run.
- **Credit sources** in `SOURCES.md` and inside skill bodies where a rule is contestable.

## PR checklist

- [ ] Folder is `kebab-case`; `name` frontmatter matches the folder.
- [ ] `description` is bilingual (DE + EN trigger phrases) and under ~1,400 chars.
- [ ] German flagship skill? Body is in German with a role-anchor.
- [ ] Body under ~500 lines; long tables in `references/` (TOC if >300 lines).
- [ ] Skill is self-contained (copy-one-folder works).
- [ ] Hard rules vs. contested style are distinguished; contestable rules cited.
- [ ] No copyrighted copy; examples original and labeled.
- [ ] One concern per skill; no dead `references/`.
- [ ] Conventional commit message (`feat:`, `fix:`, `docs:`, `refactor:`, …).
- [ ] On release: bump `version` in `plugin.json`, `marketplace.json`, and `CHANGELOG.md`.
