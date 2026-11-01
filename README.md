# Garfield Flash Games

This repository hosts a small web app that lets you play a collection of classic Garfield-themed Flash games in the browser using the local [Ruffle](https://ruffle.rs/) Flash emulator.

The project is built as a static HTML app with no backend or package installation required.

## Features

- Run Garfield Flash games directly in the browser
- Local self-hosted Ruffle runtime (no CDN dependency)
- Game list with selectable titles
- Reload, fullscreen, and stop controls
- Works from a static file or local web server

## Included games

- Escape From Hotel Muncie
- Garfield's Scary Scavenger Hunt
- Garfield's Scary Scavenger Hunt 2
- Krazy Kennel Breakout
- Mystical Forest Adventure
- Punt the Pooch

## Project structure

- `index.html` — main app and game selector UI
- `garfield.svg` — site branding asset
- `LICENSE` — project license
- `ruffle-0.7.1-web-selfhosted/` — bundled Ruffle runtime
- `*/` — game folders containing SWF files and related assets

## Run locally

Because this is a static web app, the simplest option is to open `index.html` directly in a browser.

If you prefer to serve it locally:

```bash
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Notes

- This project relies on Flash emulation via Ruffle.
- Some browsers may restrict autoplay or media behavior depending on settings, but the app includes controls for reloading and playing the game.
- The app is designed to keep all game assets local to the repository.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Credits

- Flash game content and assets are preserved for archival/playback use.
- Ruffle is used to run legacy Flash content in modern browsers.
