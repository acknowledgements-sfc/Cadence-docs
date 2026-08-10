> For Mintlify product knowledge (components, configuration, writing standards),
> install the Mintlify skill: `npx skills add https://mintlify.com/docs`

# Cadence documentation (Mintlify)

Public docs for Cadence. Live URL: `https://cadencemgmt.site/docs` (proxied through the front-door Vercel project).

## About this project

- Built on [Mintlify](https://mintlify.com)
- Pages are MDX with YAML frontmatter
- Site config: `docs.json` in this directory
- Content root for Git deploy: repo subdirectory `mintlify/`
- Internal build logs and dispatches stay in the app repo `docs/` folder — do not migrate those here

## Terminology (locked)

Use Cadence vocabulary only. Do not invent synonyms.

- **Pursuit** — not "project"
- **Effort** — not "task" (in user-facing copy)
- **Exploration** — loop-shaped, no terminus; informs pursuits
- **Handled** — completion state language
- **"How do you want to move?"** — canonical prompt phrasing
- **quiet season** — lull / downtime period
- **four-beat sensation pattern** — health / status rhythm

No exclamation points. No first-person system voice ("I").

## Style preferences

- Active voice, second person ("you")
- One idea per sentence
- Sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references
- Iris (`#7c6cfc`) is the only saturated accent — already set in `docs.json`

## Content boundaries

Document: product concepts, guides, and public API reference as they land.

Do not document: admin-only tooling, Clerk/Supabase ops runbooks, fixture accounts, or unclosed design debates from Claude digests.

## Local preview

```bash
npm run docs:dev
# or: cd mintlify && mint dev
```

Validate: `npm run docs:validate`
