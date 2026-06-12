# PRD.md

## Product Name
**GharUrja**

## Product Type
India-focused rooftop solar decision and lead-generation platform.

## Product Summary
GharUrja helps Indian homeowners understand rooftop solar, estimate system size and savings, check subsidy eligibility, and view trusted and verified local installers.

The product is designed to do three things well:
1. Bring in organic traffic through useful solar content and calculators.
2. Build trust through simple, accurate guidance.
3. Convert high-intent visitors into qualified installer leads.

The business model is a hybrid of:
- AdSense / display ad revenue from informational traffic
- Qualified lead generation for installers
- Future installer subscriptions and premium placements

---

## Problem Statement
Most people who search for solar in India face the same problems:
- They do not know how much solar they need.
- They do not understand subsidy rules.
- They do not know how much they can save.
- They do not know which installers are trustworthy.
- Existing websites are either too technical, too sales-heavy, or too generic.

Installers also struggle to get leads that are actually ready to buy.

GharUrja solves both sides of the market.

---

## Product Goals

### User Goals
- Help homeowners make a solar decision with confidence.
- Reduce confusion around solar cost, savings, and subsidies.
- Make it easy to discover trusted installers.

### Business Goals
- Earn AdSense revenue from informational content.
- Generate qualified leads from serious solar buyers.
- Build a repeatable model that can expand from one state to many.

### Technical Goals
- Keep the platform lightweight.
- Avoid storing unnecessary personal data.
- Keep the app simple to operate and cheap to host.

---

## Non-Goals
The MVP is not trying to be:
- A full solar marketplace
- A solar equipment e-commerce store
- A deep CRM for installers
- A government portal clone
- A complicated SaaS with heavy user accounts

Do not add features that do not improve trust, traffic, qualification, or revenue.

---

## Target Audience

### Primary Audience
Indian homeowners who are researching rooftop solar.

### Secondary Audience
Solar installers and EPC companies that want better-qualified residential leads.

### Initial Geographic Focus
Start with Bihar, then expand state by state.

---

## Positioning
GharUrja should feel like:
- A trusted solar advisor
- A clear explainer for normal people
- A practical lead-generation platform
- A clean informational site with useful tools

It should not feel like:
- A sales page
- A spam directory
- A government clone
- An AI gimmick

---

## Monetization Model

### 1) AdSense / Display Ads
Use ads on informational pages where users are reading guides, FAQs, and state-specific solar content.

Best ad inventory pages:
- Solar education articles
- Subsidy explanation pages
- State pages
- FAQ pages
- Calculator result pages with good SEO traffic

Important rule:
Ads must not destroy trust or make the website look cluttered.

### 2) Qualified Lead Generation
When a user finishes the calculator and wants quotes, collect a short form and send the lead to trusted installers.

### 3) Installer Monetization Later
After validation, offer:
- Paid leads
- Premium verified listings
- Subscription plans for installers

---

## Core Product Principles

### Trust First
- Never exaggerate savings.
- Never guarantee subsidy amounts.
- Always show assumptions.
- Always direct users to official government sources for verification.
- Only show trusted and verified installers.

### Simplicity First
- Keep the interface mobile-first.
- Use plain language.
- Avoid unnecessary technical jargon.
- Keep forms short.

### Revenue First
Every feature must support at least one of these outcomes:
- Traffic
- Trust
- Lead qualification
- Ad revenue
- Installer revenue

### Lightweight First
- No heavy architecture.
- No unnecessary database complexity.
- No user accounts in MVP.
- No long-term storage of personal data unless absolutely required.

---

## Privacy and Data Handling Strategy
The MVP should be designed as a lightweight, privacy-conscious product.

### Default Approach
- Do **not** store user personal information in a database.
- Process lead data only when needed to send it to a trusted installer.
- Avoid building user accounts.
- Avoid storing full lead history inside the product.

### Allowed Storage
- Static content pages
- Installer profile metadata
- State content pages
- Anonymous analytics counts
- Non-personal configuration data

### Preferred Lead Flow
1. User fills a quote request form.
2. The system immediately forwards the information to one or more verified installers.
3. The app discards the data after delivery, unless a temporary log is technically required for delivery confirmation.

### Important Limitation
If no user data is stored, then the app will not support:
- Lead dashboards
- Lead history
- CRM features
- Long-term follow-up automation inside the app

That is acceptable for the MVP.

---

## MVP Scope

## Feature 1: Solar Size Calculator
### Purpose
Help users estimate what solar system size they may need.

### Inputs
- Monthly electricity bill, or
- Monthly electricity units consumed

### Output
- Estimated system size in kW
- Short explanation of the recommendation

### Acceptance Criteria
- User can complete the calculation in under 1 minute.
- Output is understandable to a non-technical homeowner.
- Assumptions are shown clearly.

---

## Feature 2: Savings Calculator
### Purpose
Show the likely financial benefit of rooftop solar.

### Outputs
- Estimated monthly savings
- Estimated annual savings
- Estimated payback period

### Acceptance Criteria
- Output should be conservative, not overly optimistic.
- A short assumptions note should appear below the result.

---

## Feature 3: Subsidy Estimator
### Purpose
Help users understand possible subsidy eligibility.

### Inputs
- State
- System size

### Outputs
- Estimated subsidy range
- High-level subsidy guidance
- Notice to verify on official sources

### Data Rules
- Subsidy values must be editable.
- Subsidy values must not be hardcoded into logic.
- Use a simple admin-editable config or content file.

### Acceptance Criteria
- User can see state-specific guidance.
- The page clearly states that government rules may change.

---

## Feature 4: Trusted Installer Listings
### Purpose
Show only trusted and verified installers.

### Installer Listing Fields
- Company name
- City / service area
- Verified badge
- Short description
- Contact method
- Trust indicators

### Rules
- Do not show random vendors.
- Do not auto-match users blindly.
- Do not show unverified companies.
- The listings are informational and trust-based, not a mass marketplace.

### Acceptance Criteria
- Every listed installer has been manually reviewed or verified.
- The UI clearly indicates verified status.

---

## Feature 5: Quote Request Form
### Purpose
Convert high-intent users into qualified leads.

### Required Fields
- Name
- Phone number
- City
- Estimated monthly bill or units
- Rooftop type
- Approximate rooftop area
- Installation timeline

### Optional Fields
- Email
- Address area name
- Electricity provider
- Roof ownership status

### Lead Qualification Rule
A lead is qualified only when the user has completed the quote form and shown clear purchase intent.

### Acceptance Criteria
- Form is short and mobile-friendly.
- Form clearly explains what happens next.
- Lead is routed only to verified installers.

---

## Content Strategy
GharUrja should publish content that answers real search intent.

### Core Topics
- Solar subsidy in India
- Solar system cost by size
- Solar savings estimation
- Rooftop area requirements
- How solar installation works
- How to choose a trusted installer

### SEO Content Types
- State guides
- FAQ pages
- Calculator landing pages
- Comparison pages
- Step-by-step explanation pages

### Content Rule
Content should help users decide, not just attract clicks.

---

## SEO Strategy

### Primary Keyword Types
- Solar subsidy + state
- Solar calculator + state
- Solar cost + kW size
- Rooftop solar + city
- Solar savings calculator

### SEO Priorities
1. Long-tail keywords
2. State-specific keywords
3. Problem-based search queries
4. High-intent calculator pages

### Internal Linking Strategy
- Link articles to calculators
- Link calculators to quote form
- Link state pages to installer listings

---

## UX Requirements
- Mobile-first design
- Fast-loading pages
- Clear call to action
- Simple calculators
- Minimal friction before quote request
- High trust visual style

The interface should feel calm, useful, and credible.

---

## Technical Requirements

### Frontend
- Next.js
- TypeScript

### Hosting
- Prefer lightweight Cloudflare-based deployment if feasible
- Keep hosting costs near zero during MVP

### Backend
- Minimal backend only
- No heavy account system
- No database unless a feature truly requires it

### Integrations
- AdSense for ads
- Email or webhook forwarding for leads
- OCR only in later phases

### Performance Goals
- Fast mobile load times
- Simple page structure
- SEO-friendly HTML
- Minimal JavaScript where possible

---

## Analytics Requirements
Track only anonymous and aggregate metrics such as:
- Page views
- Calculator completions
- Form submissions
- Installer clicks
- State page performance

Do not overbuild analytics in MVP.

---

## MVP User Journey
1. User lands on a solar guide page or calculator page.
2. User learns about solar in simple language.
3. User uses the calculator.
4. User sees savings and subsidy guidance.
5. User views a short list of trusted installers.
6. User requests quotes if ready.
7. The lead is forwarded to verified installers.

---

## Success Metrics

### Traffic Metrics
- Organic visits
- Calculator usage rate
- Time on page

### Engagement Metrics
- Quote form completion rate
- Installer click-through rate
- Content engagement

### Revenue Metrics
- Ad impressions
- Ad revenue
- Installer lead revenue

---

## Launch Criteria
The MVP is ready to launch when:
- Calculators work reliably
- Content is readable and useful
- Installer listings are verified
- Quote requests can be submitted cleanly
- The site is fast on mobile
- No unnecessary storage of user data is built in

---

## Out of Scope for MVP
Do not build these yet:
- User accounts
- Installer dashboards
- Full CRM
- Lead history storage
- Complex automation
- Payment processing
- Multi-language support unless needed
- Government portal integration

---

## Future Roadmap
After validation, consider:
- Electricity bill OCR
- Personalized solar PDF reports
- State-by-state pages
- Installer subscription plans
- Lead delivery optimization
- WhatsApp notifications
- Better installer verification system

---

## Definition of Success
The MVP is successful if it:
- Attracts real solar-intent users
- Builds trust through useful tools
- Earns AdSense revenue from informational traffic
- Produces qualified leads for verified installers
- Proves the business can grow without unnecessary complexity
