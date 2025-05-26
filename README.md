# 🎠 Swiper Merchandise Carousel

> A modular, ready-to-use product carousel template built with SwiperJS v11

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![SwiperJS: v11](https://img.shields.io/badge/SwiperJS-v11-green.svg)](https://swiperjs.com/)
[![Demo](https://img.shields.io/badge/Live-Demo-orange.svg)](https://github.com/yourusername/swiper-merch-carousel)

<p align="center">
  <img src="./assets/gifs/download.gif" alt="Swiper Merchandise Carousel Demo" width="800px" />
</p>

## 🚀 Features

- **Zero Installation** - Uses SwiperJS via CDN, no npm/build process required
- **Coverflow Effect** - Stunning 3D rotation effect with depth and perspective
- **Mobile Friendly** - Fully responsive design that works on all devices
- **Easy to Customize** - Simple HTML/CSS structure with inline styles for quick edits
- **Smart Autoplay** - Pauses on interaction and resumes automatically
- **Accessibility** - Keyboard navigation and ARIA attributes included
- **Lightweight** - Minimal code footprint for optimal performance
- **SEO Friendly** - Properly structured content for search engines

## 📸 Showcase

<div align="center">
  <img src="./assets/screenshots/screenshot_1.png" alt="Watch Product Display" width="400px" />
  <img src="./assets/screenshots/screenshot_2.png" alt="Apparel Carousel" width="400px" />
</div>

## 🛠️ Quick Start

1. **Clone this repository**:
   ```bash
   git clone https://github.com/yourusername/swiper-merch-carousel.git
   ```

2. **Open the project**:
   ```bash
   cd swiper-merch-carousel
   ```

3. **Customize with your products**:
   - Replace placeholder images in `index.html` with your product images
   - Adjust styling as needed (colors, sizes, etc.)
   - Modify coverflow effect parameters for your desired look

4. **Test locally**:
   - Open `index.html` in your browser
   - Test navigation, autoplay, and responsive behavior

5. **Deploy to your website**:
   - Upload the files to your web server
   - Or use GitHub Pages for free hosting

## 📋 Usage Example

```html
<!-- Outer Container -->
<div style="width: 100%; background-color: #1C3C93; padding: 60px 0; box-sizing: border-box;">
  <div class="swiper-container" style="max-width: 900px; margin: auto; position: relative;">
    <div class="swiper-wrapper" style="align-items: center;">

      <!-- Product Slides -->
      <div class="swiper-slide"><img src="https://example.com/products/item1.jpg" style="width:65%; border-radius: 10px; display: block; margin: auto;" /></div>
      <div class="swiper-slide"><img src="https://example.com/products/item2.jpg" style="width:65%; border-radius: 10px; display: block; margin: auto;" /></div>
      <!-- Add more slides as needed -->

    </div>

    <!-- Navigation Elements -->
    <div style="display: flex; justify-content: center; align-items: center; gap: 20px; margin-top: 30px;">
      <div class="swiper-button-prev" style="position: static; width: 32px; height: 32px; color: white; cursor: pointer;"></div>
      <div class="swiper-pagination" style="position: static;"></div>
      <div class="swiper-button-next" style="position: static; width: 32px; height: 32px; color: white; cursor: pointer;"></div>
    </div>
  </div>
</div>
```

## 🎨 Customization

For detailed customization options, refer to the [Customization Guide](./docs/customization-guide.md).

<p align="center">
  <img src="./assets/screenshots/screenshot_3.png" alt="Embedding Code Example" width="400px" />
</p>

Quick customization points:

- **Background Color**: Change the outer container's `background-color`
- **Container Width**: Adjust the `max-width` of the swiper container
- **Image Size**: Modify the `width` percentage of images
- **Transition Speed**: Update the `speed` parameter in the Swiper config
- **Effect Parameters**: Customize the `coverflowEffect` object properties
- **Autoplay Timing**: Change the `delay` value in the autoplay settings

## 📱 Browser Compatibility

- Chrome 49+
- Firefox 52+
- Safari 9.1+
- Edge 14+
- Opera 36+
- iOS Safari 9.3+
- Android Browser 4.4+
- Chrome for Android 103+

## 🛣️ Roadmap

- [ ] Add product info overlay option
- [ ] Create multiple theme variations
- [ ] Add click-to-zoom functionality
- [ ] Implement lazy loading for better performance
- [ ] Create npm package version with bundled components

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [SwiperJS](https://swiperjs.com/) for the amazing carousel library
- [Vladimir Kharlampidi](https://github.com/nolimits4web) for creating Swiper

---

<p align="center">
  Made with ❤️ for the open-source community
</p>