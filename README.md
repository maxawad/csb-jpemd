# csb-jpemd

A one-page greeting site for a family video call. It shows a heading, "Hola Familia Rovalino Guevara", and a line in Spanish saying "Let's host a call with as many people as possible :)". It was made as a quick CodeSandbox project and deployed to GitHub Pages.

## What it does

- Displays a centered greeting on a bright green background.
- Loads the Noto Sans font from Google Fonts.
- Has no backend, no login, no forms and no API calls.

## Tech stack

- React 17 (bundled with Create React App, as exported from CodeSandbox)
- Plain CSS

## Repository layout

The `gh-pages` branch holds only the compiled build, not the source:

- `index.html`: the page entry point
- `static/js/`: the compiled JavaScript bundles (plus source maps)
- `static/css/`: the compiled stylesheet
- `asset-manifest.json`: list of build files produced by Create React App

The original source was two small files, `App.js` and `index.js`. The `App` component just renders the heading and subheading shown above. They can be read inside `static/js/main.377a2671.chunk.js.map`.

## Try it

Live demo: <https://maxawad.github.io/csb-jpemd/>

The asset links in `index.html` are absolute URLs that point to the `maxawad.github.io/csb-jpemd` address. This means the page loads its files from the live site even when you open it locally. To run it fully from a local copy, you would need to rewrite those URLs to relative paths (for example `./static/js/...`) and then serve the folder:

```bash
python3 -m http.server 8000
# open http://localhost:8000/
```

## Status

Working. It is a tiny static page and needs no API keys.

## Credits

Created with [CodeSandbox](https://codesandbox.io/) and Create React App. No license file is included.
