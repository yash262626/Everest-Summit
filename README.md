# Everest — The Roof of the World

[![Explore Live](https://img.shields.io/badge/🏔️_Explore_Live-Open_Everest-00C7B7?style=for-the-badge)](https://yash262626.github.io/Everest-Summit/)

A cinematic, **scroll-driven journey to the summit of Mount Everest (8,849 m)**. You start in the thin air of the Himalaya, follow the South Col route camp by camp, and reach the top. The page tracks your altitude and the drop in oxygen as you scroll.

Everything is in a single `index.html`: no build step and no server. Open it in a browser or host it anywhere static.

---

## The journey

The site is split into five chapters, reachable from the index menu:

| # | Chapter | What you see |
|---|---|---|
| 01 | **Mountain** | Hero title, coordinates (27°59′N 86°55′E), key facts (peak, elevation, border, lat/long). "Sagarmatha. Chomolungma. Everest." — three names for one mountain, plus the geology: marine limestone from an ancient ocean, uplifted as India collides with Asia. |
| 02 | **History** | "A century on the mountain", a timeline of the mountain's story, including Hillary and Tenzing Norgay's first ascent. |
| 03 | **Expedition** | "The South Col route": six stops and about 3.5 vertical kilometres, from Base Camp to the summit, with an interactive route atlas. |
| 04 | **Climb** | Scroll-linked altitude counter, oxygen versus sea level, and a stage tracker (1 / 6) through the camps. |
| 05 | **Summit** | 8,849 m, the highest point on Earth above sea level, then the finale: "The mountain remains." |

### The route (from the atlas)

Base Camp **5,364 m** → Khumbu Icefall **5,486 m** → Camp I **6,065 m** → Camp II **6,400 m** → Camp III **7,470 m** → Camp IV **7,920 m** → Summit **8,849 m**.
Above 8,000 m is flagged as the death zone. Landmarks on the map include the Khumbu Glacier, Western Cwm, Lhotse Face and the Yellow Band.

## Features

- Scroll-driven storytelling: pinned sections, scrubbed animation, split-text reveals
- Smooth, inertial scrolling
- Live **altitude counter** and **oxygen %** that update as you scroll (Base Camp is about 53% of sea-level oxygen)
- **Interactive route atlas**: hover, tap or tab to a point on an illustrated map to see its altitude and notes
- **Ambient sound** with a toggle (off by default), built with Web Audio
- **Hide UI** button for an unobstructed, cinematic view
- Loading screen ("Acclimatising") with a progress counter
- Keyboard accessible: skip-to-content link, focus support on atlas points, screen-reader headings
- Respects `prefers-reduced-motion`
- Responsive layout for desktop, tablet and mobile
- SEO and sharing metadata (description, Open Graph, theme colour)

## Tech stack

| Area | Tools |
|---|---|
| Animation | **GSAP** with **ScrollTrigger** and **Observer** |
| Smooth scroll | **Lenis** |
| Visuals | HTML5 **Canvas** / WebGL, CSS, inline SVG (route map) |
| Sound | Web Audio API |
| Fonts | Embedded `@font-face` |
| Build | None: one self-contained HTML file |

## Run locally

1. Download or clone the repo.
2. Open `index.html` in Chrome, Edge, Firefox or Safari.

For best results use a desktop browser with hardware acceleration on.

## Deploy

- **Netlify:** drag the folder onto app.netlify.com/drop.
- **GitHub Pages:** Settings → Pages → Deploy from branch → `main` / root.

## Credits

- Design and development: **Yash Dhanraj Ail**
- Photographs from Unsplash by Giuseppe Mondì, Andreas Gäbler, Weichao Deng, Luo Lei, Sebastian Pena Lambarri and Michael Clarke
- The route map is an original illustration

---

© 2026 Yash Dhanraj Ail. All rights reserved.
