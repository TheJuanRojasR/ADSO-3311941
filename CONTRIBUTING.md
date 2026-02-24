# Contributing

This repository stores my coursework, notes, practices, and evidence for the **ADSO – Software Analysis and Development** program, organized by **terms** and **competencies**.

Even if this is mostly a personal repository, I follow consistent rules to keep the history clean and easy to understand.

---

## Commit message convention (Conventional Commits)

All commits **must be written in English** and follow **Conventional Commits**:

```
type(scope): short summary
```

### Types (allowed)

Use one of these types:

- `docs` — notes, READMEs, guides, documentation
- `feat` — new code/functional work (exercises, project features)
- `fix` — bug fixes (code) or corrections (instructions)
- `refactor` — code changes that do not change behavior (cleanup)
- `style` — formatting only (lint/prettier, whitespace, naming) without logic changes
- `chore` — maintenance tasks (structure changes, renames, .gitignore updates)
- `test` — adding/updating tests
- `build` — build system or dependency changes
- `ci` — CI configuration changes (GitHub Actions, pipelines)

### Scope (recommended)

Scopes help locate changes quickly. Use short scopes like:

- `repo`, `structure`, `templates`
- `term1`, `term2`, `term3`, etc.
- a competency name in kebab-case, e.g. `databases`, `programming-fundamentals`

Examples of valid commit headers:

- `chore(structure): add term 1 folder template`
- `docs(term1): add week 2 notes about control flow`
- `feat(programming-fundamentals): add loops practice exercises`
- `fix(databases): correct INNER JOIN example query`
- `refactor(programming-fundamentals): simplify input validation`
- `style(repo): format markdown files`
- `test(programming-fundamentals): add unit tests for calculator`
- `build(project): update npm dependencies`
- `ci(repo): add basic lint workflow`

---

## Rules for good commits

### 1) Keep commits small and focused
Prefer multiple focused commits over one huge commit.

Good:
- `chore(structure): create term 1 and competency folders`
- `docs(term1): add notes for classes and objects`
- `feat(programming-fundamentals): add practice exercises for arrays`

Avoid (too broad):
- `feat(term1): add notes, evidence, restructure folders, and more`

### 2) Don’t mix refactors/renames with content changes
When moving/renaming folders, do that in a dedicated commit:

- `chore(structure): rename trimester folders to term folders`

Then add content in a new commit:

- `docs(term1): add notes about databases normalization`

This makes Git history cleaner and improves file rename tracking.

### 3) Use present tense, short summaries
Start with a verb: `add`, `update`, `remove`, `fix`, `refactor`.

Good:
- `docs(databases): add normalization cheat sheet`

Avoid:
- `docs(databases): added normalization cheat sheet`
- `docs(databases): normalization stuff`

---

## Suggested workflow (optional)

1. Make changes for a single topic/task.
2. Review with `git status` and `git diff`.
3. Commit with a clear message following the convention.
4. Push your changes.

Example:

```bash
git add .
git commit -m "docs(term1): add notes about Git basics"
git push
```

---