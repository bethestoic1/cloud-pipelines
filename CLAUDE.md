# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

CloudPipelines (cloudpipelines.com) is a **static HTML site** hosted on GitHub Pages. It serves as a FinOps audit lead generation and managed cloud hosting affiliate site. There is no build system, no package manager, no backend, and no database.

**Deployment:** Push to `main` → GitHub Pages auto-deploys to cloudpipelines.com.

## Architecture

Pure HTML/CSS/JS files — no framework, no bundler, no transpilation. Forms submit externally to Tally.so. Affiliate links use UTM parameters for tracking.

```
/
├── index.html                  # Homepage + embedded Tally audit form
├── comparison.html             # Cloudways vs Kinsta vs DigitalOcean table
├── success.html                # Post-audit recommendations + CTAs
├── infrastructure.html         # Solana/bare metal hosting (Cherry, Latitude.sh)
├── cloudways/index.html        # Dedicated Cloudways landing page
├── [guide pages].html          # SEO content: FinOps, AWS, GCP, CDN guides
├── docs/                       # Compliance documentation
│   ├── DISCLOSURE_UI_SEO.md    # FTC/DigitalOcean disclosure requirements
│   └── DIGITALOCEAN_AFFILIATE_REPLY.md
├── sitemap.xml / sitemap.txt
├── robots.txt
├── llms.txt                    # AI bot summary
└── CNAME                       # cloudpipelines.com
```

## Compliance Requirements

**Every page containing affiliate or DigitalOcean links MUST have a top-of-page disclosure.** Footer-only disclosures violate DigitalOcean's affiliate terms.

Required disclosure pattern:
```html
<p class="disclosure-top" role="complementary">
  Advertising disclosure: We earn commissions when you shop through the links below.
</p>
```

Pages requiring disclosure: `index.html`, `comparison.html`, `success.html`, `cloudways/index.html`

See [docs/DISCLOSURE_UI_SEO.md](docs/DISCLOSURE_UI_SEO.md) for full compliance details.

## Design System

Two theme variants used consistently:

**Dark theme** (`index.html`, `success.html`, `infrastructure.html`, `best-managed-cloud-2026.html`):
- `--bg: #0f172a` | `--accent: #38bdf8` | `--text: #e0e6ed`

**Light theme** (`comparison.html`, `cloudways/index.html`, guide pages):
- `--bg: #f9fafb` | `--text: #1f2937`

Typography uses `clamp()` for fluid scaling. Buttons: minimum 48px touch targets. All pages support `prefers-reduced-motion` and have focus-visible outlines.

## SEO Conventions

Every page includes:
- `<meta name="description">`, OG tags, Twitter Card tags
- `<link rel="canonical">`
- JSON-LD schema (FAQPage or Product where appropriate)

Use supportable, hedged phrasing (e.g., "around 30% cloud waste per industry reports") — avoid unverified absolute claims.

## Copy/Content Standards

- No secrets, API keys, tokens, or env files — all affiliate URLs and Tally form IDs are intentionally public
- Affiliate links include UTM parameters
- Tally form embed ID: `448bpr` (on `index.html`)
