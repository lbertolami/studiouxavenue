# Studio UX Avenue

Premium UX design studio landing page.

## Tech Stack

- **Framework**: Astro v5
- **Styling**: Tailwind CSS v4 (via @tailwindcss/vite)
- **Form**: Formspree
- **Fonts**: Syne (display) + DM Sans (body)

## Project Structure

```
src/
├── layouts/
│   └── Layout.astro      # Base layout with meta tags
├── pages/
│   └── index.astro       # Main landing page
└── styles/
    └── global.css        # Tailwind + custom styles/animations
public/
└── favicon.svg           # Site favicon
```

## Design System

### Colors (defined in global.css @theme)
- `--color-orange`: #FF4C24 (primary accent)
- `--color-charcoal`: #0D0D0D (dark/text)
- `--color-cream`: #FAFAF8 (background)
- `--color-gray`: #6B6B6B (secondary text)

### Typography
- Display: `font-display` (Syne) - headlines, buttons
- Body: `font-body` (DM Sans) - paragraphs, labels

### Custom Classes
- `.btn-primary` - Orange CTA button with hover effects
- `.btn-outline` - Outlined button variant
- `.hover-lift` - Card lift effect on hover
- `.corner-accent` - Orange corner border decoration
- `.price-tag` - Gradient text for pricing
- `.orange-underline` - Animated underline on hover

## Commands

```bash
npm run dev      # Start dev server (localhost:4321)
npm run build    # Build for production
npm run preview  # Preview production build
```

## Configuration

### Formspree
Replace `YOUR_FORM_ID` in `src/pages/index.astro` (line ~249) with your actual Formspree form ID.

### Content Updates
- **Services/Pricing**: Edit the `services` array in `src/pages/index.astro`
- **Stats**: Update numbers in the hero stats panel
- **Contact email**: Update in the contact section
- **Social links**: Update href values in footer

## Conventions

- Keep the bold, premium aesthetic - avoid generic/safe design choices
- Maintain orange (#FF4C24) as the primary accent color
- Use Syne for headlines/buttons, DM Sans for body text
- Prefer CSS animations over JavaScript when possible
- Mobile-first responsive design
