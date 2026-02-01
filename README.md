# JavaScript Minify / Format Tool

A single-page, mobile-friendly web tool for minifying and formatting JavaScript. It runs entirely in the browser using CDN-loaded dependencies (Terser for minification and Prettier for formatting) and includes a bookmarklet generator.

## Features

- **Minify** JavaScript with Terser (non-mangling settings by default).
- **Format** JavaScript with Prettier (Babel parser + Estree plugins).
- **Swap** input/output, **clear** both panels, and **copy/paste/select** helpers.
- **Bookmarklet** link generation from the output panel.
- **Light/Dark** theme toggle with persistent preference.
- **Mobile-friendly** UI with large tap targets.

## Project Structure

```
.
├── docs/
│   └── index.html   # The full HTML/CSS/JS implementation
└── README.md
```

## Usage

1. Open `docs/index.html` in a browser.
2. Paste JavaScript into the **Input** panel.
3. Click **Minify** to generate minified output.
4. Paste minified or bookmarklet code into **Output** and click **Format** to beautify into **Input**.
5. Drag the **bookmarklet** link to your bookmarks bar (or long-press on mobile) to save the generated snippet.

## Notes

- The tool relies on CDN scripts:
  - `terser` for minification
  - `prettier` + `plugins/babel` + `plugins/estree` for formatting
- Since everything runs client-side, no server setup is required.

## License

See [LICENSE](LICENSE).
