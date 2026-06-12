# LOCAL SEO ANALYSIS — gorgeoushairdesign.uk
**Audit Date:** 1 May 2026
**Primary URL Audited:** https://www.gorgeoushairdesign.uk/services.html
**Analyst:** Claude Sonnet 4.6 (Local SEO Agent)
**Cross-referenced pages:** /, /about.html, /contact.html, /team.html, /testimonials.html

---

## LOCAL SEO SCORE: 58 / 100

| Dimension | Weight | Raw Score | Weighted Score | Notes |
|-----------|--------|-----------|----------------|-------|
| GBP Signals | 25% | 52/100 | 13.0 | Maps link/embed present; no confirmed GBP posts, photos or Q&A evidence on-site |
| Reviews & Reputation | 20% | 82/100 | 16.4 | Strong Fresha volume; Google count is low; no aggregateRating on inner pages |
| Local On-Page SEO | 20% | 62/100 | 12.4 | Good titles/H1s; no meta desc on services; no dedicated sub-service pages; one H1 "Our Services" is generic |
| NAP Consistency & Citations | 15% | 50/100 | 7.5 | Perfect on-site consistency; near-zero confirmed Tier 1 citations |
| Local Schema Markup | 10% | 60/100 | 6.0 | Correct HairSalon type on homepage; missing on services/about/team; Monday hours absent from schema |
| Local Link & Authority Signals | 10% | 18/100 | 1.8 | TikTok only confirmed external link; no local directory backlinks found |
| **TOTAL** | **100%** | | **57.1** | Rounded to **58 / 100** |

---

## 1. BUSINESS TYPE DETECTION

**Detected: Brick-and-Mortar**

Signals detected:
- Full street address visible in footer, contact page, and JSON-LD schema on every audited page
- Google Maps iframe embed present on contact.html
- Google Maps place link with coordinates (52.2672351, -2.1553533) present site-wide in footer social links
- "Visit Us" CTA in footer with physical address
- No service area language, no "we come to you" language
- Directions link present via Google Maps URL

---

## 2. INDUSTRY VERTICAL DETECTION

**Detected: Hair Salon (Beauty / Personal Care)**

Primary vertical signals:
- Cuts, colour, balayage, wedding hair — core hairdressing services
- "HairSalon" schema type used correctly on homepage and contact page
- Staff directory with named stylists, booking per stylist

Secondary vertical signals (extending beyond pure hairdresser):
- Aesthetics: anti-wrinkle, dermal filler, skin boosters, vitamin injections, micro needling
- Beauty: lashes, brows, waxing
- Piercing: ear, facial, oral, body — implant-grade titanium

**Implication:** The GBP primary category is almost certainly "Hair Salon." Secondary categories should include "Beauty Salon," "Piercing Shop" or "Spa" — these cannot be confirmed without live GBP access. The breadth of services (aesthetics, piercing) means the business is competing in multiple sub-niches, each needing its own SEO treatment. This is currently unaddressed on the website.

---

## 3. NAP CONSISTENCY AUDIT

### Source Comparison Table

| Source | Name | Street Address | Locality | Postcode | Phone |
|--------|------|---------------|----------|----------|-------|
| index.html (visible footer) | Gorgeous Hair Design | 20 Ombersley Street West | Droitwich Spa, Worcestershire | WR9 8HZ | 01905 799055 |
| index.html JSON-LD schema | Gorgeous Hair Design | 20 Ombersley Street West | Droitwich Spa | WR9 8HZ | +441905799055 |
| services.html (visible footer) | Gorgeous Hair Design | 20 Ombersley Street West | Droitwich Spa, Worcestershire | WR9 8HZ | 01905 799055 |
| services.html JSON-LD | (No LocalBusiness schema present) | — | — | — | — |
| contact.html (visible body) | Gorgeous Hair Design | 20 Ombersley Street West | Droitwich Spa | WR9 8HZ | 01905 799055 |
| contact.html JSON-LD schema | Gorgeous Hair Design | 20 Ombersley Street West | Droitwich Spa | WR9 8HZ | +441905799055 |
| about.html (visible footer) | Gorgeous Hair Design | 20 Ombersley Street West | Droitwich Spa, Worcestershire | WR9 8HZ | 01905 799055 |
| team.html (visible footer) | Gorgeous Hair Design | 20 Ombersley Street West | Droitwich Spa, Worcestershire | WR9 8HZ | 01905 799055 |
| testimonials.html (visible footer) | Gorgeous Hair Design | 20 Ombersley Street West | Droitwich Spa, Worcestershire | WR9 8HZ | 01905 799055 |
| Fresha listing | Gorgeous Hair Design | 20 Ombersley Street West | Droitwich | — | Not visible |
| GBP (via Maps URL) | Gorgeous Hair Design Piercings and Aesthetics Droitwich | — | Droitwich | — | Not confirmed |

### NAP Flags

**FLAG 1 — Name mismatch between schema and GBP:**
The JSON-LD on index.html uses `"alternateName": "Gorgeous Hair Design Piercings and Aesthetics"` which matches the GBP listing name visible in the Maps URL. However the primary `"name"` field in schema is "Gorgeous Hair Design" while the GBP listing name appears to be "Gorgeous Hair Design Piercings and Aesthetics Droitwich." This is a soft inconsistency — the GBP name includes the location town which is non-standard but common.

**FLAG 2 — Phone format:**
Visible HTML uses local format `01905 799055`; JSON-LD uses international format `+441905799055`. This is technically correct and consistent in meaning, but some citation scrapers may flag it. Fresha did not expose a phone number in its listing view.

**FLAG 3 — Monday hours absent from schema:**
Monday is "Beautician Only" — a non-standard state that is correctly omitted from `openingHoursSpecification` (which only lists Tue–Sat). However, the visible footer and contact page do show Monday: Beautician Only. This is not an error but it means the schema does not reflect Monday availability at all, which may cause the GBP hours panel to show "Closed Monday" if Google reads schema over GBP data.

**Overall NAP consistency: GOOD on-site, UNKNOWN off-site.** All five pages present identical visible NAP with no discrepancies in street address, postcode, or phone.

---

## 4. LOCAL SCHEMA MARKUP VALIDATION

### Homepage (index.html)

**Schema type:** `HairSalon` — CORRECT. (HairSalon is a valid Schema.org subtype of LocalBusiness/BeautySalon. It is the correct type for a hair and beauty salon.)

| Property | Status | Value / Notes |
|----------|--------|---------------|
| @type | PASS | HairSalon |
| name | PASS | "Gorgeous Hair Design" |
| alternateName | PASS | "Gorgeous Hair Design Piercings and Aesthetics" |
| url | PASS | https://www.gorgeoushairdesign.uk |
| telephone | PASS | "+441905799055" |
| email | PASS | hello@gorgeoushairdesign.uk |
| address (PostalAddress) | PASS | Street, locality, region, postcode, country all present |
| geo (GeoCoordinates) | PASS | lat: 52.2672351, lng: -2.1553533 — 7 decimal places, exceeds 5-decimal minimum |
| openingHoursSpecification | PARTIAL | Tue–Sat covered. Monday ("Beautician Only") absent. Sunday absent (correct — closed). |
| aggregateRating | PASS | ratingValue: 5.0, reviewCount: 297, bestRating: 5 |
| sameAs | PASS | Facebook, Instagram, TikTok, Fresha URLs included |
| priceRange | PASS | "££" |
| hasOfferCatalog | PASS | 8 services listed |
| logo | ISSUE | Points to hero-home.jpg, not a logo file. Should be a dedicated logo image URL. |
| image | PASS | hero-home.jpg |
| foundingDate | MISSING | Recommended — business established 2006 |
| currenciesAccepted | MISSING | Minor omission |
| areaServed | MISSING | Recommended for local signals |

**BreadcrumbList:** Present on homepage — single item (Home). Correct.

### Services Page (services.html)

**LocalBusiness / HairSalon schema:** ABSENT. The services page carries only:
1. A BreadcrumbList (Home > Services) — PASS
2. An ItemList of 8 services — PASS

**Issue:** No LocalBusiness entity schema on the page most likely to be discovered via service-keyword searches. Google cannot extract NAP, geo, or hours from this page independently. Every page that may land in SERPs for local queries should carry the full HairSalon entity block.

### Contact Page (contact.html)

**Schema type:** `HairSalon` — CORRECT.

| Property | Status | Notes |
|----------|--------|-------|
| name | PASS | "Gorgeous Hair Design" |
| telephone | PASS | "+441905799055" |
| email | PASS | hello@gorgeoushairdesign.uk |
| address | PASS | Full PostalAddress |
| geo | PASS | 52.2672351, -2.1553533 |
| openingHoursSpecification | PARTIAL | Same issue as homepage — Monday absent |
| contactPoint | PASS | ContactPoint with telephone and availableLanguage |
| aggregateRating | MISSING | Not present on contact page schema |
| sameAs | MISSING | Not present on contact page schema |
| url | PASS | https://www.gorgeoushairdesign.uk |

**BreadcrumbList:** Present (Home > Contact) — PASS.

### About, Team, Testimonials Pages

No JSON-LD schema blocks detected on about.html, team.html, or testimonials.html. These pages would benefit from at minimum a BreadcrumbList and ideally a condensed HairSalon entity block.

**Testimonials page gap:** The testimonials.html page has no `aggregateRating` schema. This is the page most likely to rank for "[salon name] reviews" queries and the one where structured review data would add the most value.

### Schema Issue Summary

| Issue | Severity | Pages Affected |
|-------|----------|---------------|
| HairSalon entity absent | High | services.html, about.html, team.html, testimonials.html |
| aggregateRating absent | High | contact.html, services.html, testimonials.html |
| logo property points to hero image not logo | Medium | index.html |
| Monday hours not in schema | Medium | index.html, contact.html |
| foundingDate absent | Low | index.html |
| sameAs absent | Low | contact.html |
| areaServed absent | Low | all pages |

---

## 5. GBP SIGNALS ASSESSMENT

| Signal | Status | Evidence |
|--------|--------|---------|
| Google Maps place link | DETECTED | Full Maps URL with Place ID in footer on all pages |
| Google Maps embed iframe | DETECTED | contact.html has embedded Maps iframe |
| Geo coordinates | DETECTED | 52.2672351, -2.1553533 in schema and Maps URLs |
| Review count cited (Google) | DETECTED | "62 reviews on Google" on homepage hero |
| Review rating cited (Google) | DETECTED | "4.9" on homepage |
| Review link to Google | DETECTED | href links to Google Maps review filter |
| GBP posts evidence | NOT DETECTED | No post content or publication dates on site |
| GBP Q&A evidence | NOT DETECTED | No Q&A content referenced |
| GBP photos evidence | PARTIAL | Site has strong image library but no GBP photo gallery widget |
| GBP booking button | NOT ASSESSED | Requires live GBP panel view |
| GBP primary category | NOT CONFIRMED | Likely "Hair Salon" based on schema type; cannot confirm without GBP access |
| Google review widget/badge | NOT PRESENT | Reviews are hardcoded HTML, not a live Google widget |

**GBP Name Concern:** The Maps URL uses the name "Gorgeous Hair Design Piercings and Aesthetics Droitwich." Google historically penalises keyword-stuffed business names. "Piercings and Aesthetics" is a descriptor, not a legal trading name, and including "Droitwich" as a city modifier in the business name is against GBP guidelines. This warrants review.

**Review velocity concern:** Google shows 62 reviews. The site does not surface when the most recent Google review was left. Per the Sterling Sky 18-day rule, if no Google review has been posted in the past 3 weeks, rankings may be suppressed. With only 62 reviews total (vs 297 on Fresha), Google review velocity is likely the primary ranking constraint and should be the #1 active priority.

---

## 6. REVIEW HEALTH SNAPSHOT

| Metric | Fresha | Google |
|--------|--------|--------|
| Rating | 5.0 | 4.9 |
| Review count | 297 | 62 |
| Platform type | Booking platform (closed ecosystem) | Public search signal |
| On-site display | Yes — homepage hero, testimonials page | Yes — homepage hero |
| aggregateRating schema | Yes (homepage only) | (same schema block — 297/5.0 referenced) |
| Response rate | Unknown (not observable without platform access) | Unknown |
| Velocity (last 18 days) | Unknown | Unknown |

**Critical observation:** The aggregateRating schema on the homepage uses Fresha data (297 reviews, 5.0). This is technically valid but Google's guidelines state that aggregateRating should reflect ratings the site itself hosts and controls, or should clearly reference the source. Google may or may not pass rich snippet eligibility for this. More importantly: there is no mention of the 62 Google reviews in any schema block. Google gives significantly more weight to its own review ecosystem for local pack rankings.

**Review split problem:** 297 reviews on Fresha vs 62 on Google represents an 83% review leakage rate to a closed platform. Fresha reviews do not feed local pack signals. The business needs a structured programme to convert booking completions into Google reviews.

**Sample review quality:** Reviews sourced on-site are positive and specific (naming stylists, mentioning specific services). This is a strong quality signal. No negative reviews or owner responses are visible on the site — response rate on Google is unknown but should be actively managed.

---

## 7. CITATION PRESENCE — TIER 1 DIRECTORIES

| Directory | Status | Notes |
|-----------|--------|-------|
| Google Business Profile | CONFIRMED (indirect) | Maps listing exists — visible via Maps URLs/embed |
| Fresha | CONFIRMED | Active booking presence; sameAs in schema |
| Facebook | CONFIRMED | Active page at /GoRgEoUsHaIr20 |
| Instagram | CONFIRMED | Active at /hair_piercings_aesthetics_ |
| TikTok | CONFIRMED | Active at @gorgeoushairandpiercings; known external backlink |
| Yell.com | UNCONFIRMED | 403 error — could not verify. Priority citation for UK businesses |
| Yelp UK | UNCONFIRMED | 403 error — less critical for UK but worth checking |
| Treatwell | UNCONFIRMED | No result returned in search — likely not listed |
| Thomson Local | NOT CHECKED | UK Tier 1 directory — unknown status |
| Scoot | NOT CHECKED | UK directory — unknown status |
| Checkatrade | NOT CHECKED | Less relevant for hair salons |
| BBB | NOT APPLICABLE | US directory — not relevant for UK business |
| Bing Places | NOT CHECKED | Should mirror GBP if synced |
| Apple Maps | NOT CHECKED | Increasingly important for iOS users |
| Cylex UK | NOT CHECKED | Mid-tier UK directory |
| FreeIndex | NOT CHECKED | UK salon-relevant directory |
| Wahanda/Treatwell | LIKELY ABSENT | Treatwell search returned no result for this business |
| Nextdoor | NOT CHECKED | Hyper-local; relevant for Droitwich Spa community |

**Citation gap assessment:** The business has strong presence on social/booking platforms but appears to have minimal presence on traditional UK business directories. Yell.com alone (which returned a 403, suggesting the listing may exist but could not be confirmed) reaches millions of UK searchers. The Whitespark 2026 ranking study identifies citations as 3 of the top 5 AI visibility factors — this gap is a meaningful ranking suppressor.

**Priority citation targets for hair/beauty in UK:**
1. Yell.com (confirm and optimise)
2. Treatwell (key platform for salon discovery)
3. Thomson Local
4. Bing Places (sync from GBP)
5. Apple Maps Connect
6. Scoot
7. FreeIndex
8. Nextdoor (Droitwich Spa neighbourhood)

---

## 8. LOCAL ON-PAGE SEO EVALUATION

### Title Tags

| Page | Title Tag | Assessment |
|------|-----------|------------|
| index.html | "Gorgeous Hair Design — Hair, Aesthetics & Piercing \| Droitwich" | GOOD — brand + services + geo. 58 chars. |
| services.html | "Hair & Beauty Services in Droitwich \| Gorgeous Hair Design" | GOOD — service keyword + geo + brand. 59 chars. |
| contact.html | "Contact Our Droitwich Hair Salon \| Gorgeous Hair Design" | GOOD — geo + service type + brand. |
| about.html | "About Us \| Droitwich Hair Salon Since 2006 \| Gorgeous Hair Design" | GOOD — geo + trust signal + brand. |
| team.html | "Meet Our Team \| Gorgeous Hair Design, Droitwich" | ACCEPTABLE — could include service noun. |
| testimonials.html | "Client Reviews \| Gorgeous Hair Design, Droitwich" | ACCEPTABLE — "reviews" is the keyword. |

### Meta Descriptions

| Page | Meta Description | Assessment |
|------|-----------------|------------|
| index.html | "Expert hair salon in Droitwich Spa — cuts, colour, balayage, aesthetics & piercing since 2006. 5.0★ from 297 reviews. Book online today." | EXCELLENT — geo, services, social proof, CTA. |
| services.html | "Full range of hair, aesthetics, lashes, brows, waxing and body piercing services at Gorgeous Hair Design, Droitwich. View our complete price list and book today." | GOOD — comprehensive service list. |
| contact.html | "Contact Gorgeous Hair Design, 20 Ombersley Street West, Droitwich Spa WR9 8HZ. Call 01905 799055 or book online via Fresha. Opening hours and directions." | EXCELLENT — full NAP in meta description is strong for local. |
| about.html | "Learn about Gorgeous Hair Design, Droitwich's trusted hair salon since 2006. Meet our passionate team of stylists, beauticians and piercers dedicated to making you look and feel amazing." | GOOD. |
| testimonials.html | "Read real reviews from Gorgeous Hair Design clients in Droitwich. Rated 5.0 on Fresha with 297 reviews and 4.9 on Google. See what our clients say about our stylists." | GOOD — review count as social proof in snippet. |
| team.html | Not confirmed from source read | UNKNOWN — no meta description seen in head section read. |

### H1 Tags

| Page | H1 | Assessment |
|------|----|------------|
| index.html | "Where Great Hair Begins." | WEAK for local SEO — no geo, no service keyword. Purely brand/emotional. |
| services.html | "Our Services" | WEAK — generic. Should include geo or primary service. |
| contact.html | "Get in Touch" | ACCEPTABLE — contact intent is clear. |
| about.html | "About Us" | WEAK — no geo, no differentiator. |
| team.html | "Meet the Team" | ACCEPTABLE for its purpose. |
| testimonials.html | "What Our Clients Say" | ACCEPTABLE. |

**H1 gap:** The two highest-traffic pages (homepage, services) have H1 tags optimised for brand feel rather than local search. The homepage H1 "Where Great Hair Begins." contains no local keyword. The services page H1 "Our Services" is entirely generic. Neither would help Google understand the local relevance of these pages for queries like "hairdresser Droitwich" or "hair salon Droitwich."

### Canonical Tags

All six audited pages have correct self-referencing canonical tags. No canonicalisation issues detected.

### Service Page Architecture

**Major structural gap:** The site has one flat services page (/services.html) covering all services with anchor links. While the anchor links (#cuts, #balayage, #antiwrinkle, etc.) are a sensible UX pattern, they do not create individually indexable pages for each service category.

Per Whitespark 2026 rankings research, dedicated service pages are the #1 local organic factor and #2 AI visibility factor. Currently the site has:
- 0 dedicated pages for "balayage droitwich"
- 0 dedicated pages for "dermal filler droitwich"
- 0 dedicated pages for "body piercing droitwich"
- 0 dedicated pages for "hair colour droitwich"

Each of these represents a separate ranking opportunity with distinct commercial intent. GSC data showing 392 impressions for "hairdressers droitwich" with low CTR suggests the site surfaces for hair queries but loses clicks — dedicated landing pages with optimised titles and meta descriptions would improve CTR and likely improve rankings.

### Internal Linking

The footer on every page includes anchor links to all 12 service sections on services.html. This is a reasonable internal linking pattern. However:
- No internal links from services to team members offering those services
- No internal links from testimonials to services mentioned in reviews
- About page does not link to any specific service pages
- Team page individual stylist entries do not link to their service specialisms

### Booking Flow

Primary CTA throughout site is "Book Now" which opens a modal. The modal correctly deep-links to Fresha per-stylist. However the CTA on the services page footer reads "Book Now" and links to contact.html (not Fresha), introducing an extra friction step for users who have decided to book after viewing services.

---

## 9. LOCAL LINK & AUTHORITY SIGNALS

**Confirmed external backlinks:** 1 (TikTok profile)

**Assessment:** Critically thin link profile. For a business established 18–20 years, the expected natural link profile would include:
- Local press (Droitwich Advertiser, Worcestershire-area news sites)
- Wedding directories (Hitched, Bridebook — the site offers bridal hair)
- Local business association links (Droitwich Business Association, Worcestershire Chamber)
- Supplier or product brand links (e.g., colour brands listing salons)
- Fresha press/blog mentions
- Historic Wix/previous platform backlinks (may still exist — not checked)

The indexing situation (1 of 8 pages indexed as of early May 2026, sitemap just submitted) means the site is effectively brand new in Google's eyes despite the domain age and trading history. Link acquisition is essential to accelerate re-indexing and establish authority.

---

## 10. MULTI-LOCATION ASSESSMENT

**Not applicable.** This is a single-location business. No location page quality audit required.

---

## 11. INDEXING STATUS NOTE

Per provided business context, only 1 of 8 pages is confirmed indexed as of early May 2026, with the sitemap submitted recently. The sitemap.xml (confirmed present at /sitemap.xml) contains 7 URLs with correct lastmod dates (2026-04-30). This means:

- Google is likely still crawling and processing all pages
- Rankings data (impressions, CTR) will be volatile during this period
- Any schema or on-page fixes should be implemented immediately, before Google's indexing crawl completes
- The priority is ensuring all pages pass Core Web Vitals and have no technical crawl barriers

The robots.txt file is present (confirmed in file listing). Its content was not read — recommend verifying it does not accidentally disallow any pages.

---

## 12. TOP 10 PRIORITISED ACTIONS

### CRITICAL

**Action 1 — Launch a Google review acquisition programme (immediately)**
With 62 Google reviews vs 297 Fresha reviews, the business is severely underweight on the signal that matters most for local pack rankings. The Sterling Sky 18-day rule means any gap in Google review velocity risks ranking suppression. Implement a post-appointment SMS or email sequence asking for a Google review (link direct to the Google review form). Target: 5+ new Google reviews per month minimum.

**Action 2 — Add HairSalon schema to services.html, about.html, team.html, testimonials.html**
The services page is the most commercially important page on the site and has no LocalBusiness entity schema. Add the same HairSalon block from index.html (minus aggregateRating if concerned about guideline compliance, but including name, address, geo, telephone, url, openingHoursSpecification, sameAs) to all four missing pages. This ensures Google can extract structured local signals regardless of which page it lands on.

**Action 3 — Verify and optimise Yell.com listing**
Yell.com is the primary UK equivalent of Yelp for local citation authority. A listing here (with correct NAP matching the site exactly: "Gorgeous Hair Design," "20 Ombersley Street West," "Droitwich Spa," "WR9 8HZ," "01905 799055") provides a high-authority citation backlink and surfaces the business in Yell search results.

### HIGH

**Action 4 — Create dedicated service landing pages for priority keywords**
Build individual pages for the highest-value service/location combinations. Priority order:
1. /balayage-droitwich (or /balayage.html) — competitive, high-intent
2. /hair-colour-droitwich (or /colour.html) — core hairdressing query
3. /dermal-filler-droitwich — aesthetic services, high value per appointment
4. /body-piercing-droitwich — unique differentiator, low local competition

Each page needs a unique H1, 300+ words of original content, localised copy, its own schema, and internal links from the main services page.

**Action 5 — Fix H1 tags on homepage and services page**
Homepage H1 "Where Great Hair Begins." should incorporate a local keyword. Suggested: "Droitwich's Favourite Hair Salon — Where Great Hair Begins." Or restructure so the emotional tagline is an H2/eyebrow and H1 carries geo + service intent. Services page H1 "Our Services" should become "Hair, Aesthetics & Piercing Services in Droitwich" or similar.

**Action 6 — Audit and clean up GBP business name**
The GBP listing name appears to be "Gorgeous Hair Design Piercings and Aesthetics Droitwich." Per Google's guidelines, the business name should match the real-world trading name — keyword descriptors and city names are against policy. The listing may be at risk of suspension or a spam report from a competitor. Recommended GBP name: "Gorgeous Hair Design" — with services and location expressed through categories and the address field respectively.

**Action 7 — List on Treatwell**
Treatwell is the dominant UK salon booking and discovery platform, equivalent in reach to Fresha but with stronger SEO authority. A Treatwell listing with complete NAP, photos, services and pricing creates a high-authority citation, a new booking channel, and another review source. The business is currently absent from Treatwell.

### MEDIUM

**Action 8 — Add aggregateRating schema to testimonials.html and fix logo property**
The testimonials page is the natural home for aggregateRating structured data and will likely compete for "[business name] reviews" queries. Add a condensed HairSalon block with aggregateRating. Separately, update the `logo` property in index.html schema to point to the actual logo/brand mark file rather than the hero image.

**Action 9 — Build local citations on Bing Places, Apple Maps, Thomson Local, Scoot**
Submit to Bing Places for Business (which populates Bing local and Cortana), Apple Maps Connect (iOS users — significant share), and UK business directories Thomson Local, Scoot, FreeIndex, and Cylex UK. Each submission should use identical NAP: "Gorgeous Hair Design," "20 Ombersley Street West," "Droitwich Spa," "WR9 8HZ," "01905 799055."

**Action 10 — Add areaServed and foundingDate to schema; fix services CTA**
Add `"areaServed": "Droitwich Spa"` (or an array including nearby towns: Droitwich, Worcester, Bromsgrove, Kidderminster) to the HairSalon schema to explicitly signal the geographic service area. Add `"foundingDate": "2006"` as a trust signal. Fix the services page bottom CTA — change "Book Now" link from contact.html to the Fresha booking URL or booking modal trigger to reduce friction.

### LOW (Backlog)

- Verify robots.txt does not disallow any pages
- Add Monday ("Beautician Only") handling — consider adding a special hours note or removing the "Closed" implication by adding a custom hours note
- Pursue wedding directory citations (Hitched, Bridebook) given bridal hair offering
- Consider Nextdoor business listing for Droitwich Spa hyper-local community
- Investigate and recover any historic backlinks from previous Wix site
- Add team member Person schema to team.html for individual stylist authority
- Meta description for team.html — confirm whether present and optimise if missing

---

## 13. LIMITATIONS DISCLAIMER

The following could not be assessed without paid tools or authenticated access:

- **Live GBP panel data:** Primary category, secondary categories, GBP posts, GBP Q&A, GBP photo count, GBP booking button status, GBP attributes (wheelchair access, appointment required, etc.) — requires Google Business Profile Manager or a DataForSEO/BrightLocal API call.
- **Google review velocity:** The date of the most recent Google review is not visible without live GBP access. This is critical given the 18-day ranking cliff rule.
- **Google review response rate:** Cannot confirm without live GBP access.
- **Local pack position:** Real-time local pack ranking for "hairdressers droitwich" and related queries requires DataForSEO `google_local_pack_serp` or similar tool. The proximity variable (55.2% of ranking variance per Search Atlas ML study) means rankings vary significantly by searcher location.
- **Yell.com citation status:** Yell.com returned a 403 error; a paid tool (BrightLocal, Whitespark) would confirm existence and NAP accuracy.
- **Full backlink profile:** Ahrefs or Semrush required for complete link audit.
- **GSC full data:** Only the single "hairdressers droitwich" data point was provided. Full keyword impression data would reveal additional ranking opportunities.
- **Core Web Vitals / PageSpeed:** Not assessed — requires Google PageSpeed Insights or CrUX data.
- **Mobile usability:** Responsive CSS is present but live device testing was not performed.
- **GBP Spam/Competitor analysis:** No competitor GBP audit was performed. Droitwich Spa is a small market — assessing competitor GBP optimisation levels would clarify the effort required to achieve top-3 local pack position.

---

*Report generated: 1 May 2026 | gorgeoushairdesign.uk Local SEO Agent Audit*
