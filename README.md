# Project Meridian — Final Credit Diligence Package · Rev 2 (tabbed edition, open)

`index.html` is the full document served directly — no client-side encryption
or password gate in this edition.

This revision carries the sixteen-section tab navigation (Overview → Appendix)
and eight exhibits across Brand Health, Merchandising, Trade & Retail Media,
and Supply Chain. Content is unchanged from Rev 2 — no new findings raised;
every exhibit traces to a section or register number already in the package.

## Deploy

    vercel --prod

from this folder (or connect the GitHub repo in the Vercel dashboard — no
build step, framework preset "Other"). `vercel.json` sets the security
headers: noindex, no-referrer, no-store, frame-deny, and a locked-down CSP.

Since the document itself is unencrypted, access control now rests entirely
on the deployment layer: enable **Vercel Deployment Protection** (password or
Vercel Authentication) if the URL should not be world-readable.
