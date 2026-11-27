# Fargo Meridian — Completion Checklist

Source: https://fargomeridian.com
Repository: pixelrisemedia1/fargomeridian.com
Status: IN PROGRESS — unchecked items are not verified complete.
Rule: Check an item only after comparing against the source or testing the public deployment and recording evidence in the commit/issue/notes.

## 1. Routes and source pages
- [ ] Home
- [ ] About/company routes (extract exact list)
- [ ] All catalog/category routes
- [ ] Every individual product/detail route (extract complete list from source)
- [ ] Contact/inquiry routes and any quote/account routes

## 2. Images, video, documents and other media
- [ ] assets/logo.webp — verify exact mark, clearspace and responsive variants
- [ ] assets/aluminium.webp and assets/aluminium-sheet.webp — map to source category/product pages and distinguish exact products
- [ ] assets/copper-bars.webp and assets/copper-wire.webp — map each to its source item and crop
- [ ] assets/metal-ingots.webp and assets/metal-wire.webp — map each to source items
- [ ] assets/scrap-metal.webp — verify source page, grade/context and crop
- [ ] assets/steel-bars.webp, assets/steel-coils.webp, assets/steel-plates.webp, assets/steel-sheets.webp, assets/steel-tubes.webp — map each file to the exact catalog item
- [ ] Inventory all source product photos, variants, diagrams, specification sheets, certificates, icons, banners and downloadable documents; compare against current 12 listed product images

## 3. Site-specific content and functionality
- [ ] Extract and implement the full source product sitemap; no catalog item may be omitted or sent to a generic placeholder
- [ ] Match each product name, grade, material, size, finish, standards, packaging, availability and inquiry path to source
- [ ] Build category navigation, product search/filter/sort, product cards, detail pages, related items and pagination if present
- [ ] Verify image-to-product mapping; ensure visually similar materials are not mislabeled
- [ ] Recreate About/company history, sourcing, logistics, quality, sustainability and certifications only when supported by source
- [ ] Implement quote/contact inquiry with required fields, confirmation and actual authorized delivery
- [ ] Verify all product documents, certificates, tables and downloadable specifications are correct and current

## Shared production acceptance checks
- [ ] Verify source route inventory against the live source and archived export; record date and evidence for each route.
- [ ] Compare each page at matching desktop, tablet and mobile viewports; record unresolved visual differences.
- [ ] Audit every image, logo, icon, video, poster, caption, document and embedded asset; verify local/independent URL, dimensions, crop, alt text and successful public loading.
- [ ] Confirm no Base44 media URLs, SDK/runtime, API, auth, storage, form or database dependency remains in the copied site or its public requests.
- [ ] Verify every navigation destination, CTA, form, menu, carousel, modal, filter and document link; no dead controls or fake success states.
- [ ] Verify accurate title/description/social metadata, favicon, headings, canonical URL plan, robots/sitemap when appropriate and not-found behavior.
- [ ] Check keyboard use, focus visibility, contrast, labels, alt text, reduced-motion, mobile touch targets and responsive reflow.
- [ ] Check spelling, dates, claims, addresses, phone numbers, email addresses, legal content and document versions against approved source material.
- [ ] Check browser console, failed network requests, broken links, 404s, image loading and performance on desktop/mobile.
- [ ] Verify GitHub Actions deployment succeeds; open the live deployed copy in a fresh session and directly load/refresh every route.
- [ ] Record final verification date, deployed commit, public URL, and any remaining limitation. Custom domain/DNS is intentionally deferred until requested.

## Verified audit notes — 2026-11-27
- [x] Inspected source homepage: it identifies a Singapore trading company handling metals, minerals, plastics and soft commodities; includes About, Global Networks, Contact and product navigation.
- [x] Confirmed source homepage has a logo plus a 12-slide hero carousel; its source images are Base44-hosted and the copy has 12 product-material image files/candidate slide images.
- [x] Direct request to the copy's `/Home` path returned GitHub Pages 404 during this check.
- [ ] Map every source slide image and all catalog image variants to the correct local files; the current file list alone does not prove exact asset matching.
- [ ] Build and verify all product category/product pages, company routes, correct base paths and inquiry interactions.

### Fargo Meridian image verification detail
- [x] Source homepage audit captured a Base44-hosted logo and 12 hero-carousel slide images.
- [ ] Compare the 12 source slides to the 12 local product/material candidates one by one; current filenames do not prove that the hero carousel imagery matches.
- [ ] Inventory product photos separately from hero slides and map every catalog image/document to a specific source product.

## Repository-level checks
- [x] Inspected the repository file tree and confirmed the root homepage file and deployment workflow path.
- [x] Compared local asset filenames against references in the root homepage HTML.
- [x] Scanned the root homepage HTML for Base44, Supabase, and Unsplash URL references: none found in `index.html`.
- [ ] Scan every repository file, document, metadata field and deployed network request for any remaining third-party/Base44 runtime or media dependency.
- [ ] Confirm all listed local assets are source-matched and used in the appropriate page; unused files are not removed until their role is understood.
- [ ] Verify the latest deployment for this checklist commit and smoke-test every route and asset after deployment.

## Fargo Meridian source inventory (checked 2026-11-27)
- [x] Confirmed source header routes: Home, About Us, Products and Contact Us; homepage also links to About, GlobalNetworks, Contact and Products.
- [x] Confirmed the homepage describes a Singapore-based trader in metals, minerals, plastics and soft commodities; has an animated/clickable 12-slide hero and company/network/contact sections.
- [x] Captured 13 homepage images: logo plus twelve Base44-hosted carousel photos.
- [ ] Inspect About, GlobalNetworks, Contact and Products destinations; enumerate all product categories/SKUs and establish which source images are hero slides versus product detail photos.
