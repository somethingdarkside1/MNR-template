# Midnight Nexus Records - Cyberpunk Website Template

The template of [Midnight Nexus Records](https://midnightnexusrecords.com/).

A modern, responsive website template featuring a cyberpunk aesthetic with interactive particle animations, glowing effects. Built with vanilla JavaScript and CSS, focusing on performance and customization. Built with Claude 3.5 Sonnet in about 20 minutes.

## Features

- Interactive particle background
- Customizable settings
- Glitch and glow animations
- Customizable color schemes
- Fully responsive layout
- No dependencies required

## Table of Contents

- [Features](#features)
- [Quick Start](#quick-start)
- [Customization](#customization)
  - [Colors](#colors)
  - [Fonts](#fonts)
  - [Particle System](#particle-system)
- [Structure](#structure)
- [Browser Support](#browser-support)
- [Contributing](#contributing)
- [License](#license)

## Quick Start

1. Open `index.html` in your preferred editor
2. Replace placeholder content with your own
3. Customize colors and fonts (see [Customization](#customization))
4. Deploy to your hosting service

## Customization

### Colors

The template uses CSS variables for easy color customization. Edit these in the `:root` section of `style.css`:

```css
:root {
    --primary-color: #ff00ff;     /* Primary accent color */
    --secondary-color: #00ffff;   /* Secondary accent color */
    --background-color: #0c0c1d;  /* Main background */
    --text-color: #fff;          /* Default text color */
    --gradient-start: #9333FF;   /* Gradient animations start */
    --gradient-end: #00ffff;     /* Gradient animations end */
}
```

### Fonts

Choose ONE font combination. Add the corresponding link to your HTML `<head>` and CSS variables to your stylesheet.

### Particle System

The background animation can be customized in `particles.js`. Adjust these settings for different effects:

```javascript
const SETTINGS = {
    // Particle count - adjust based on screen size
    NODE_COUNT: Math.min(50, Math.floor((canvasWidth * canvasHeight) / 20000)),
    
    // Maximum distance for particle connections
    MAX_DISTANCE: 200,
    
    // Individual particle size
    BASE_PARTICLE_SIZE: 2.5,
    
    // Color range for particles
    HUE_RANGE: {
        start: 170,  // Starting hue value
        range: 60    // Amount of hue variation
    },
    
    // Overall animation speed
    ANIMATION_SPEED: 0.001
};
```

#### Performance Tips
- Reduce `NODE_COUNT` for better performance on mobile devices
- Decrease `MAX_DISTANCE` to reduce the number of connections
- Increase `ANIMATION_SPEED` for smoother animation on powerful devices

## Structure

### Main Sections

#### Header/Logo
```html
<svg class="logo" viewBox="0 0 100 100">
    <!-- Replace with your logo SVG -->
</svg>
```

#### Biography Section
```html
<section class="bio-container">
    <h2 id="about-section" class="visually-hidden">About</h2>
    <p class="bio-text">Your introduction</p>
    <div class="bio-signature">
        <p>- Your Name</p>
    </div>
</section>
```

#### Project Cards
```html
<section class="projects-section">
    <a href="project-url" class="project-card">
        <h3 class="project-title">Project Name</h3>
        <div class="project-description">
            Project details here
        </div>
    </a>
</section>
```

## License

This work is licensed under a [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/).

You are free to:
- Share — copy and redistribute the material in any medium or format
- Adapt — remix, transform, and build upon the material for any purpose, even commercially

Under the following terms:
- Attribution — Please include a link back to this repository or "Template by [Your Name]" in your project.

## Contact

Your Name - [@yourtwitter](https://twitter.com/yourtwitter) - email@example.com
Project Link: [https://github.com/yourusername/cyberpunk-website-template](https://github.com/yourusername/cyberpunk-website-template)
