# Stars & Stripes Canvas — Fireworks Over the Harbor

A CSS-only, multi-page Independence Day storybook built with semantic HTML5 and
CSS3. No JavaScript is used anywhere in this project — all navigation,
interactivity, and animation is achieved with `:target`, `:checked`,
`:hover`/`:focus`, CSS Grid/Flexbox, `@keyframes`, and the modern `:has()`
selector.

## Storybook chapters

1. **Freedom's Dawn** — the harbor town at dusk, before the show begins
2. **Patriot's Plaza** — the main event: an animated *Fireworks Over the Harbor*
   night scene (fireworks bursts, glowing skyline, anchored boats, a dock
   crowd, gulls, drifting smoke, shimmering water reflections)
3. **United We Stand** — the closing chapter

Navigate between chapters using the sticky header nav or the prev/next links
at the bottom of each page. Everything is driven by `:target` — no JavaScript.

## Interactive / animated elements (harbor scene)

- Three looping fireworks bursts (gold, red, blue) built with the classic
  CSS `box-shadow` spark trick
- A fourth "encore" firework triggered via a hidden checkbox + `:checked`
  (try the **🎆 Launch an Encore Firework** button)
- Twinkling stars, drifting haze, and three smoke trails
- A glowing city skyline made of pure CSS gradients (no images)
- Two anchored boats bobbing on the water
- A 12-person dock crowd with a subtle "cheer" animation
- Three gulls flying across the sky at staggered heights/speeds
- Shimmering, color-matched reflections on the harbor water

## Project structure

```
/ (project root)
├── index.html              # Stars & Stripes Canvas main storybook page
├── stars-and-stripes.css   # 4th of July theme stylesheet
├── assets/
│   ├── images/              # (empty — the scene is built entirely in CSS,
│   │                           no external images needed)
│   └── fonts/                # (empty — fonts loaded from Google Fonts
│                                 in index.html <head>)
└── README.md
```

## Accessibility notes

- Semantic landmarks: `<header>`, `<nav>`, `<main>`, `<section>`, `<footer>`
- Skip-to-content link for keyboard users
- All decorative scene elements are `aria-hidden="true"`; the scene itself
  has a descriptive `aria-label`
- Visible focus states on every link/button (`:focus-visible`)
- `prefers-reduced-motion` is respected — all animation/transition durations
  collapse to near-zero for users who request reduced motion

## Collaboration

Two team members should each have visible, meaningful commits in this
repo's history. Update the credit names in the footer of `index.html`:

```html
Built by <span class="credit-name">[Your Name]</span> &amp;
<span class="credit-name">[Partner Name]</span>
```

Suggested split:
- **Member A:** `index.html` structure + content copy
- **Member B:** `stars-and-stripes.css` animations + responsive rules

Then both commit and push your own changes so the contribution history shows
both names — that satisfies the "Collaboration & Submission" rubric line.

## Deployment

Upload this folder to `codd.cs.gsu.edu` per the assignment instructions, then
add the live URL to your submission.
