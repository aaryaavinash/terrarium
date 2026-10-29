<p align="center"><img src="docs/banner.svg" alt="Bell & Moss themed project banner" width="100%"></p>

# Bell & Moss

*A whole climate under glass*

An imagined London workshop for sealed, hand-blown terrariums. Each glass bell holds a small climate that makes its own rain and asks to be observed over years.

The planned project address is `https://terrarium.aarya.cyou/`. The site is an interactive concept; its booking, purchase, or application invitations do not complete real transactions.

## The idea

This project treats terrarium as an atmosphere to enter. Its selected scenes move from **Moss Forest** to **The water cycle**, giving the central subject several different scales and moods. The result is a designed world rather than a catalogue of screens.

<p align="center"><img src="docs/chapters.svg" alt="Four themed chapters from Bell & Moss" width="100%"></p>

## Four scenes

| No. | Scene | Place in the story |
| --- | --- | --- |
| 1 | **Moss Forest** | A shaded world with its own floor. |
| 2 | **High Desert** | A dry landscape under glass. |
| 3 | **Cloud Tropic** | Humidity gathers above the canopy. |
| 4 | **The water cycle** | A closed world tends itself. |

These scenes are a selection from the full site. The page also contains supporting editorial sections and a closing invitation.

## Visual language

Linen paper, moss green, walnut brown, and soft editorial type make a miniature ecosystem feel like a keepsake.

The color plate below records the project's ground, ink, accent, and secondary tone. The type families in the design are Fraunces · Manrope.

<p align="center"><img src="docs/palette.svg" alt="Bell & Moss color and typography plate" width="100%"></p>

## The site

The experience is built for the browser, with a visual scene that responds to the page and pointer. Its text remains arranged as a readable sequence of sections. The screenshot below shows the opening composition.

<p align="center"><img src="docs/media/terrarium.webp" alt="Opening screen of the Bell & Moss website" width="100%"></p>

<p align="center"><sub>Opening scene captured from the original project.</sub></p>

## Built with

| Part | Tools |
| --- | --- |
| Site and build | JavaScript, Vite, Tailwind CSS, custom CSS |
| Three-dimensional scene | Three.js and project-specific shaders/models |
| Motion and scrolling | GSAP, ScrollTrigger, Lenis |
| Hosting configuration | Cloudflare Pages, `wrangler.jsonc` |

The site is one project at the repository root. The current application is in `src/`; render, asset, input, scroll, and UI utilities are in `src/core/`. Old collection material is preserved under `docs/archive/`.

## Run locally

Use Node.js 22.12 or newer:

```bash
npm ci
npm run dev
```

Vite serves the site at `http://127.0.0.1:5190/`. To build and preview the production output:

```bash
npm run build
npm run preview
```

The build writes to `dist/`; preview serves it at `http://127.0.0.1:5191/`.

## Deployment

For Cloudflare Pages, connect the repository's `main` branch. Use `npm run build` as the build command, `dist` as the output directory, and the repository root as the root directory. The React (Vite) preset supplies the build values; `wrangler.jsonc` also records the Pages output directory. The intended address is `https://terrarium.aarya.cyou/`; DNS and a Pages project must be connected separately before it becomes live.

## Repository guide

| Path | Contents |
| --- | --- |
| `index.html` | Single site entry |
| `src/` | Scene, styles, shaders, and page modules |
| `src/core/` | Shared rendering and interaction utilities |
| `public/` | Project models and images |
| `docs/` | Project art, screenshot, credits, and notices |
| `docs/archive/` | Preserved earlier collection material |
| `wrangler.jsonc` | Cloudflare Pages output configuration |

## Rights and credits

The repository has separate rights scopes. Reuse rights for one part do not extend to the others:

| Material | Terms |
| --- | --- |
| Adapted source code | [MIT license](LICENSE), with the original copyright retained |
| New project SVGs and original presentation | [Bell & Moss content notice](LICENSE-TERRARIUM.md) |
| Zyrix Dev name and marks, where referenced | [Zyrix Dev brand notice](LICENSE-ZYRIXDEV.md) |
| Models, source images, and the screenshot | [Asset licenses](docs/ASSET-LICENSES.md) |
| Libraries and web fonts | [Third-party notices](docs/THIRD-PARTY-NOTICES.md) |

The source project and contributors are acknowledged in [Credits](docs/CREDITS.md). The original source copyright remains in [LICENSE](LICENSE).
