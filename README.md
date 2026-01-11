# Swiper Merchandise Carousel

A plug-and-play product carousel built with SwiperJS v11. Static HTML/CSS/JS, no build step.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![SwiperJS: v11](https://img.shields.io/badge/SwiperJS-v11-green.svg)](https://swiperjs.com/)

<p align="center">
  <img src="https://raw.githubusercontent.com/MADPANDA3D/SWIPER-MERCH-CAROUSEL/main/assets/demo.gif" width="800" alt="Swiper Merchandise Carousel demo" />
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/MADPANDA3D/QDRANT-MCP/main/assets/brand/header.jpg" width="800" alt="Placeholder screenshot (replace)" />
  <br />
  <em>Placeholder image from another repo. Replace with your own screenshot.</em>
</p>

## Overview

This repo provides a ready-to-embed carousel for merch or product showcases. It uses SwiperJS via CDN and focuses on a clean, responsive layout with a coverflow effect.

## Status

- Stage: stable
- Maintainer: MADPANDA3D
- Support: GitHub issues

## Quick Start

```bash
# 1) Clone

```

```bash
git clone https://github.com/MADPANDA3D/SWIPER-MERCH-CAROUSEL.git
cd SWIPER-MERCH-CAROUSEL
```

```bash
# 2) Run a local server (recommended)
python3 -m http.server 8000
```

Open `http://localhost:8000` in your browser.

## Features

- Zero install: uses SwiperJS CDN
- Coverflow effect with depth and perspective
- Responsive layout for mobile and desktop
- Keyboard navigation and ARIA attributes
- Lightweight HTML/CSS structure for fast edits

## Tech Stack

- Runtime: Static HTML/CSS/JS
- UI: SwiperJS v11 (CDN)
- Hosting: Any static host

## Architecture

Single-page static layout with a Swiper instance initialized in `index.html`.

## Configuration

No environment variables required. Customize directly in `index.html`:

- Swap product images
- Adjust coverflow settings
- Tune autoplay speed
- Change colors and layout

## Usage

Embed snippet (example):

```html
<div class="swiper-container">
  <div class="swiper-wrapper">
    <div class="swiper-slide"><img src="/assets/products/item-1.jpg" alt="Product 1" /></div>
    <div class="swiper-slide"><img src="/assets/products/item-2.jpg" alt="Product 2" /></div>
  </div>
  <div class="swiper-pagination"></div>
  <div class="swiper-button-prev"></div>
  <div class="swiper-button-next"></div>
</div>
```

## Project Structure

```
.
├── assets/
├── docs/
├── index.html
└── README.md
```

## Development

Edit `index.html` and refresh your browser. No build step required.

## Testing

No automated tests.

## Deployment

- GitHub Pages, Netlify, Vercel, or any static host
- Upload the project files and set `index.html` as the entry point

## Roadmap

- Add product info overlay option
- Add click-to-zoom
- Add lazy loading for large catalogs

## Contributing

1. Fork the repo
2. Create a branch: `git checkout -b feature/name`
3. Commit: `git commit -m "Add feature"`
4. Push: `git push origin feature/name`
5. Open a PR

## License

MIT.

## Contact

Open an issue in `MADPANDA3D/SWIPER-MERCH-CAROUSEL`.
