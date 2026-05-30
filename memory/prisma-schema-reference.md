---
name: prisma-schema-reference
description: Always reference prisma/schema.prisma when working with database structure
metadata:
  type: project
---

The database schema is defined in `prisma/schema.prisma`. Reference it anytime you need to understand the structure of data stored in the database.

Current models:
- `User` — id (cuid), email (unique), password (hashed), timestamps, relation to projects
- `Project` — id (cuid), name, userId (optional, for anon projects), messages (JSON string, default `[]`), data (JSON string for VFS, default `{}`), timestamps, cascading delete from User

**Why:** Keeps DB work grounded in the actual schema rather than assumptions.

**How to apply:** Before writing any Prisma queries, server actions, or migrations, read `prisma/schema.prisma` first.
