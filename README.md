<p align="center">
  <img src="./assets/brand/swiper-merch-carousel-header.jpg" alt="Swiper Merchandise Carousel header" />
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="MIT License" /></a>
  <a href="https://swiperjs.com/"><img src="https://img.shields.io/badge/SwiperJS-v11-green.svg" alt="SwiperJS v11" /></a>
  <a href="https://github.com/MADPANDA3D"><img src="https://img.shields.io/badge/Built%20by-MADPANDA3D-black?style=flat-square" alt="Built by MADPANDA3D" /></a>
</p>

<h1 align="center">Swiper Merchandise Carousel</h1>

<p align="center">A plug-and-play product carousel built with SwiperJS v11. Static HTML/CSS/JS, no build step.</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/MADPANDA3D/SWIPER-MERCH-CAROUSEL/main/assets/demo.gif" width="800" alt="Swiper Merchandise Carousel demo" />
</p>

## Screenshots

![Base Carousel](https://raw.githubusercontent.com/MADPANDA3D/SWIPER-MERCH-CAROUSEL/main/assets/screenshots/base-carousel.png)
![Coverflow Carousel](https://raw.githubusercontent.com/MADPANDA3D/SWIPER-MERCH-CAROUSEL/main/assets/screenshots/stacked-coverflow.png)

## Overview

This repo provides a ready-to-embed carousel for merch or product showcases. It uses SwiperJS via CDN and focuses on a clean, responsive layout with a coverflow effect.

## Status

- Stage: stable
- Maintainer: MADPANDA3D
- Support: GitHub issues

## Quick Start

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

## Support

[![Donate to the Project](https://img.shields.io/badge/Donate_to_the_Project-Support_Development-ff69b4?style=for-the-badge&logo=heart&logoColor=white)](https://donate.stripe.com/cNidRbdkAbdP8iU7SD4ko0b)

## Affiliate Links

<details>
<summary>Services I use (affiliate)</summary>

Using these links helps support continued development.

### Hostinger VPS
- [KVM 1](https://www.hostinger.com/cart?product=vps%3Avps_kvm_1&period=12&referral_type=cart_link&REFERRALCODE=ZUWMADPANOFE&referral_id=0199a491-d783-7057-85d2-27de6e01e2c5)
- [KVM 2](https://www.hostinger.com/cart?product=vps%3Avps_kvm_2&period=12&referral_type=cart_link&REFERRALCODE=ZUWMADPANOFE&referral_id=0199a492-26cf-7333-b6d7-692e17bf8ce1)
- [KVM 4](https://www.hostinger.com/cart?product=vps%3Avps_kvm_4&period=12&referral_type=cart_link&REFERRALCODE=ZUWMADPANOFE&referral_id=0199a492-531e-70d3-83f5-e28eb919466d)
- [KVM 8](https://www.hostinger.com/cart?product=vps%3Avps_kvm_8&period=12&referral_type=cart_link&REFERRALCODE=ZUWMADPANOFE&referral_id=0199a492-7ce9-70fb-b96c-2184abc56764)

### Cloud Hosting
- [Cloud Economy](https://www.hostinger.com/cart?product=hosting%3Acloud_economy&period=12&referral_type=cart_link&REFERRALCODE=ZUWMADPANOFE&referral_id=0199a48f-e7fa-7358-9ff0-f9ba2e8d6e36)
- [Cloud Professional](https://www.hostinger.com/cart?product=hosting%3Acloud_professional&period=12&referral_type=cart_link&REFERRALCODE=ZUWMADPANOFE&referral_id=0199a490-20fd-70bc-959e-a1f2cd9a69a6)
- [Cloud Enterprise](https://www.hostinger.com/cart?product=hosting%3Acloud_enterprise&period=12&referral_type=cart_link&REFERRALCODE=ZUWMADPANOFE&referral_id=0199a490-5972-72e4-850f-40d618988dc1)

### Web Hosting
- [Premium](https://www.hostinger.com/cart?product=hosting%3Ahostinger_premium&period=12&referral_type=cart_link&REFERRALCODE=ZUWMADPANOFE&referral_id=0199a48f-4c21-7199-9918-8f31a3f6a0d9)
- [Business](https://www.hostinger.com/cart?product=hosting%3Ahostinger_business&period=12&referral_type=cart_link&REFERRALCODE=ZUWMADPANOFE&referral_id=0199a48f-1135-72ba-acbb-13e0e7550db0)

### Website Builder
- [Premium](https://www.hostinger.com/cart?product=hosting%3Ahostinger_premium&period=12&referral_type=cart_link&REFERRALCODE=ZUWMADPANOFE&referral_id=0199a492-f240-7309-b3fe-9f6909fbc769&product_type=website-builder)
- [Business](https://www.hostinger.com/cart?product=hosting%3Ahostinger_business&period=12&referral_type=cart_link&REFERRALCODE=ZUWMADPANOFE&referral_id=0199a492-7ce9-70fb-b96c-2184abc56764)

### Agency Hosting
- [Startup](https://www.hostinger.com/cart?product=hosting%3Aagency_startup&period=12&referral_type=cart_link&REFERRALCODE=ZUWMADPANOFE&referral_id=0199a490-d03c-71de-9acf-08fd4fa911de)
- [Growth](https://www.hostinger.com/cart?product=hosting%3Aagency_growth&period=12&referral_type=cart_link&REFERRALCODE=ZUWMADPANOFE&referral_id=0199a491-6af4-731f-8947-f1458f07fa5b)
- [Professional](https://www.hostinger.com/cart?product=hosting%3Aagency_professional&period=12&referral_type=cart_link&REFERRALCODE=ZUWMADPANOFE&referral_id=0199a491-03fb-73f8-9910-044a0a33393a)

### Email
- [Business Pro](https://www.hostinger.com/cart?product=hostinger_mail%3Apro&period=12&referral_type=cart_link&REFERRALCODE=ZUWMADPANOFE&referral_id=0199a493-5c27-727b-b7f9-8747ffb4e5ee)
- [Business Premium](https://www.hostinger.com/cart?product=hostinger_mail%3Apremium&period=12&referral_type=cart_link&REFERRALCODE=ZUWMADPANOFE&referral_id=0199a493-a3fc-72b8-a961-94ed6e1c70e6)

### Reach
- [Reach 500](https://www.hostinger.com/cart?product=reach%3A500&period=12&referral_type=cart_link&REFERRALCODE=ZUWMADPANOFE&referral_id=0199a494-3ebf-7367-b409-9948de50a297)
- [Reach 1000](https://www.hostinger.com/cart?product=reach%3A1000&period=12&referral_type=cart_link&REFERRALCODE=ZUWMADPANOFE&referral_id=0199a494-8bb9-726e-bb8d-9de9a72a3c21)
- [Reach 2500](https://www.hostinger.com/cart?product=reach%3A2500&period=12&referral_type=cart_link&REFERRALCODE=ZUWMADPANOFE&referral_id=0199a494-c9c1-7191-b600-cafa2e9adafc)

</details>

## Contact

Open an issue in `MADPANDA3D/SWIPER-MERCH-CAROUSEL`.

<p align="center">
  <img src="https://assets.zyrosite.com/cdn-cgi/image/format=auto,w=316,fit=crop,q=95/dJo56xnDoJCnbgxg/official-logo-mxBMZGQ8Owc8p2M2.jpeg" width="160" alt="MADPANDA3D logo" />
  <br />
  <strong>MADPANDA3D</strong>
</p>
