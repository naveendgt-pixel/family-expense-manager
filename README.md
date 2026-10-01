# Family Expense Manager

Mobile-first foundation for a private family finance application shared by the Owner and Wife.

## Local setup

1. Copy `.env.local.example` to `.env.local` and add a Supabase project URL and anonymous key when Supabase is ready to be connected.
2. Run `npm install`.
3. Run `npm run dev`.

Authentication screens are not connected yet; the database references Supabase Auth users without creating accounts or passwords.

## Database

Versioned PostgreSQL migrations are in `supabase/migrations`. They create the family finance tables, constraints, indexes, RLS policies, default categories, payment methods, and the `My Family` seed. No authentication users or financial transactions are seeded. See `supabase/README.md` for migration and initial-membership instructions.

## Commands

- `npm run dev` — start the local development server
- `npm run db:check` — parse migrations and verify the database contract
- `npm run lint` — run ESLint
- `npm run typecheck` — run TypeScript checks
- `npm run build` — create a production build
