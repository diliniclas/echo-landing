# echo-landing

Echo's public marketing site — plain HTML/CSS, no build step, no framework. Reuses In&Out
Consulting's design system (`css/chrome.css`, `buttons.css`, `forms.css`, copied verbatim from
`Reply/docs/design-system-export/`) for speed; `css/site.css` holds only page-specific layout.

## Pages
- `index.html` — landing page (hero, features, how-it-works, pricing, final CTA)
- `terms.html`, `privacy.html`, `impressum.html` — legal pages. **All three contain
  `[placeholder]`-marked gaps (Bright Peak GmbH's registered address, HRB number, support
  email, etc.) and have NOT been reviewed by a lawyer — fill in real details and get counsel's
  sign-off before this goes live and is used to take real payments.**

## Preview locally
Just open `index.html` in a browser — no server or build step needed. (Anchor links between
pages assume they're served from the same directory, so a simple local file open works fine.)

## Deploy
Static files only — works on Vercel, Netlify, Cloudflare Pages, or GitHub Pages with zero
config. Point the chosen host's custom domain at `echotxt.ai` (already owned/controlled — used
for the Azure AD tenant set up in docs/GO-TO-MARKET.md Phase 1).

## Download links
All CTAs point at `https://github.com/diliniclas/echo-releases/releases/latest` rather than a
specific installer filename, so they keep working as new versions ship — no landing-page edit
needed per release.
