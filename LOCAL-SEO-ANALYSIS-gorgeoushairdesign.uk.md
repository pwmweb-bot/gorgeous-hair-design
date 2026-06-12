# Local SEO Analysis — gorgeoushairdesign.uk

**Date:** 5 May 2026  
**Analyst:** Claude (seo-local skill)  
**URL:** https://www.gorgeoushairdesign.uk/

---

## Local SEO Score: 64/100

| Dimension | Weight | Score | Notes |
|-----------|--------|-------|-------|
| GBP Signals | 25% | 12/25 | Maps link only, no embed or widget |
| Reviews & Reputation | 20% | 16/20 | Strong ratings, multi-platform |
| Local On-Page SEO | 20% | 17/20 | Strong — Droitwich in title + H1, NAP visible, service pages built |
| NAP Consistency & Citations | 15% | 9/15 | FreeIndex website wrong; Bing/Apple unclaimed |
| Local Schema Markup | 10% | 7/10 | Correct HairSalon type; minor gaps (no logo, no Monday hours, no @id) |
| Local Link & Authority | 10% | 3/10 | No chamber, press, or community signals detectable |
| **Total** | 100% | **64/100** | Good foundations; authority signals are the gap |

---

## Business Type

**Brick-and-Mortar** — Physical address visible in footer, H2 sections, schema, and contact page. Google Maps link present. No service-area-only language.

---

## Industry Vertical

**Beauty — Hair Salon** (correct schema subtype: `HairSalon`)  
Secondary services: Body Piercing, Aesthetics (lashes, brows, cryotherapy, mole mapping)

Industry-specific note: A business offering aesthetics/medical-adjacent services (mole mapping, cryotherapy) may benefit from adding a secondary `MedicalClinic` or `HealthAndBeautyBusiness` schema alongside `HairSalon` for the aesthetics arm — but this is optional and schema validators accept multiple types.

---

## 1. GBP Signals — 12/25 (Partial)

| Signal | Status | Notes |
|--------|--------|-------|
| Google Maps link on page | ✅ | Links to correct GBP listing |
| Google Maps embed (iframe) | ❌ | Only a text link — no geographic signal reinforcement |
| Reviews widget / embed | ❌ | Reviews mentioned (4.9, 62) but no live GBP widget |
| Business hours on page | ✅ | Full hours table visible |
| GBP posts active | Unknown | Cannot assess from website |
| Photos/video on GBP | Unknown | Cannot assess from website |
| Google Verified badge | Unknown | Cannot assess from website |
| GBP primary category | Unknown | Inferred: Hair Salon — appropriate |
| GBP link not to homepage | ⚠️ | Schema `sameAs` and link goes to GBP — check that GBP website URL points to a non-homepage page (Sterling Sky Diversity Update) |

**Action needed:** Add a lazy-loaded Google Maps iframe to `contact.html`. This gives geographic signal reinforcement without hurting page speed.

---

## 2. Reviews & Reputation — 16/20 (Strong)

| Signal | Status | Notes |
|--------|--------|-------|
| Google reviews: 62 at 4.9★ | ✅ | Well above 4.5 threshold (31% of consumers filter here) |
| Fresha reviews: 324 at 5.0★ | ✅ | Excellent — schema says 297 (needs updating to 324) |
| Star rating display on page | ✅ | Hero section shows ratings from both platforms |
| AggregateRating in schema | ✅ | Present — but value is 297, Fresha now shows 324 |
| Review recency | Unknown | Cannot determine last review date from website |
| Owner responses visible | Unknown | Cannot assess from website |
| Third-party platforms | ✅ | Fresha + Google (2 platforms) |
| Yell listing | ✅ | Present |
| Yelp UK listing | ❌ | No UK listing found |
| Review gating detected | ❌ (clean) | No pre-screening detected |
| 18-day review velocity | Unknown | Monitor actively — rankings cliff if 3+ weeks without new review |

**Key risk:** 62 Google reviews is good but growing this number matters most for local pack. Fresha reviews (324) don't directly feed Google rankings. Encourage every happy client to leave a Google review.

---

## 3. Local On-Page SEO — 17/20 (Strong)

| Signal | Status | Notes |
|--------|--------|-------|
| Title tag includes Droitwich | ✅ | "... Hair, Aesthetics & Piercing \| Droitwich" |
| H1 includes city + service | ✅ | "Award-Winning Hair Salon in Droitwich Spa." |
| NAP visible in footer/page | ✅ | Full address + phone in footer |
| Click-to-call tel: link | ✅ | `tel:01905799055` + individual stylist numbers |
| Contact form present | ✅ | On contact.html with service selection |
| Google Maps embed | ❌ | Link only — no iframe embed |
| Dedicated service landing pages | ✅ | balayage, hair-colour, dermal-filler, body-piercing built |
| Inner pages have Droitwich in titles | ✅ | services, about, contact, team pages updated |
| Internal linking (hub-and-spoke) | ✅ | Footer links to all pages + landing pages |

**Note:** The "Monday: Beautician Only" hours are not in the schema but do appear on the website. Clarify whether the salon is open Monday for hair or not — if beautician services run on Monday, add a Monday `openingHoursSpecification` entry.

---

## 4. NAP Consistency & Citations — 9/15 (Partial)

### NAP Comparison Across Sources

| Field | Website HTML | Schema | Fresha | FreeIndex | Yell |
|-------|-------------|--------|--------|-----------|------|
| Name | Gorgeous Hair Design | Gorgeous Hair Design | Gorgeous Hair Design | Gorgeous Hair Design | Gorgeous Hair Design & Gorgeous Piercings |
| Street | 20 Ombersley Street West | 20 Ombersley Street West | 20 Ombersley Street West | 20 Ombersley Street West | 20 Ombersley Street West |
| City | Droitwich Spa | Droitwich Spa | **Droitwich** (missing Spa) | **Droitwich** (missing Spa) | Droitwich |
| County | Worcestershire | Worcestershire | — | Worcestershire | WR9 (postcode only) |
| Postcode | WR9 8HZ | WR9 8HZ | WR9 8HZ | WR9 8HZ | WR9 |
| Phone | 01905 799055 | +441905799055 | Not listed | 01905 79**** (masked) | — |
| Website | gorgeoushairdesign.uk | gorgeoushairdesign.uk | Not listed | **facebook.com/GoRgEoUsHaIr20** ❌ | — |

### ⚠️ Critical NAP Issues

1. **FreeIndex website field** shows `facebook.com/GoRgEoUsHaIr20` instead of `gorgeoushairdesign.uk` — this means FreeIndex is passing no link equity to the site and may confuse data aggregators. **Fix: Update FreeIndex profile website URL.**

2. **Name inconsistency on Yell:** Listed as "Gorgeous Hair Design & Gorgeous Piercings" — different from the canonical name used everywhere else. Minor, but worth aligning.

3. **"Droitwich Spa" vs "Droitwich"** — Fresha and FreeIndex drop "Spa". Ideally consistent, but Google understands both. Lower priority.

### Citation Presence

| Directory | Status | Notes |
|-----------|--------|-------|
| Google Business Profile | ✅ | 62 reviews, linked from site |
| Fresha | ✅ | 324 reviews, 5.0★ — strong |
| Facebook | ✅ | Active page |
| Yell.com | ✅ | Listed (name slightly different) |
| FreeIndex | ✅ | Listed but wrong website URL — fix needed |
| Groupon | ✅ | Listed |
| Local and Loyal | ✅ | Listed |
| Instagram | ✅ | Active |
| TikTok | ✅ | Active |
| Bing Places | ❌ | **Not confirmed** — powers ChatGPT, Copilot, Alexa |
| Apple Business Connect | ❌ | **Not confirmed** — usage doubled to 27% (BrightLocal 2026) |
| Yelp UK | ❌ | No UK listing found |
| Thomson Local | ❌ | Not found |
| Data aggregators | ❌ | Data Axle, Foursquare, Neustar not confirmed |

---

## 5. Local Schema Markup — 7/10 (Good)

### Current Implementation (index.html)

```json
{
  "@type": "HairSalon",  ← ✅ Correct subtype
  "name": "Gorgeous Hair Design",
  "alternateName": "...",
  "geo": { "latitude": 52.2672351, "longitude": -2.1553533 },  ← ✅ 7 decimal places
  "aggregateRating": { "ratingValue": "5.0", "reviewCount": "297" },  ← ⚠️ Fresha now shows 324
  "openingHoursSpecification": [ Tue–Sat ],  ← ⚠️ Monday missing
  "foundingDate": "2006",  ← ✅
  "areaServed": [...],  ← ✅
  "hasOfferCatalog": {...},  ← ✅
  "sameAs": [ Facebook, Instagram, TikTok, Fresha ]  ← ✅ (add Yell URL too)
}
```

### Schema Issues

| Issue | Severity | Fix |
|-------|----------|-----|
| `logo` property missing | Medium | Add `"logo": "https://www.gorgeoushairdesign.uk/images/logo.png"` |
| `@id` missing | Medium | Add `"@id": "https://www.gorgeoushairdesign.uk/#business"` |
| Monday not in `openingHoursSpecification` | Low | Add Monday entry — even if hours say "Beautician Only", add the hours for that service |
| `reviewCount` outdated (297 vs 324) | Low | Update to current Fresha count periodically |
| Yell not in `sameAs` | Low | Add Yell URL to sameAs array |
| Services.html schema | ✅ | HairSalon + BreadcrumbList + ItemList — well implemented |

### Ready-to-Use Fix (add to index.html schema)

```json
"@id": "https://www.gorgeoushairdesign.uk/#business",
"logo": {
  "@type": "ImageObject",
  "url": "https://www.gorgeoushairdesign.uk/images/logo.png"
},
```
And add to `openingHoursSpecification`:
```json
{ "@type": "OpeningHoursSpecification", "dayOfWeek": "Monday", "opens": "09:00", "closes": "17:00" }
```
(adjust hours to match actual beautician hours)

---

## 6. Local Link & Authority Signals — 3/10 (Low)

| Signal | Status | Notes |
|--------|--------|-------|
| Chamber of Commerce | ❌ | No mention on site |
| BBB / trade body | ❌ | N/A for UK; equivalent: FSB or Guild of Hairdressers |
| Local press mentions | ❌ | Not detectable |
| Community sponsorships | ❌ | Not detectable |
| "Best of" list placements | ❌ | #1 AI visibility factor (Whitespark 2026) |
| Groupon listing | ✅ | Some authority |
| Industry directories | ⚠️ | Fresha strong; Yell present |

This is the biggest gap and the hardest to fix quickly. Without backlinks, ranking competitively for "hairdressers Droitwich" vs established local competitors is very difficult.

---

## Top 10 Prioritised Actions

### 🔴 Critical

**1. Claim and optimise Bing Places**  
ChatGPT does not access GBP — it sources from Bing's index, Yelp, and directories. Bing Places feeds ChatGPT, Copilot, and Alexa. Claim at: bingplaces.com. NAP must exactly match website.

**2. Fix FreeIndex website URL**  
Currently shows `facebook.com/GoRgEoUsHaIr20` instead of `gorgeoushairdesign.uk`. This sends incorrect data through the directory network. Log in to FreeIndex and update the website field to `https://www.gorgeoushairdesign.uk`.

**3. Claim Apple Business Connect**  
Apple Maps usage has doubled to 27% (BrightLocal 2026). Claim at: register.apple.com/business. Complete all fields with exact NAP.

### 🟠 High

**4. Add Google Maps iframe embed to contact.html**  
Replace the text link with a lazy-loaded `<iframe>` embed. This provides geographic signal reinforcement for crawlers. Use `loading="lazy"` to protect page speed.

**5. Grow Google reviews to 100+**  
You have 324 Fresha reviews but only 62 Google reviews. Google reviews directly affect local pack ranking. Fresha reviews do not. Implement a post-appointment SMS or email asking specifically for a Google review. Aim for the 18-day minimum velocity (at least one new review per 18 days to avoid ranking cliff).

**6. Update schema reviewCount (297 → 324)**  
Fresha now shows 324 reviews. Update in `index.html` and `services.html`. Set a monthly reminder to sync this number.

### 🟡 Medium

**7. Add `@id` and `logo` to schema**  
Both properties improve entity disambiguation for Google's Knowledge Graph. `@id` creates a stable identifier. `logo` improves GBP integration. Ready-to-use fix shown above.

**8. Submit to data aggregators**  
Data Axle, Foursquare, and Neustar/TransUnion distribute business data downstream to hundreds of directories. A one-time submission multiplies citation coverage significantly.

**9. Update Yell listing name to match canonical name**  
Yell shows "Gorgeous Hair Design & Gorgeous Piercings" vs your canonical "Gorgeous Hair Design". Log in to Yell and align the name.

**10. Build one local authority link per month**  
Target: Droitwich Chamber of Commerce, Worcestershire County tourism directory, The Guild of Hairdressers (industry body), local Droitwich newspaper (Droitwich Advertiser). One quality local link per month for 6 months will materially improve non-branded rankings.

---

## AI Search Visibility (Local Context)

ChatGPT converts local visitors at 15.9% vs Google organic at 1.76% — making AI visibility increasingly important. For this business, the biggest AI visibility gaps are:

- **Bing Places not claimed** — ChatGPT sources local data from Bing
- **No "best of" list placements** — #1 AI visibility factor per Whitespark 2026
- **Yelp UK listing absent** — Yelp is a primary source for ChatGPT local recommendations

Run `/seo geo https://www.gorgeoushairdesign.uk/` for a full AI search visibility audit including llms.txt, passage citability scoring, and brand mention analysis.

---

## What This Analysis Could NOT Assess

| Gap | What It Means | Tool to Fill It |
|-----|---------------|-----------------|
| Real-time local pack position | Where the salon ranks in Google Maps for "hairdressers droitwich" | BrightLocal, Whitespark, or DataForSEO geo-grid |
| GBP Insights data | Impressions, clicks, calls, direction requests from GBP | Google Business Profile dashboard |
| Review velocity trend | Whether reviews are coming in consistently (18-day rule) | Review monitoring tool or manual GBP check |
| Domain Authority / DR | Link authority vs competitors | Moz, Ahrefs, or Semrush |
| Comprehensive backlink profile | Who links to the site | Ahrefs, Semrush (only 1 TikTok backlink confirmed via GSC) |
| GBP photo count and recency | Photo engagement affects direction requests | GBP dashboard |
| Competitor comparison | How the salon stacks up against nearby competitors | Local rank tracking tool |
