# Canopy — Rainforest Observatory

A minimal rainforest dashboard in forest-green and sage tones, featuring interactive, stylized 3D wildlife.

**Live dashboard:** https://canopy-rainforest-matt.neuronsarealsocool.chatgpt.site

The live site is private and requires the owner's ChatGPT sign-in.

## Features

- Tree frog, keel-billed toucan, and jaguar scenes built with Three.js.
- Drag to rotate, zoom, reset the view, and pause animation.
- Keyboard controls: arrow keys rotate; `+` and `-` zoom when the scene is focused.
- Species detail panels and a collection saved in browser local storage.
- Interactive rainforest layers and ecosystem spotlights.
- Responsive layout and reduced-motion support.

## Run locally

Install Node.js, clone this repository, and run:

```sh
node serve.cjs
```

Open http://127.0.0.1:4173. No dependency installation or build step is needed.

## Source

- `dist/index.html`: dashboard structure.
- `dist/style.css`: styling and responsive layout.
- `dist/app.js`: animal models and dashboard interactions.
- `dist/vendor/three.module.js`: vendored Three.js 0.169.0 (MIT license).
- `serve.cjs`: local static preview server.
- `.openai/hosting.json`: deployment configuration for the existing private Sites project.

Serve `dist/` through any static web host to run the dashboard elsewhere. WebGL is required for the 3D scenes. Typography uses Google Fonts, with local font fallbacks. Animal models and notes are educational illustrations; the dashboard does not show live ecological measurements.

## Validation

JavaScript syntax was checked with `node --check dist/app.js`. Browser checks covered 3D rendering, species switching, collection filtering, detail panels, and camera controls.
