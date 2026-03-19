<div align="center">
  English | <a href="./README.md">简体中文</a>
</div>

# Beijing 10-Day Journal -- Immersive Artistic Web Experience

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![GSAP](https://img.shields.io/badge/GSAP-3.12-88CE02?style=flat-square&logo=greensock)

An immersive static web page themed around a "10-Day Beijing Journal," documenting a deep cultural exploration of Beijing. The design blends modern artistic aesthetics with immersive interactive experiences, built entirely with native web technologies without any frontend frameworks, achieving cinematic visual storytelling through the GSAP animation engine.

## Design Philosophy

This project elevates travel documentation into a visual narrative experience. Unlike traditional photo-and-text blogs, the page uses carefully choreographed animation timing, scroll-driven content reveals, and cinematic transitions to make viewers feel as though they are walking through each day in Beijing alongside the author.

## Core Interaction Features

### Cinematic Opening

- Full-screen loading transition: Serif-font title gradually reveals, creating a sense of ceremony
- Smooth transition to main content area after loading completes
- Hero section with background animation and "Begin the Journey" CTA button

### Scroll-Driven Storytelling

- Real-time reading progress bar at the top of the page reflecting current scroll position
- GSAP ScrollTrigger-based block fade-in animations: content progressively reveals as the user scrolls
- Smooth-scroll navigation anchoring to sections (Planning / Stats / Itinerary)

### Custom Cursor System

- Dual-layer cursor design: outer ring (cursor) + inner dot (cursor-dot)
- Cursor follows mouse movement with smooth delayed tracking
- Morphing feedback on interactive elements (links, buttons)

### Dynamic Data Display

- Key numbers (trip days, attraction count, walking distance, etc.) trigger zero-to-target increment animations when entering the viewport
- Data counters paired with easing functions present natural numerical progression

### Card-Based Itinerary Layout

- 10-day itinerary presented in a responsive card grid layout
- Each card contains date, theme, and trip highlights
- Custom visual feedback on card hover

## Page Structure

The page consists of the following major sections:

- Hero Section: Full-screen title with background animation, guiding users to begin browsing
- Pre-trip Planning: Key travel preparation elements and practical advice
- Data Overview: Dynamic visualization of key trip statistics
- 10-Day Itinerary: Day-by-day detailed card-based itinerary

## Technology Stack

- HTML5: Semantic markup structure with attention to document accessibility and SEO
- CSS3
  - Native custom properties (CSS Variables) for unified theme management
  - Flexbox and Grid hybrid layouts
  - Responsive media queries adapting to multiple screen sizes
  - Custom scrollbar styling
  - Transitions and keyframe animations
- Vanilla JavaScript
  - DOM manipulation and event listeners
  - Intersection Observer API for element visibility detection
  - Custom cursor position calculation and tracking logic
  - Data counter increment algorithms
- GSAP (GreenSock Animation Platform)
  - Industrial-grade animation engine loaded via CDN
  - ScrollTrigger Plugin: Scroll-position-driven animation triggering and timeline control
  - Rich easing function presets for natural motion curves
- Google Fonts
  - Noto Sans SC: Body sans-serif font
  - Noto Serif SC: Heading serif font for cultural texture

## File Structure

```text
123/
├── index.html       # Main page: complete content structure and semantic markup
├── styles.css       # Global styles: CSS variables, layout, responsive rules, animations
├── script.js        # Interaction logic: GSAP animations, ScrollTrigger, counters, cursor
└── README.md        # Project documentation
```

## Local Preview

No build tools or dependency installation required. Use Python's built-in HTTP server:

```bash
git clone https://github.com/saudademjj/123.git
cd 123
python3 -m http.server 8080
```

Visit `http://localhost:8080` in your browser to see the full experience.

Alternative static file servers also work:

```bash
# Using Node.js serve
npx serve .

# Using PHP built-in server
php -S localhost:8080
```

## Customization Guide

This project is well-suited as a template for travel journals, event pages, or personal narrative pages:

### Content Modification
- Edit text content, section structure, and card data in `index.html`
- Replace the Hero section title and subtitle
- Adjust the number of itinerary days and card content

### Theme Colors
- Modify CSS variables in the `:root` section at the top of `styles.css`
- Adjust background colors, text colors, accent colors, and other theme parameters

### Animation Tuning
- Modify GSAP timeline configurations in `script.js`
- Adjust ScrollTrigger trigger positions and animation durations
- Change easing functions to alter animation rhythm

### Font Replacement
- Replace Google Fonts links in the `<head>` of `index.html`
- Update corresponding `font-family` declarations in `styles.css`

## Browser Compatibility

- Recommended: Modern browsers (latest versions of Chrome, Firefox, Safari, Edge)
- GSAP ScrollTrigger requires Intersection Observer API support
- Custom cursor effects are automatically hidden on touch devices

## License

MIT License
