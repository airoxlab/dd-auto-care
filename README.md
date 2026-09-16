# D & D Auto Care

Single-page website for D & D Auto Care — a mobile mechanic and car detailing service in Sandusky County, northwest Ohio. Repairs, maintenance and diagnostics at the customer's location (everything except transmission internals and body work), plus interior and exterior detailing. Open weekday evenings until 9 PM and from 7 AM on weekends.

- **Phone (call/text):** (419) 601-4587
- **Area:** Sandusky County, Ohio (service-area business — no public street address listed)
- **Rating:** 5.0 on Google

## Structure

- `index.html` — the complete site (self-contained CSS, no build step, no framework)
- `img/` — three job photos from the Google Business Profile
- `screenshots/` — per-section renders with the navbar visible (light theme), `screenshots/dark/` for dark theme, plus full-page desktop and mobile captures

Open `index.html` in a browser, or deploy the folder as-is to any static host (GitHub Pages, Netlify, etc.).

## Design

Midnight blue with a wax-shine gold accent, taken from the mirror-black Cadillac in the business's own hero photo; the light theme resolves to warm cream and bronze rather than a flat inversion. Type is Sora (display) / Outfit (body). Palette is fully tokenised on `:root` and redefined for light mode under both `@media (prefers-color-scheme: light)` and `:root[data-theme="light"]`, so the page follows the OS theme and an explicit toggle. A "D&D" monogram stands in for a logo, since the business has no logo mark published anywhere.

Seven sections: hero, services, maintenance (mobile mechanic scope: routine maintenance, brakes/steering/suspension, engine/electrical/cooling, plus what is not covered and how a mobile job works), work gallery, hours, reviews, and a booking form (department selector: detailing / mobile repair & maintenance / both; composes the request into a text message to the shop's number, since no email is published) — plus a strip and footer. The hours table is treated as the lead differentiator (weekend rows highlighted), because evening and weekend availability is the most distinctive verifiable fact about this business.

## Data sources

The mechanical scope — "everything to a vehicle besides transmission internals and cosmetic work" — was stated directly by the owner (Sep 2026); the maintenance section lists common jobs within that scope. Everything else on this page comes from the business's public **Google Business Profile**: name, phone number, category, opening hours, wheelchair-accessibility note, 5.0 rating, the customer review and the owner's reply, and the three photos.

The business was identified by matching the phone number (419) 601-4587 against the Google Maps listing — several unrelated Ohio businesses share the "D & D Auto" name, and all were excluded. Location was derived from the listing's map coordinates (41.389, -83.362 → Madison Township, Sandusky County) since no street address is published; the site therefore says "Sandusky County" rather than naming a town.

No prices, packages, turnaround times, guarantees, certifications, years in business, or owner biography were added — none are published. The review is quoted verbatim and shown in full, including the owner's reply, rather than being padded out with invented testimonials. There is no website, Facebook page, or Yelp listing for this business.
