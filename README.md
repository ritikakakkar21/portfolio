# Ritika Kakkar - Portfolio Website

Static, dependency-free portfolio site: a home page plus eight deep-dive case studies.

## Files

- `index.html` - home: hero, impact snapshot, case index, approach, toolkit, about, contact
- `case-01-ai-seo-programmatic-growth-system.html` - case 01: AI SEO + Programmatic Growth System
- `case-02-90-day-gtm-recovery-ga4-slack-bot.html` - case 02: 90-Day GTM Recovery + GA4-to-Slack Bot
- `case-03-andaman-love-travel-site.html` - case 03: Travel Site: From AI Filler to 460% Click Growth
- `case-04-eleczo-ecommerce-platform.html` - case 04: E-commerce Platform: 238K Clicks and 115% Growth
- `case-05-riversoft-local-business.html` - case 05: Local Business: 77 to 781 Clicks in Four Months
- `case-06-brandshark-multi-client-agency.html` - case 06: Multi-Client Agency: 500%+ Organic Growth with CRO
- `case-07-sunanda-global-waterproofing.html` - case 07: Waterproofing: Page 1 in One Month
- `case-08-sportstech-eu-market-migration.html` - case 08: Six EU Markets, One Migration Window
- `style.css` - design system (light + dark mode, responsive)
- `main.js` - mobile nav, scroll reveal, footer year

## Run locally

Open `index.html` in any browser, or serve the folder:

```
python3 -m http.server 8080
```

## Publish

- **Netlify / Vercel:** drag the folder into the dashboard, or connect a repo. No build step needed.
- **GitHub Pages:** push the folder to a repo and enable Pages on the branch root.
- **Custom domain:** point DNS at the host and add canonical/OG URLs once the domain is live.

## Editing content

All copy lives in `build_site.py` (the generator) in the `CASES` list. Edit and rerun:

```
python3 build_site.py
```

You can also edit the HTML directly - the markup is plain and semantic.

## Notes

- Dark mode follows the visitor's OS setting via `prefers-color-scheme`.
- Charts are inline SVG, so they inherit theme colours and scale without image assets.
- Person and Article JSON-LD are embedded for search and AI-search visibility.
