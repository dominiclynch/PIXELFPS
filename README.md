# PIXELFPS

**Competitive FPS platform — homepage, auth, stats, rankings, lobby, and matchmaking.**

PIXELFPS is the web product and player platform for the broader PixelFPS stack.
It handles everything around the game client itself: player identity, progression surfaces, rankings, lobby coordination, and the browser paths that sit in front of match execution.

## Scope

- Homepage and entry surface
- Google login and player identity
- Stats and rankings
- Lobby creation and pre-match coordination
- Matchmaking entry
- Browser QA baselines for the core user paths

## Tech stack

| Layer | Tech |
|---|---|
| Auth | Google OAuth + Supabase Auth |
| Database | Supabase |
| Game handoff | [pixelfps.com/game](https://game.pixelfps.com) |
| Delivery | GitHub Pages + GitHub Actions |

## Environment

Copy `.env.example` to `.env` and provide:

```bash
GOOGLE_CLIENT_ID=
GOOGLE_CLIENT_SECRET=
SUPABASE_URL=
SUPABASE_ANON_KEY=
GAME_ENGINE_URL=
```

## QA

Use the browser smoke pack in [QA_BROWSER.md](./QA_BROWSER.md) for homepage, auth, stats, rankings, lobby, and matchmaking verification.

## Current State

This repo is currently infrastructure-led.
The live value today is the platform contract, environment shape, and QA path for the next implementation pass.

## License

[FSL-1.1-MIT](./LICENSE) — Functional Source License.

Free to use for personal projects, indie development, hobbyist use, and non-commercial purposes. Converts to MIT on 28 April 2028. Commercial use that competes with PixelFPS is not permitted.
