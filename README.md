# Nisith Akain Studio

A light, professional, 3D scroll-driven website for a web design studio. As you scroll, the camera flies through a scene of floating 3D shapes modelled in Blender, with blur-reveal text, scroll-velocity blur and skew, moving marquees and tilting glass cards.

**Live site:** https://nisith-akain.github.io/NisithAkain-Studio/

## Features

- Scroll-controlled 3D camera path built with Three.js
- Custom 3D models made in Blender (knot, icosphere, octahedron, ring, cube, cone, capsule), embedded in the page
- Animated split-text headlines that blur in, plus scroll-speed blur and skew
- Live GitHub projects section that pulls public repositories from [`Nisith-Akain`](https://github.com/Nisith-Akain), cached in the browser for 10 minutes, with a fallback if the API is unavailable
- Contact form that opens your email client addressed to h.a.dnisith@gmail.com
- Single-file site: everything lives in `index.html`

## Run locally

Open `index.html` in a modern browser. An internet connection is needed for Three.js (loaded from a CDN) and the GitHub API.

## Project structure

| Path | Purpose |
| --- | --- |
| `index.html` | The complete site (models embedded as base64) |
| `_build/index.src.html` | Editable source with a `__GLB_BASE64__` placeholder |
| `_build/models.glb` | Blender export of the 3D models |

To rebuild `index.html`, replace `__GLB_BASE64__` in `_build/index.src.html` with the base64 of `_build/models.glb`.

## Contact

- Email: h.a.dnisith@gmail.com
- GitHub: https://github.com/Nisith-Akain
