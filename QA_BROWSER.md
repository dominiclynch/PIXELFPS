# Browser QA Runbook

Use Chrome DevTools MCP for browser-first checks on PixelFPS.

## First smoke pack
- Homepage loads without console errors
- Auth flow works for login, logout, and bad-credential handling
- Stats and rankings pages render without failed XHR or blank states
- Lobby and matchmaking flows can enter, cancel, and recover cleanly

## What to capture every run
- one full-page screenshot per major route
- console errors and warnings
- failed network requests
- obvious layout breaks on desktop width and mobile width

## Pass criteria
- no uncaught console errors
- no 5xx requests on core routes
- no dead buttons on primary actions
- no blocking visual regressions on homepage, auth, stats, rankings, lobby

## Suggested execution order
1. Homepage
2. Auth
3. Stats
4. Rankings
5. Lobby
6. Matchmaking

## Notes
- keep this focused on user-visible breakage, not pixel-perfect polish
- attach screenshots and request failures to any bug report
