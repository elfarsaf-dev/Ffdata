# FF Cyberpunk Profile

A Free Fire player profile viewer with a cyberpunk/glassmorphism visual design.

## Overview

Single-page static HTML application. No build system or backend — everything is in `index.html`.

## Features

- Search Free Fire player profiles by UID
- Displays avatar, banner, level, rank points, guild info, pet, weapon showcase, and outfit
- Animated particle background
- Glassmorphism card UI with cyberpunk color scheme

## External APIs

- Player data: `https://ff.cocspedsafliz.workers.dev/uid?uid=<UID>`
- Asset lookup: `https://ff.cocspedsafliz.workers.dev/lookup?id=<ID>`

## Development

Served via Python's built-in HTTP server:

```
python3 -m http.server 5000
```

## Deployment

Configured as a static site deployment with `publicDir: "."`.

## Files

- `index.html` — entire application (HTML + CSS + JS inline)
- `ffdb.json` — local data file (Free Fire database)
- `rank_01.png` – `rank_37.png` — rank badge images
