# Jess DeFranco Portfolio

## About
Portfolio website for Jess DeFranco, a San Francisco-based contemporary dancer and dance educator. Built with Astro (static site).

## Tech
- **Astro 5** — static site generator, zero JS except mobile nav toggle
- **Vanilla CSS** — custom properties for theming, no framework
- **Deployed on** Cloudflare Pages (`npm run build`, output `dist`)

## Commands
- `npm run dev` — local dev server at localhost:4321
- `npm run build` — production build to `dist/`
- `npm run preview` — preview production build

## Structure
```
src/
  layouts/BaseLayout.astro       # Shared HTML shell, meta, nav + footer
  components/
    Nav.astro                    # Fixed nav with mobile hamburger
    Footer.astro                 # Social links, floral divider, copyright
    Hero.astro                   # Reusable page hero
    FloralDivider.astro          # SVG floral accent (mint + gold)
  pages/
    index.astro                  # Home — split hero with photo, intro, featured work, collaborators
    about.astro                  # First-person bio, portrait, training, downloadable resume
    work.astro                   # 19 performances (2018–2025), real images for recent 3
    teaching.astro               # PLACEHOLDER — no real content yet
    gallery.astro                # PLACEHOLDER — no real photos yet
    contact.astro                # Contact form + email/social links
  styles/global.css              # Design tokens, reset, typography
public/
  images/                        # Real photos (hero, portrait, 3 production images)
  jess-defranco-resume.pdf       # Downloadable resume
rsc/                             # Source assets (not deployed, gitignored)
  images/                        # Original photos
  jess-resume.pdf                # Original resume PDF
```

## Design
- **Palette**: Off-white `#faf9f6` bg, mint `#a8d5ba` accents, golden `#c9a84c` accent, charcoal `#2d2d2d` text
- **Typography**: Playfair Display (headings), Inter (body) via Google Fonts
- **Floral divider**: Minimal SVG with mint leaves + gold bloom, used on home and footer
- **Work entries without photos**: Gold uppercase title card instead of empty placeholder

## Real Content Sources
- **Bio/Resume**: `rsc/jess-resume.pdf` — BA Dance + Asian American Studies from SF State, training at LINES Ballet and Pacific Ballet Academy
- **Linktree**: https://linktr.ee/jessdefrancodance
- **Instagram**: @small_jess95
- **LinkedIn**: https://www.linkedin.com/in/jessica-defranco-b503b015b/
- **Show pages**: kularts-sf.org (Burden of Proof), alyssaevemitchel.com (Endure)
- **Email**: jessicadefranco95@gmail.com

## Still Needs
- **Teaching page**: has placeholder content, needs real class/workshop info from Jess
- **Gallery page**: has placeholder grid, needs real photos
- **Contact form**: HTML form exists but not wired to a backend (Formspree, Netlify Forms, etc.)
- **More work images**: only 3 of 19 performances have real photos
- **Video reel**: no video content yet — add when available
