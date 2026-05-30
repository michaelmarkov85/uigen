---
name: eslint-read-first
description: Read .eslintrc.json first before working on source files
metadata:
  type: feedback
---

Always read `.eslintrc.json` before starting work on source files so lint rules are understood upfront.

Current config: `{ "extends": "next" }` — uses the Next.js ESLint ruleset.

**Why:** Knowing the active lint rules prevents writing code that fails linting and avoids needing to fix it after the fact.

**How to apply:** When beginning any task that involves editing or creating source files, read `.eslintrc.json` first.
