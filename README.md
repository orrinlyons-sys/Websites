# Bord De L'Eau — Restaurant Website

Professional website for **Bord De L'Eau**, a French restaurant at 2 Market Street, Wick, Scotland.

## Features

- Fullscreen hero with animated river waves
- Smooth scroll reveal animations throughout
- Interactive tabbed menu (Starters / Mains / Desserts)
- Reviews section with TripAdvisor quotes
- Visit section with hours, address, and map link
- Fixed navigation with scroll-aware styling
- Mobile-responsive with hamburger menu
- Zero dependencies — pure HTML, CSS, and vanilla JS
- Google Fonts only external resource

## Structure

```
bord-de-leau/
└── index.html    # Complete single-file website
```

## Customisation

### Update contact details
Search for `+441955604400` and replace with the current phone number.
Update the email address in the CTA section (`info@borddeleau.co.uk`).

### Update menu prices
Prices are hardcoded in the menu section. Search for `£` to find all instances.

### Add a real map
Replace the `.map-placeholder` div with a Google Maps embed iframe:
```html
<iframe
  src="https://www.google.com/maps/embed?pb=..."
  width="100%" height="400"
  style="border:0;" allowfullscreen loading="lazy">
</iframe>
```

### Opening hours
Update the hours table inside the `#visit` section to match current hours.

### Add photos
Replace the hero background gradient with a real image:
```css
.hero-bg {
  background-image: url('images/hero.jpg');
  background-size: cover;
  background-position: center;
}
```

## Deployment

This is a single HTML file — no build step needed.

**GitHub Pages (free hosting):**
1. Push this repo to GitHub
2. Go to Settings → Pages → Source: main branch / root
3. Site will be live at `https://yourusername.github.io/bord-de-leau`

**Custom domain:**
Add a `CNAME` file containing your domain (e.g. `www.borddeleau.co.uk`) and configure your DNS accordingly.

## Tech

- HTML5 / CSS3 / Vanilla JS
- [Cormorant Garamond](https://fonts.google.com/specimen/Cormorant+Garamond) — display serif
- [Jost](https://fonts.google.com/specimen/Jost) — UI sans-serif
- IntersectionObserver for scroll animations
- No frameworks, no dependencies, no build tools
- 
