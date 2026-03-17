English | [简体中文](README.md)

# Beijing in Ten Days


`Beijing in Ten Days` is a static front-end showcase page built around a curated 10-day cultural itinerary in Beijing. The project focuses on immersive visual storytelling, scroll-based motion, itinerary cards, and a polished presentation style that works well for portfolio pieces, travel landing pages, or visual design experiments.

## Features

- Cinematic hero section with a loading transition
- Pre-trip planning cards for reservations, transit, food, lodging, and packing
- A modular 10-day itinerary presentation
- Scroll progress bar, animated counters, and parallax-inspired motion
- Custom cursor and hover interactions
- Mobile-friendly responsive layout

## Tech Stack

- `HTML5`
- `CSS3`
- `Vanilla JavaScript`
- `GSAP` loaded from CDN with `ScrollTrigger`, `ScrollToPlugin`, and `TextPlugin`

## Run Locally

No build step is required. Start a static file server:

```bash
git clone https://github.com/saudademjj/123.git
cd 123
python3 -m http.server 8080
```

Then open `http://localhost:8080`

## Structure

```text
123/
├── index.html
├── styles.css
├── script.js
├── README.md
└── README.en.md
```

## Customization

- Edit `index.html` to change the itinerary content
- Update `styles.css` root variables to retheme the page
- Tweak GSAP timelines and triggers in `script.js`

## Deployment

This project can be deployed directly to:

- GitHub Pages
- Vercel
- Netlify
- Any static Nginx directory

## License

This project is licensed under the MIT License. See [LICENSE](./LICENSE).
