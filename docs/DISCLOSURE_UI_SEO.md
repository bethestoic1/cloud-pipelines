# Disclosure placement: UI & SEO best practice

## Goal

Stay **FTC- and DigitalOcean-compliant** (disclosure at top of page) while keeping the site **appealing and conversion-focused**. The disclosure should be visible and clear without dominating the layout or hurting trust.

---

## What we use (recommended pattern)

- **One short line** at the top of the main content (directly under the header or at top of container).
- **No box** — no background panel or heavy border. A subtle bottom border or no border keeps it readable but low-visual-weight.
- **Muted color, small type** (e.g. 0.8rem) so it reads as “standard transparency” rather than a warning.
- **Copy:** “Advertising disclosure: We may receive commissions from [recommended providers / providers below / providers linked on this page].” Optional: “This supports our independent [audit/comparisons].”
- **Keep footer disclosure** on key pages (e.g. index) for redundancy; primary compliance is satisfied by the **top** placement.

---

## Why this works

### UI / conversion

- **Above the fold** — Satisfies “top of page” without a big block. First thing users see after the brand is still the value prop (headline, audit, comparison).
- **Trust, not alarm** — Short, neutral wording reads as transparency. No alert styling (red, yellow, big icons), so it doesn’t feel like a warning.
- **Minimal real estate** — One line + thin separator uses little space; CTAs and main content stay dominant. On mobile, no big disclosure box pushing the form or table down.
- **2026 pattern** — Common on comparison and review sites: one clear line at top, full legal in footer or “Disclosure” expandable. Users who care can read it; others scroll to content.

### SEO

- **Content hierarchy** — H1 and first paragraph stay the main topical signal. A long disclosure block as first content can dilute relevance; a single line keeps “FinOps audit” / “Cloudways vs Kinsta vs DigitalOcean” as the clear focus.
- **EEAT** — Transparent monetization supports trust and “experience” signals. Brief, professional disclosure is a positive, not a negative.
- **Crawlability** — One line is still in the DOM and visible; no need to hide or collapse for SEO. If you later add an expandable “Full disclosure,” keep a short visible line at top for compliance.

### Compliance

- **FTC** — “Clear and conspicuous”: visible without scrolling on typical viewports, readable (contrast, size). One line at top meets this.
- **DigitalOcean** — “Top of the page”: same placement satisfies their requirement. No need for a large box.

---

## What to avoid

- **Footer-only** — DO explicitly disallows; commissions at risk.
- **Heavy box** — Large panel with border/background competes with headline and CTAs; can hurt conversion and feel “salesy.”
- **Tiny or low-contrast text** — Could be seen as hiding the disclosure; keep at least 0.8rem and sufficient contrast.
- **Vague wording** — “This site is supported by its audience” is okay as supplement; primary line should clearly say you may receive **commissions** from **recommended** providers/links.

---

## Optional enhancements (if you want to test)

- **Expandable “Disclosure”** — Top line: “Advertising disclosure: We may earn from recommended providers. [Details ▼].” Expandable section has full text. Still compliant if the summary line is clear and at top.
- **Inline in subtitle** (comparison only) — e.g. “Comparing managed performance… We may earn from links below.” Slightly more integrated; ensure it’s unmissable on mobile.
- **Sticky slim bar** — One line in a thin top bar that stays visible on scroll. Use only if it doesn’t cover CTAs or feel intrusive on small screens.

Current implementation uses the **minimal top line** (no box, subtle separator). It keeps you compliant and keeps the layout clean and conversion-friendly.
