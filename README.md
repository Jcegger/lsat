# LSAT Study Tracker

A personal study tracker built for my 14-week LSAT prep leading up to the August 2026 exam. Live at [lsat.jayegger.com](https://lsat.jayegger.com).

## Features

- **Dashboard** — today's task pulled automatically from the study plan, score trajectory, day streak, and countdown to test day
- **Session logger** — mark each day complete, add notes, reverse-chronological feed
- **PT score tracker** — log all 6 practice tests with LR/RC miss breakdowns, score progression chart, trendline projection toward target, plateau detection
- **Miss pattern tracker** — log individual questions by type, surfaces top 3 weak areas automatically

## Stack

- Vanilla HTML/CSS/JS — no frameworks, no build step
- [Supabase](https://supabase.com) — Postgres backend for cross-device sync
- GitHub Pages — static hosting
- Custom domain via Cloudflare DNS

## How it works

All state is stored in a single Supabase row and synced on every change. localStorage serves as an offline cache. Opening the app on any device loads the latest state from the database.

## Study plan

14 weeks · May 1 – August 8, 2026 · 45–90 min/day · 6 practice tests

| Phase | Weeks | Focus |
|-------|-------|-------|
| 1 | 1–4 | RC foundation (PowerScore RC Bible) + LR rebuild + start The Loophole |
| 2 | 5–9 | Timed sections + full LR reintegration (Loophole method) |
| 3 | 10–13 | Full test simulation |
| 4 | 14 | Test week |

Target: **167** (Fordham Law Part-Time Evening median: 165)

## Materials

- **The Loophole** (Ellen Cassidy) — primary LR instruction, read sequentially starting May 9
- **PowerScore RC Bible** — RC foundation, Weeks 1–4
- **PowerScore LR Bible** — formal logic reference only (conditional logic depth)
- **7Sage** — PT drilling, RC passages, analytics
- See [LOOPHOLE_REFERENCE.md](LOOPHOLE_REFERENCE.md) for chapter → question type lookup
