# Space Invaders v2

Een retro Space Invaders-kloon, volledig gebouwd in één zelfstandig HTML-bestand met vanilla JavaScript en de HTML5 Canvas API — geen build-tools of dependencies nodig.

## Spelen

Open `index.html` direct in een browser, of serveer de map lokaal:

```bash
python3 -m http.server 8765
```

en ga naar `http://localhost:8765/index.html`.

## Besturing

**Desktop**
- `←` / `→` of `A` / `D` — bewegen
- `SPATIE` — schieten (en spel starten/herstarten)
- `P` — pauzeren

**Mobiel / touch**
- Op-scherm knoppen (◀ ▶ en SCHIETEN) verschijnen automatisch op touch-apparaten

## Features

- Vijf rijen aliens in drie types (elk met eigen puntenwaarde), die versnellen naarmate de vloot slinkt
- Verwoestbare bunkers met pixel-nauwkeurige schadeberekening
- Bonus-UFO die af en toe overvliegt voor extra punten
- Synthesizer-geluidseffecten via de Web Audio API (schieten, explosies, alien-stappen, UFO, overwinningsmelodie)
- Levels, levens, score en highscore (opgeslagen in `localStorage`)
- iOS-vriendelijke viewport-afhandeling (safe areas, geen pull-to-refresh/zoom)

## Techniek

- Geen frameworks: pure HTML/CSS/JS in één bestand
- Tailwind CSS via CDN voor styling
- "Press Start 2P" Google Font voor de retro arcade-look
- Alle graphics zijn handgetekende pixel-art sprites, gerenderd op een `<canvas>`
