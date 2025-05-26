# SwiperJS Merchandise Carousel Customization Guide

This guide covers how to customize the SwiperJS Merchandise Carousel for your specific needs.

## Table of Contents
- [Basic Customization](#basic-customization)
- [Advanced Configuration](#advanced-configuration)
- [Styling Options](#styling-options)
- [Event Handling](#event-handling)
- [Responsive Design](#responsive-design)

## Basic Customization

### Replacing Images
To replace the placeholder images with your own product images:

1. Locate the slide elements in `index.html`:
```html
<div class="swiper-slide"><img src="https://example.com/images/slide1.jpg" style="width:65%; border-radius: 10px; display: block; margin: auto;" /><!-- Add your image URL here --></div>
```

2. Replace the `src` attribute with your image URL:
```html
<div class="swiper-slide"><img src="https://your-domain.com/path/to/product1.jpg" style="width:65%; border-radius: 10px; display: block; margin: auto;" /></div>
```

### Adding More Slides
To add more product slides:

1. Copy an existing slide element
2. Paste it within the `swiper-wrapper` div
3. Update the image source to your new product image

```html
<div class="swiper-wrapper" style="align-items: center;">
  <!-- Existing slides -->
  
  <!-- New slide -->
  <div class="swiper-slide"><img src="https://your-domain.com/path/to/product6.jpg" style="width:65%; border-radius: 10px; display: block; margin: auto;" /></div>
</div>
```

### Changing Background Color
To change the background color of the carousel container:

1. Locate the outer container div:
```html
<div style="width: 100%; background-color: #1C3C93; padding: 60px 0; box-sizing: border-box;">
```

2. Change the `background-color` value to your desired color:
```html
<div style="width: 100%; background-color: #FF5733; padding: 60px 0; box-sizing: border-box;">
```

## Advanced Configuration

### Swiper Parameters
The carousel is initialized with the following configuration:

```javascript
const swiper = new Swiper(".swiper-container", {
  effect: "coverflow",
  grabCursor: true,
  centeredSlides: true,
  slidesPerView: "auto",
  speed: 1200,
  loop: true,
  coverflowEffect: {
    rotate: 0,
    stretch: 300,  // 👈 Tight overlap
    depth: 350,
    modifier: 0.85,
    slideShadows: false,
  },
  autoplay: {
    delay: 3000,
    disableOnInteraction: false
  },
  navigation: {
    nextEl: ".swiper-button-next",
    prevEl: ".swiper-button-prev"
  },
  pagination: {
    el: ".swiper-pagination",
    clickable: true
  },
  // Additional event handlers
});
```

You can modify these parameters to change the carousel behavior:

- **effect**: Change to "slide", "fade", "cube", or "flip" for different transition effects
- **speed**: Adjust the transition speed in milliseconds
- **slidesPerView**: Change to a number (e.g., 3) to show multiple slides
- **spaceBetween**: Add spacing between slides (e.g., 30)
- **autoplay.delay**: Change the time between automatic slide transitions

### CoverFlow Effect Options
The coverflow effect can be customized:

- **rotate**: Rotation angle (in degrees)
- **stretch**: Stretching ratio (lower = less stretch)
- **depth**: Depth offset ratio (higher = more perspective)
- **modifier**: Effect multiplier (lower = less intense effect)
- **slideShadows**: Enable/disable slide shadows

Example:
```javascript
coverflowEffect: {
  rotate: 20,           // Add rotation
  stretch: 200,         // Less stretch
  depth: 400,           // More depth
  modifier: 1,          // Standard effect
  slideShadows: true,   // Enable shadows
}
```

## Styling Options

### Image Styling
Customize the appearance of your product images:

```html
<div class="swiper-slide">
  <img src="https://example.com/images/slide1.jpg" 
       style="width: 75%;                   /* Change size */
              border-radius: 15px;          /* Rounded corners */
              display: block;
              margin: auto;
              box-shadow: 0 5px 15px rgba(0,0,0,0.3);  /* Add shadow */
              border: 2px solid white;      /* Add border */
              " />
</div>
```

### Pagination Dots
Customize the pagination dots at the bottom:

```css
.swiper-pagination-bullet {
  background: white !important;    /* Dot color */
  opacity: 0.5;                    /* Inactive dot opacity */
  width: 12px;                     /* Dot size */
  height: 12px;                    /* Dot size */
  margin: 0 6px;                   /* Dot spacing */
}

.swiper-pagination-bullet-active {
  opacity: 1 !important;           /* Active dot opacity */
  background: #ffcc00 !important;  /* Active dot color */
}
```

### Navigation Arrows
Customize the navigation arrows:

```css
.swiper-button-next, .swiper-button-prev {
  color: #ffffff;                   /* Arrow color */
  background: rgba(0,0,0,0.3);      /* Arrow background */
  width: 40px;                      /* Arrow size */
  height: 40px;                     /* Arrow size */
  border-radius: 50%;               /* Round arrows */
  display: flex;
  justify-content: center;
  align-items: center;
}

.swiper-button-next:after, .swiper-button-prev:after {
  font-size: 18px;                  /* Arrow icon size */
}
```

## Event Handling

### Click Events
Add click events to your slides:

```javascript
// Add after swiper initialization
swiper.slides.forEach((slide, index) => {
  slide.addEventListener('click', () => {
    console.log(`Slide ${index+1} clicked!`);
    // Add your custom action here
    // e.g., open product details, add to cart, etc.
    window.open(`https://your-shop.com/product/${index+1}`, '_blank');
  });
});
```

### Custom Pause/Resume
The carousel includes a custom autoplay pause/resume feature:

```javascript
function pauseAutoplay() {
  autoplayPaused = true;
  swiper.autoplay.stop();
  clearTimeout(autoplayTimeout);
  autoplayTimeout = setTimeout(() => {
    swiper.autoplay.start();
    autoplayPaused = false;
  }, 5000);  // Change this value to adjust pause duration
}
```

## Responsive Design

To make your carousel responsive, add media queries:

```html
<style>
  /* Default settings */
  .swiper-container {
    max-width: 900px;
  }
  
  /* Tablet adjustments */
  @media (max-width: 768px) {
    .swiper-container {
      max-width: 700px;
    }
    .swiper-slide img {
      width: 75%;
    }
  }
  
  /* Mobile adjustments */
  @media (max-width: 480px) {
    .swiper-container {
      max-width: 100%;
      padding: 0 20px;
    }
    .swiper-slide img {
      width: 85%;
    }
    .swiper-button-next, .swiper-button-prev {
      width: 30px;
      height: 30px;
    }
  }
</style>
```

## Advanced Examples

For more examples and advanced implementations, refer to:
- [SwiperJS API Documentation](https://swiperjs.com/swiper-api)
- [SwiperJS Demos](https://swiperjs.com/demos)

---

Need more help? Check out our [GitHub repository](https://github.com/yourusername/swiper-merch-carousel) or open an issue.