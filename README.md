# README

[中文版本](README_CN.md)

## About

sveltekit wails template

use pnpm by default

## Live Development and Building

To run in live development mode, run `wails dev` in the project directory. In another terminal, go into the `frontend`
directory and run `pnpm run dev`. The frontend dev server will run on http://localhost:34115. Connect to this in your
browser and connect to your application.

To build a redistributable, production mode package, use `wails build`.

## Architecture

### About assets/static files

For images, fonts, and other assets, please put them in `src/assets` and use

```javascript
import logo from "path/to/logo.png
```

to import.

For static files (such as `manifest.json`, `favicon.ico`), which should have stable URLs and undergo no processing, put them in `static` directory (Maybe in desktop apps, this directory is used rarely?).

### Path alias

To use path alias, please edit them in `svelte.config.js`, there are already two pre-defined alias `@assets` and `@wailsjsMain`

