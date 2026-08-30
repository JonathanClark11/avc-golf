# STEERING.md — AVC.golf

Standing context and rules for Bucky when working on this project.

## What this is
Aaron Varlow Classic golf tournament website. Same pattern as boggs.golf. Domain avc.golf (pending confirmation). No paying users, for-fun.

## Stack
- Next.js 16, React 19, Tailwind v4, TypeScript
- Supabase for data (TBD — may not need a database initially)
- Deploy: Vercel, auto-deploy on push to `main`

## Risk gate — auto-merge OK
- Doc-only changes, copy/typo fixes, CSS-only changes (< 50 lines), test additions
- Version bumps in devDependencies that pass build + lint

## Risk gate — approval required
- Any change to `supabase/` schema/migrations
- Any change to `package.json` runtime dependencies
- Any change to `.env*`
- PRs > 200 lines net
- Removing/renaming exported functions or existing routes
