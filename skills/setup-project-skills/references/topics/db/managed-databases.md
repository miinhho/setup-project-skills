# Managed databases and ORMs

| Skill | Install source | Use when |
| --- | --- | --- |
| `prisma-patterns` | `affaan-m/ECC` | Prisma schema, query, pagination, transaction, and migration safety patterns recur in TypeScript backends. |
| `prisma-client-api` | `prisma/skills` | Prisma Client filters, CRUD methods, or transactions need exact API guidance. |
| `prisma-cli` | `prisma/skills` | Prisma generate, migrate, db, validate, format, Studio, or MCP commands recur. |
| `prisma-database-setup` | `prisma/skills` | Prisma must be connected to PostgreSQL, MySQL, SQLite, or MongoDB. |
| `prisma-upgrade-v7` | `prisma/skills` | An existing Prisma 6 project is upgrading to Prisma 7. |
| `prisma-mongodb-upgrade` | `prisma/skills` | A Prisma MongoDB project needs an upgrade-path decision. |
| `prisma-postgres` | `prisma/skills` | Prisma Postgres provisioning, Console, Management API, or operations recur. |
| `prisma-driver-adapter-implementation` | `prisma/skills` | Work occurs inside a Prisma 7 SQL driver adapter or its transaction and error mapping. |
| `drizzle-orm-patterns` | `giuseppe-trisciuoglio/developer-kit` | Cross-dialect Drizzle schemas, queries, relations, transactions, or migrations recur. |
| `drizzle-nextjs-postgres` | `pproenca/dot-skills` | Drizzle with PostgreSQL runs inside a Next.js App Router service. |
| `drizzle-sqlite` | `pproenca/dot-skills` | Drizzle targets better-sqlite3, libSQL/Turso, Bun SQLite, D1, Expo SQLite, or op-sqlite. |
| `drizzle-sqlite-scaffold` | `pproenca/dot-skills` | A new Drizzle and SQLite setup needs config, client, schema, migrations, and repository scaffolding. |
| `neon-postgres` | `neondatabase/agent-skills` | Neon connection, pooling, branching, autoscaling, restore, replication, or search work recurs. |
| `neon-postgres-branches` | `neondatabase/agent-skills` | Branch-per-PR, schema-only branches, migration tests, or branch expiry recur. |
| `neon-postgres-egress-optimizer` | `neondatabase/agent-skills` | Query overfetching or database network cost needs diagnosis. |
| `neon-functions` | `neondatabase/agent-skills` | Long-running Node.js HTTP, WebSocket, SSE, webhook, bot, or MCP functions deploy next to Neon data. |
| `neon-object-storage` | `neondatabase/agent-skills` | S3-compatible object storage must branch with Neon database state. |
| `neon-ai-gateway` | `neondatabase/agent-skills` | A Neon project routes model calls through its AI Gateway. |
| `supabase` | `supabase/agent-skills` | Supabase Auth, Database, Storage, Realtime, Edge Functions, logs, or CLI work recurs. |
| `firebase-basics` | `firebase/agent-skills` | Firebase project configuration recurs across products. |
| `firebase-auth-basics` | `firebase/agent-skills` | Firebase sign-in, user management, or auth-backed access rules recur. |
| `firebase-firestore` | `firebase/agent-skills` | Firestore schemas, indexes, rules, or queries recur. |
| `firebase-data-connect` | `firebase/agent-skills` | Firebase Data Connect uses PostgreSQL schemas, authorized operations, or generated SDKs. |
| `firebase-hosting-basics` | `firebase/agent-skills` | Static sites, SPAs, redirects, headers, domains, or preview channels use Firebase Hosting. |
| `firebase-app-hosting-basics` | `firebase/agent-skills` | Next.js or Angular SSR deploys through Firebase App Hosting. |
| `firebase-crashlytics` | `firebase/agent-skills` | Firebase Crashlytics provisioning or SDK integration recurs. |
| `firebase-remote-config-basics` | `firebase/agent-skills` | Firebase Remote Config templates, flags, defaults, fetch, or listeners recur. |
| `firebase-ai-logic-basics` | `firebase/agent-skills` | A web app integrates Gemini through Firebase AI Logic. |
| `firestore-rules-creation` | `firebase/agent-skills` | Firestore security rules need implementation. |
| `firebase-security-rules-auditor` | `firebase/agent-skills` | Existing Firestore or Storage rules need a security review. |

Choose the broad provider skill only when the project repeatedly spans several provider products. Prefer the focused sibling for a recurring narrow task.
