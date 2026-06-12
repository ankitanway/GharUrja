# AGENT.md

## Project: GharUrja

**GharUrja** is an India-focused rooftop solar decision platform that helps homeowners understand solar, estimate savings, check subsidy eligibility, and discover trusted and verified local installers.

The business goal is not to build a generic solar blog, a simple calculator, or a directory of random vendors. The business goal is to become a trusted solar advisory and lead-generation platform, starting with one region first and expanding state by state.

---

## Core Business Goal

Build a platform that:

1. Attracts homeowners searching for solar information.
2. Educates them with clear and useful tools.
3. Qualifies their intent through smart forms and calculations.
4. Shows them trusted and verified installers.
5. Generates revenue from qualified leads, installer partnerships, and advertising.

---

## Target Users

### 1) Homeowners
People who want to:
- Reduce electricity bills
- Understand rooftop solar
- Check subsidy eligibility
- Estimate cost and savings
- Find reliable installers

### 2) Solar Installers
Businesses that want:
- Better-qualified residential leads
- More site visits
- More installation bookings
- A simple way to receive and manage leads

---

## Initial Market Strategy

### Phase 1 Focus
Start with **one Indian state or one city cluster first**.

Recommended starting point:
- Bihar

Why:
- Lower competition than national keywords
- Strong local SEO opportunity
- Easier to build trust region by region
- Easier to recruit installers and collect testimonials

### Expansion Strategy
Do **not** create separate websites for each state.

Use one main domain and create state-specific sections, such as:
- /bihar/
- /jharkhand/
- /uttar-pradesh/

This keeps SEO authority in one place and makes scaling easier.

---

## Business Model

### Revenue Stream 1: Google AdSense / Advertising
Use display ads and content monetization for informational traffic.

Best ad-supported pages:
- Solar guides
- Subsidy articles
- FAQ pages
- State-specific informational pages
- Calculator result pages with high traffic

Important:
- Ads must not damage trust or user experience.
- Keep the site clean and readable.
- Ads are secondary to the core user experience.

### Revenue Stream 2: Qualified Lead Generation
Capture leads from users who want installer quotes.

### Revenue Stream 3: Installer Partnerships
Charge installers for:
- Qualified leads
- Premium visibility
- Monthly subscriptions
- Verified profile placement

### Revenue Stream 4: Software Tools for Installers
Add later:
- Lead dashboard
- Quote management
- Follow-up tools
- Customer tracking

---

## Product Positioning

GharUrja is:

- A solar decision platform
- A trusted advisory tool
- A lead-generation system
- A local solar education hub
- An ad-supported informational content platform

GharUrja is **not**:
- A generic solar directory
- A hard-selling marketplace
- A solar equipment seller
- A clone of government portals
- A vague AI wrapper with no real utility

---

## Product Principles

### 1) Trust First
- Never exaggerate savings
- Never promise guaranteed subsidies
- Always show assumptions clearly
- Always encourage verification on official government portals
- Only show trusted and verified installers

### 2) Simplicity First
- Design for normal homeowners, not engineers
- Avoid jargon unless explained
- Keep forms short and clear
- Mobile-first experience is mandatory

### 3) Lead Quality First
- Do not collect random traffic leads
- Only forward users who show real intent
- A lead must have enough information to be useful to installers

### 4) Local Relevance
- State-specific solar guidance matters
- Use location-aware content when possible
- Local SEO is a major growth lever

### 5) Build for Revenue
- Every major feature should support traffic, trust, qualification, advertising, or monetization
- Avoid features that look good but do not help the business

---

## MVP Features

### 1) Solar Size Calculator
Input:
- Monthly electricity bill OR monthly units consumed

Output:
- Suggested solar system size
- Simple explanation of why that size was chosen

### 2) Savings Calculator
Output:
- Estimated monthly savings
- Estimated annual savings
- Approximate payback period

### 3) Subsidy Estimator
Input:
- State
- System size

Output:
- Estimated subsidy range
- State-specific guidance if available
- Disclaimer that users should verify with official sources

### 4) Trusted Installer Listings
Show:
- Verified installer name
- Service area
- Rating or trust badge
- Contact details
- Short profile

Important:
- Do not show random vendors
- Do not auto-match users blindly
- Only display trusted and verified installers in the final step

### 5) Installer Quote Request Form
Collect:
- Name
- Phone number
- City
- Monthly bill range
- Rooftop type
- Approximate rooftop area
- Installation timeline

Only users who complete this form should be considered qualified leads.

---

## Future Features

Add these only after the MVP is working:

- Electricity bill upload
- OCR extraction from bill images or PDFs
- Personalized solar report PDF
- Installer dashboard
- Installer reviews
- WhatsApp lead notifications
- State-specific installer filtering
- Financing/EMI guidance

---

## Lead Qualification Rules

A lead is qualified only if it has at least:
- Name
- Phone number
- City
- Solar interest level
- Estimated monthly bill or units
- Installation timeline

Optional but useful:
- Rooftop area
- Roof type
- Electricity provider
- Bill upload

Do not send incomplete leads to installers.

---

## Monetization Rules

The product should be built to make money in a practical way.

Best monetization path:
1. Free user tools
2. Organic traffic and AdSense revenue
3. Qualified lead capture
4. Paid installer leads
5. Installer subscriptions
6. Premium visibility for verified partners

Never build features that do not support one of these outcomes.

---

## SEO Strategy

Focus on long-tail and state-level solar searches.

Examples:
- solar subsidy Bihar
- 3 kW solar system cost Bihar
- rooftop solar Patna
- solar calculator India
- PM Surya Ghar Bihar
- solar panel price for home
- solar savings calculator

Prioritize:
- High-intent keywords
- Location-specific keywords
- Question-based searches
- Informational content that leads to calculator use

---

## Content Strategy

Create content that answers the questions people actually ask:
- How much solar do I need?
- How much roof area is required?
- How much can I save?
- Is subsidy available?
- What documents are needed?
- How do I choose an installer?

Content should help users decide, not just read.

---

## Technical Preferences

Use:
- Next.js
- TypeScript
- Supabase or a similar clean backend
- Mobile-first responsive UI
- OCR/API integrations only where they add real value

Prefer:
- Reusable components
- Clean file structure
- Minimal dependencies
- Simple, maintainable logic

---

## Cursor AI Instructions

When generating or modifying code:

1. Keep business goals in mind.
2. Build for conversion, not just appearance.
3. Use clear component names.
4. Keep the codebase simple.
5. Avoid overengineering.
6. Favor production-ready structure.
7. Write code that can scale across Indian states.
8. Keep SEO and mobile performance in mind.
9. Use environment variables for secrets.
10. Separate business logic from UI logic.

---

## Development Priorities

### Highest Priority
- Calculator accuracy
- Lead capture flow
- Trust-building UX
- Installer verification
- SEO-ready pages

### Medium Priority
- Bill upload
- OCR
- PDF reports
- Installer dashboard

### Low Priority
- Fancy animations
- Non-essential features
- Complex automation that does not help revenue

---

## Decision Filter

Before adding any feature, ask:

1. Does this help the user make a solar decision?
2. Does this help qualify a lead?
3. Does this help an installer get a better customer?
4. Does this support trust, advertising, or revenue?

If the answer is no, do not build it yet.

---

## Definition of Success

The MVP is successful if it can:
- Attract relevant visitors
- Help them estimate solar needs
- Generate AdSense-friendly informational traffic
- Convert a portion of visitors into qualified leads
- Prove that installers are willing to pay for those leads

The goal is not perfection. The goal is validation, trust, and revenue.
