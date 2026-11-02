# Scorecard

An applicant tracking system for recruiters and hiring teams.

## Features

- Hiring pipeline board with configurable stages
- Resume upload and parsing into candidate profiles
- Candidate sourcing with plain-language search and filters (job title, industry, years of experience)
- Job creation, including from an uploaded job description
- Interview scheduling, calendar and queue, with suggested questions and interview scorecards
- Client management and emailed client reports
- Email and password sign-in, with a credit balance per user

## Tech stack

React 18, TypeScript, Vite, Tailwind CSS, shadcn/ui, TanStack Query,
Supabase (Postgres, Auth, Edge Functions), Resend, DeepSeek API

## Getting started

```bash
npm install
npm run dev
```

The app runs at http://localhost:8080.

The Supabase Edge Functions need `DEEPSEEK_API_KEY` and `RESEND_API_KEY` set as Supabase secrets.

## Project structure

```
src/
  components/      UI components and feature views
  hooks/           React hooks
  integrations/    Supabase client and generated types
  pages/           Routes
supabase/
  functions/       Edge Functions (resume parsing, client reports)
  migrations/      Database schema
```
