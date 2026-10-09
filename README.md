# Portfolio — Muhammad Radwan

Personal portfolio site for a **Database & Power BI Developer**: SQL Server data
modelling, ETL pipelines, and executive dashboards.

**Live:** <https://muhammad-redwan.github.io>

---

## About this site

A single static page — no framework, no build step, no dependencies. Plain HTML
and CSS with ~20 lines of vanilla JavaScript for the scroll-spy navigation.
It loads as three requests plus fonts.

It presents three dashboard case studies drawn from real client engagements in
commercial real estate across the Gulf:

| Project | Focus | Stack |
| --- | --- | --- |
| Collections & Receivables Control | MTD collections, invoicing, aging, net outstanding | Power BI · DAX |
| Leasing Performance & Pipeline | Lead-to-contract funnel, MOU stages, specialist ranking | Power BI · Fabric |
| Commercial Portfolio Reporting | Occupancy, rent & service income, budget vs. actual | SQL · ETL · SSRS |
| Lease Expiry & Holdover Tracking | Expiry banding, holdover pipeline, leases at risk | Power BI · DAX |

## A note on the data

**Every dashboard image is anonymised.** Client names, organisational branding,
staff names and tenant entities have been replaced with fictional equivalents
before publication. The dashboards shown are my own design and modelling work;
the organisations they were built for are not identified, and no client-owned
figures are presented as attributable to any named party.

Dashboard pages containing personally identifiable information — individual
tenant names, lease records, named debtor balances — were excluded from this
portfolio entirely rather than redacted.

## Structure

```
.
├── index.html                  # the whole site
├── collection.webp             # dashboard screenshots (1400px, WebP)
├── leasing.webp
├── commercial.webp
├── expiry.webp
├── og-image.png                # social share card (1200×630)
├── Muhammad-Radwan-CV.pdf      # linked from the Experience section
└── .nojekyll                   # serve files as-is on GitHub Pages
```

## Running it locally

No tooling required — open `index.html` in a browser.

To serve it over HTTP instead (closer to production, and makes relative paths
behave identically):

```bash
python -m http.server 8000
# then open http://localhost:8000
```

## Deploying

Published with **GitHub Pages** from the `main` branch
(*Settings → Pages → Source: Deploy from a branch*).

The absolute URLs required for social previews (`canonical`, `og:image`,
`og:url`, `twitter:image`) are already set in `index.html`. If the site ever
moves, those four tags and the link at the top of this README need updating —
LinkedIn and WhatsApp will not resolve relative paths.

For a custom domain, add a `CNAME` file containing the bare domain and point
the DNS records at GitHub Pages.

## Contact

- **Email:** MRedwan214@gmail.com
- **LinkedIn:** [/in/mredwan214](https://www.linkedin.com/in/mredwan214/)
