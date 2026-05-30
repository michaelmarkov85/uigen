---
name: timestamp-on-save
description: Add a timestamp comment at the end of every file when saving
metadata:
  type: feedback
---

When saving (writing or editing) any file, append a timestamp comment at the very end.

Use the appropriate comment syntax for the file type, e.g.:
- TypeScript/JavaScript/TSX/JSX: `// Last modified: 2026-05-24T14:32:00Z`
- CSS: `/* Last modified: 2026-05-24T14:32:00Z */`
- JSON/Prisma schema: not applicable (no comment syntax)

Timestamp must be in UTC (ISO 8601 format with `Z` suffix).

**Why:** User wants a visible record of when each file was last touched.

**How to apply:** After every Write or Edit, add a trailing timestamp comment in the correct syntax for that file type. Use today's date from [[current-date]].
