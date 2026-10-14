# Canopy Atlas — A Living Field Guide

A minimal rainforest atlas in sage-green tones, with an open 3D stage, editorial species details, and interactive wildlife. The layout follows the Feather Atlas video reference supplied for this project.

**Live dashboard:** https://canopy-rainforest-matt.neuronsarealsocool.chatgpt.site

The live site is hosted with Sites. Its existing access settings are preserved during updates.

## Features

- Flying keel-billed toucan and scarlet macaw, plus tree frog and jaguar models built with Three.js.
- Layered flight feathers, procedural feather textures, gentle wing motion, and soft ground shadows.
- Drag to rotate, zoom, reset the view, toggle daylight/evening lighting, and pause animation.
- Automatic 360-degree rotation and an expanded stage view.
- Keyboard controls: arrow keys rotate; `+` and `-` zoom when the scene is focused.
- Close-up camera views, searchable species tabs, and group filters.
- Species traits and habitat details, with a collection saved in browser local storage.
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
- `dist/app.js`: scene, camera controls, species data, and atlas interactions.
- `dist/birds.js`: flying toucan and macaw models and procedural feather materials.
- `dist/forest-models.js`: tree frog and jaguar models.
- `dist/vendor/three.module.js`: vendored Three.js 0.169.0 (MIT license).
- `serve.cjs`: local static preview server.
- `.openai/hosting.json`: deployment configuration for the existing Sites project.

Serve `dist/` through any static web host to run the dashboard elsewhere. WebGL is required for the 3D scenes. Typography uses Google Fonts, with local font fallbacks. Animal models and notes are educational illustrations; the dashboard does not show live ecological measurements.

## Validation

JavaScript syntax was checked for all three application modules. Browser checks covered desktop and mobile layouts, 3D rendering, species search and filtering, saved collections, and close-up camera controls. The browser reported no console warnings or errors during these checks.

## Species references

- [BirdLife / IUCN keel-billed toucan assessment](https://doi.org/10.2305/IUCN.UK.2021-3.RLTS.T22682102A168670038.en)
- [San Diego Zoo Wildlife Alliance: macaws](https://animals.sandiegozoo.org/animals/macaw)

The models are original artistic interpretations, rather than scientific scans.
