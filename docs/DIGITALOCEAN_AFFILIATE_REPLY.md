# DigitalOcean Affiliate: Validation & Reply

## Validation summary

### Where the “cost below 2000” DO content appears

- The **“Audit Result: Efficiency Optimization Identified”** block (DigitalOcean recommendation + “Claim Your $200”) is **not in this repo**. It is shown when the user selects **“Under $2,000”** in the Tally form on the homepage.
- That content is almost certainly:
  - **Either** a **Tally thank-you / result screen** (hosted by Tally), or  
  - **Or** a **redirect** to a URL on cloudpipelines.com that we don’t yet have in the repo.

**Action:** If the DO recommendation is on a **Tally-hosted** thank-you screen, add the same advertising disclosure at the **top** of that screen in Tally’s form settings (e.g. custom thank-you message). If it redirects to a **cloudpipelines.com** page, that page must have a top-of-page disclosure (we’ve already added it to `index.html` and `success.html`).

### Which site actually needs the change (in this repo)

- **Only CloudPipelines (cloudpipelines.com)** is in this repo and has affiliate/DO placements today.
- **Learn Solana, Code Pipelines, CryoVault, Tech Walkthroughs** are separate codebases; when DO links go live there, each **page that contains a DO link** must have the disclosure at the **top** of the page (same pattern as CloudPipelines).

### What was changed on CloudPipelines

- **Top-of-page** “Advertising disclosure” added on every page that contains affiliate or DO recommendations:
  - **index.html** – Homepage with audit form and compare link to DO; disclosure directly under the header.
  - **comparison.html** – Cloudways vs Kinsta vs DigitalOcean table (and future DO CTA); disclosure at top of container.
  - **success.html** – Audit result with Cloudways/Kinsta (and any DO path); disclosure at top of body.
  - **cloudways/index.html** – Cloudways blueprint (mentions DO); disclosure at top of body.
- Footer disclosures are kept where they still add value; DO’s requirement is satisfied by the **top** placement.

---

## Sample pages (for DigitalOcean’s request)

Use these when they ask “sample pages on each site where the links will go”:

| Site | Sample pages where DO links will appear |
|------|------------------------------------------|
| **CloudPipelines** | https://cloudpipelines.com/ (audit tool; DO recommendation when “Estimated Monthly Cloud Spend” = Under $2,000), https://cloudpipelines.com/comparison.html (DO in comparison table and future CTA), https://cloudpipelines.com/success.html (audit result CTAs), https://cloudpipelines.com/finops-audit-2026.html (links to compare/DO), https://cloudpipelines.com/cloudways/ (managed layer on DO). |
| **Learn Solana** | DO will appear on pages covering RPC node hosting or dev/staging (e.g. hosting / infrastructure guides). Specific URLs to be shared once those pages are published. |
| **Code Pipelines** | DO will appear in DevEx/tooling content and dev/staging hosting recommendations. Sample URLs when those pages go live. |
| **CryoVault Solutions** | DO where relevant for backup or compliant infrastructure. Sample URLs when live. |
| **Tech Walkthroughs** | DO in hosting and deployment software comparisons. Sample URLs when live. |

---

## Draft reply to DigitalOcean

You can send something like this (adjust tone/names as you like):

---

**Subject:** Re: DigitalOcean affiliate – sample pages & disclosure placement

Hi Adam,

Thank you for the clarification.

**Sample pages (where DigitalOcean links will appear):**

- **CloudPipelines (https://cloudpipelines.com/)**  
  - Homepage: https://cloudpipelines.com/ — audit tool; when users select “Under $2,000” for estimated monthly cloud spend, the audit result recommends DigitalOcean (e.g. “Claim Your $200”) and links to DO.  
  - Comparison: https://cloudpipelines.com/comparison.html — DigitalOcean is in the comparison table and will have a direct CTA once we’re in the program.  
  - Audit result: https://cloudpipelines.com/success.html — post-audit recommendations (including paths that lead to DO).  
  - Guides: https://cloudpipelines.com/finops-audit-2026.html and https://cloudpipelines.com/cloudways/ — references and links to DO where relevant.

- **Learn Solana (https://learnsolana.io/)**  
  DO will be listed as a hosting option for RPC nodes or dev/staging. I’ll share specific page URLs once those pieces are published.

- **Code Pipelines, CryoVault Solutions, Tech Walkthroughs**  
  DO will be used in comparison sections, setup guides, and resource pages as described in my previous email. I’ll send specific sample URLs as each site’s relevant pages go live.

**Advertising disclosure – top of page:**

I’ve updated **CloudPipelines** so that every page that contains affiliate or DigitalOcean recommendations now has an **advertising disclosure at the top of the page** (directly under the header or at the top of the main content), not only in the footer. Wording used: “Advertising disclosure: We earn commissions when you shop through the links below.”

For **Learn Solana, Code Pipelines, CryoVault Solutions, and Tech Walkthroughs**, I will apply the same pattern: on any page that includes a DigitalOcean link or recommendation, the disclosure will appear at the **top** of the page. I’ll ensure this is in place before driving traffic to those DO links.

If you need different wording or placement (e.g. exact distance from first affiliate link), please let me know and I’ll adjust.

Best regards,  
Stoic

---

## Checklist before sending

- [ ] Confirm where the “Under $2,000” DO result is shown (Tally screen vs. redirect). If Tally: add disclosure at top of that screen in Tally.
- [ ] Deploy CloudPipelines so live site shows top-of-page disclosures on index, comparison, success, cloudways.
- [ ] Optionally add 1–2 direct DO sample URLs for other sites if any pages are already live with DO placeholders.
