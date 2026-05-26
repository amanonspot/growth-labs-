# SPOTO Growth Labs Website Plan

## Objective
Build and ship a high-converting landing page for SPOTO Growth Labs that clearly communicates services, pricing, credibility, and conversion paths.

## Current Baseline
- Static one-page `index.html` with premium visual design and animations.
- Sections included: hero, trust strip, services bento, pricing, process, and final CTA.

## Implementation Roadmap

### Phase 1: Foundation (Immediate)
- Keep current landing page as base in `index.html`.
- Replace placeholders before launch:
  - WhatsApp number (`wa.me` URL)
  - Phone number in contact row
  - Any example brand/client names if needed
- Update footer year dynamically or set to current year.

### Phase 2: Conversion Infrastructure
- Add lead capture form (name, phone, business type, monthly ad budget).
- Connect form submissions to one endpoint:
  - Option A: Netlify Forms
  - Option B: Google Sheets webhook/Apps Script
  - Option C: CRM webhook (HubSpot/Zoho)
- Track critical events:
  - `book_call_click`
  - `whatsapp_click`
  - `pricing_cta_click`
  - `scroll_75`

### Phase 3: Performance and SEO
- Add metadata:
  - Open Graph tags
  - Twitter card tags
  - Canonical URL
- Add `sitemap.xml`, `robots.txt`, and basic schema markup (`Organization`, `Service`).
- Optimize:
  - Compress assets if external media is introduced
  - Respect reduced-motion preferences
  - Remove heavy effects on low-end/mobile devices if needed

### Phase 4: Trust and Sales Readiness
- Replace placeholder logos with real client logos/testimonials.
- Add 2–3 short case studies with:
  - Industry
  - Ad spend
  - Leads generated
  - ROI/ROAS lift
- Add FAQ section for common objections (pricing, timeline, guarantee, minimum budget).

### Phase 5: Deployment and Iteration
- Deploy to Netlify or Vercel with custom domain.
- Set up analytics dashboard (GA4 + Search Console + ad platform attribution).
- Run A/B tests:
  - Hero headline variants
  - CTA copy
  - Pricing section placement and layout

## Recommended Next Build Tasks
1. Replace all placeholders with production contact details.
2. Add a real lead form and submission backend.
3. Add analytics events for CTA buttons.
4. Perform mobile UX pass and launch.

## Repo Notes
- Primary landing page: `index.html`
- Planning document: `PROJECT_PLAN.md`
