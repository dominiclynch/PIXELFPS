# PIXELFPS

PIXELFPS is the platform repo for the PixelFPS competitive FPS stack.
It covers the web product surfaces around the game: homepage, auth, stats, rankings, lobby, and matchmaking.

## Current Scope

- marketing and entry surface
- account and login flow
- player stats and rankings
- lobby state and matchmaking entry
- browser QA runbooks for core routes

## Stack

- Google OAuth
- Supabase
- external game engine endpoint via `GAME_ENGINE_URL`
- GitHub Actions deploy path

See `.env.example` for required configuration.

## Features

- homepage and entry surface
- account and login flow
- player stats and rankings
- lobby coordination
- matchmaking entry
- browser QA baseline for core routes

## QA

Browser smoke testing lives in [QA_BROWSER.md](./QA_BROWSER.md).
Use Chrome DevTools MCP for route, console, and network verification.

## Current State

This repo is currently lightweight and documentation-led.
The main public value right now is the platform scope, environment contract, and QA baseline for future implementation passes.
