# PIXELFPS Platform

**Full-stack competitive FPS platform — auth, lobbies, matchmaking, rankings, and real-time analytics.**

PIXELFPS Platform is the web infrastructure layer for [PixelFPS](https://pixelfps.com) — a browser-based competitive first-person shooter. This repo handles everything outside the game engine: player identity, session management, leaderboards, and lobby coordination.

## Features

- **Auth** — Google OAuth via Supabase, session handling, player profiles
- **Lobby system** — create, join, and manage game lobbies pre-match
- **Matchmaking** — skill-based match pairing
- **Rankings** — global and regional leaderboards with stat tracking
- **Analytics** — real-time match data, kill/death ratios, win rates
- **Homepage** — public-facing site with player stats and game info

## Tech stack

| Layer | Tech |
|---|---|
| Auth | Google OAuth + Supabase Auth |
| Database | Supabase (Postgres) |
| Game engine | [pixelfps.com/game](https://game.pixelfps.com) |
| Deployment | GitHub Actions |

## Setup

```bash
cp .env.example .env
# Fill in Supabase URL, anon key, Google OAuth credentials
```

Required environment variables — see `.env.example` for full list:

```
GOOGLE_CLIENT_ID
GOOGLE_CLIENT_SECRET
SUPABASE_URL
SUPABASE_ANON_KEY
GAME_ENGINE_URL
```

## License

MIT
