# CLAUDE.md

## Project Overview

Personal portfolio website for Evan Luputra — Senior UX Designer at Expedia. Built with Astro and Tailwind CSS.

## Tech Stack

- **Framework:** Astro 4.x
- **Styling:** Tailwind CSS 3.x with `@astrojs/tailwind`
- **Language:** TypeScript
- **Font:** Poppins (Google Fonts)

## Project Structure

```
src/
  components/     # Astro components (one per section)
  layouts/        # Layout.astro — base HTML shell
  pages/          # index.astro — single page
  styles/         # global.css
public/           # Static assets
```

## Page Sections (in order)

1. `Navbar` — navigation with links to Projects, About, Resume
2. `Hero` — intro, title, CTA buttons
3. `Projects` — portfolio work
4. `TrustedBy` — client/company logos
5. `Services` — offered services
6. `Testimonials` — client testimonials
7. `Footer`

## Design Tokens

Defined in `tailwind.config.mjs`:

| Token | Value |
|---|---|
| `primary` | `#5957d0` |
| `primary-dark` | `#4745b8` |
| `font-poppins` | `'Poppins', sans-serif` |

Base text color: `#020202`

## Common Conventions

- Components are plain `.astro` files with no props unless needed
- Layout uses `<slot />` for page content injection
- Responsive breakpoints follow Tailwind defaults (`sm`, `lg`)
- Section padding pattern: `px-5 sm:px-10 lg:px-[120px] py-12 sm:py-16 lg:py-20`
- Max content width: `max-w-7xl mx-auto`
- Button style: `btn-press` class with hover lift + shadow effect

## Dev Commands

```bash
npm run dev      # Start local dev server
npm run build    # Build for production (outputs to /dist)
npm run preview  # Preview production build
```

## Figma Design

- **File:** Evan portfolio 2026
- **File Key:** `1N5lu2pPHv611ODI0I6eM0`
- **Main frame:** `Portfolio Kesatu` (node `1:26960`) — 1440px wide desktop design
