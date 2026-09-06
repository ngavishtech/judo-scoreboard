# Base44 Dev Environment

## Project
Static Judo scoreboard — pure HTML/CSS/JS, no build step, no backend, no database.
All app files live in `judoscoreboard/` with `index.html` as the entry point.

## Running
```
docker compose -f docker-compose.base44.yml up -d
```
Serves `judoscoreboard/` via nginx:alpine on host port 3000.

## Editing
Edits to files under `judoscoreboard/` are reflected immediately (bind-mounted, read-only to nginx).
Call `reload_preview` after changes to refresh the preview iframe.

## Secrets
None required — fully static, no external services.
