---
framework_version: 1.1.1
---

# Candidate Profile

<!-- Populated by /setup (Path B) on 2026-09-07 from Dhaval_Fatnani_Resume_latest.pdf plus follow-up answers -->

## Identity
- **Name:** Dhaval Fatnani
- **Location:** Mumbai, India
- **Phone:** +91 89802 26979
- **Email:** info.dhavalfatnani@gmail.com
- **LinkedIn:** https://linkedin.com/in/dhavalfatnani
- **GitHub:** https://github.com/dhavalfatnani
- **Website:** https://dhavalfatnani.vercel.app
- **Status:** Employed full-time at KNOT (Mumbai); searching while employed
- **Constraints:** None on location. Open to Mumbai, any Indian metro, fully remote, and relocation abroad (visa sponsorship would be required outside India; Indian citizen).
- **Salary baseline:** INR 40,00,000 per annum in hand (40 LPA net). A role that would otherwise be a soft deal-breaker (pure operations, very early-stage startup) becomes acceptable if it clears this number.

### Languages
<!-- Every language you can work in professionally, with your honest level. Used by the
Language Gate in 04-job-evaluation.md and by job-scraper/search-queries.md's query-language
generation. Omit any language you don't actually work in - an undeclared language is treated as
a hard no, not a gap to smooth over. -->

| Language | Level | Notes |
|----------|-------|-------|
| English | Fluent (full professional proficiency) | Working language; CV and cover letters in English |
| Hindi | Fluent | Day-to-day language with warehouse and rider teams |
| Gujarati | Fluent | |
| Sindhi | Fluent | |

## Education

| Degree | Period | Institution | Key Topics |
|--------|--------|-------------|------------|
| BTech, Computer Science & Engineering (CGPA 8.64) | Nov 2020 - May 2024 | Navrachana University, Vadodara, India | Software engineering, web development (MERN), databases, cloud and ML foundations (AWS Academy) |

### Certifications
- Certified MERN Full Stack Developer
- AWS Academy Graduate - Machine Learning Foundations
- AWS Academy Graduate - Cloud Foundations
- GUVI AI For India 2.0
- Build and Deploy Your First Web App with Modern Tooling

## Professional Experience

### Founding Product Operations & Systems Lead - KNOT (Aug 2025 - Present)
Mumbai, India. Quick-commerce fashion, 60-minute try-and-buy. 800+ orders/day, 30,000+ SKUs, three warehouses, 100+ person warehouse floor.
- Own the in-house Warehouse Management System end to end: process design with operators on the floor, PRDs and FRDs with the CTO, schema decisions, UAT, defect triage, release documentation, and production software across multiple dark stores. Serialized inventory lifecycle covering tracking, returns, barcode failures, and reuse.
- Ship internal tools solo using AI-assisted development (Claude Code and Claude for architecture, Cursor for build). Twelve are in production, used daily by warehouse, rider, finance, and content teams.
- Rebuilt goods receiving from paper to a digital GRN flow: processing effort down roughly 70%, turnaround time down roughly 90%.
- Designed and shipped COD cash reconciliation from rider collection to bank deposit: a six-state collection-record state machine (CS1 to CS6) with a Razorpay QR settlement bypass, a live finance dashboard, and the as-built PRD.
- Hold cost-side P&L ownership (cost per order, OPEX, rider payouts) and built the reporting that tracks each. Run vendor evaluations and cost cases against those numbers.
- Diagnosed spam-tagging across roughly 1,200 outbound calls a day, costing an estimated 10 to 12% order failure. Built the cost case, benchmarked vendor quotes, won founder approval for a 48-DID warm-up and cutover, then delegated execution through role-based runbooks.
- Built the customer support function from zero (structure, hiring, tooling, escalation paths) and still own it. Warehouse and support teams report daily on orders, dispatch, cash position, rider performance, and SLA breaches; own operational reporting and escalation upward to founders.
- Designed the rider batching dispatch engine for 60-minute last-mile delivery, encoding Mumbai-specific constraints (order type, SLA tier, dwell time, road network, building-entry time, traffic windows). Fixed rider GPS tracking reliability at fleet scale on Android (foreground service, battery-optimization exemptions, OEM-specific watchdogs, server-side heartbeat detection). Built a rider penalty tracker with a nine-category taxonomy feeding payout calculations.

### Growth & Operations Specialist, then Growth & Strategy Associate - KNOT (Nov 2024 - Aug 2025)
Bengaluru, then Mumbai, India. Joined pre-launch; grew from associate to founding lead.
- Set up KNOT's first dark store from zero: core warehouse, inbound, and delivery operations.
- Wrote the SOPs enabling 60-minute apparel delivery across Mumbai; scaled the floor to 400+ orders/day.
- Identified and onboarded 100+ fashion brands targeting Gen Z and young professionals; managed logistics and brand coordination; developed inventory tracking and inbound shipment processes.
- Led customer support and experience operations; served as product liaison with the tech team on WMS development.

### MERN Stack Developer Intern - GeeksforGeeks (Feb 2024 - Aug 2024)
Bengaluru, India
- Designed and implemented RESTful APIs for front-end/back-end data exchange.
- Built responsive web applications on MongoDB, Express.js, React.js, and Node.js; version-controlled team projects via Git.

### Operations & Growth Intern - Inagiffy (Nov 2023 - Jul 2024)
Bengaluru, India
- Managed client delivery for accounts including Motilal Oswal; developed tailored growth strategies aligned to business objectives.
- Implemented automation solutions boosting operational efficiency by 20%; executed SEO strategies; KPI reporting.

<!-- Earlier short roles (Nucleon Health 2022, AIESEC 2022, Hack Club NUV 2022, Shvvet Enterprise 2024) were dropped from the latest resume and are not used in applications. -->

## Independent Projects
- **Automated Cold Outreach System** (personal): Human-in-the-loop LLM pipeline that researches a prospect and sends 30 personalized outreaches a day. Gemini 2.0 Flash for generation, Tavily for research, Gmail API for delivery, Google Sheets as CRM, GitHub Actions for scheduling.
- **KNOT Internal Tooling Suite** (built solo at work, 12+ production tools):
  - Warehouse reporting dashboard: one 1,215-line vanilla JS file. Drop in three CSVs, get merged KPIs that drill down to filtered tables and CSV export, plus colour-coded order-age buckets. PapaParse inlined, zero network calls, works offline.
  - Procurement and serial governance dashboard: full vendor to purchase request to PO to GRN to invoice to payment lifecycle, plus serial-range reservation across three warehouses. Next.js 14, Supabase with RLS and Realtime, shadcn/ui, TanStack Query, Zustand.
  - Escalation portal: replaced WhatsApp groups and verbal handoffs with a raise, assign, track, resolve, audit flow on a creator-owns-until-closure model.
  - Picker-packer Android app: geofenced selfie login, bag-driven picking, scan confirmation, lock mapping. Replaced printed pick sheets so mispicks surface at the shelf rather than the doorstep.
  - Bin location master: generated 4,578 bins for a new warehouse with dual-zone directional logic in Python. The audit layer caught 23 naming conflicts before day one. Repeated for a second warehouse.
  - GRN generator and barcode printing system (Next.js, TypeScript, Supabase, PostgreSQL), standardizing inbound receiving across three warehouses.
  - COD dashboard and cash reconciliation state machine (see experience above).

## Technical Skills

### Programming & Build
- **TypeScript / JavaScript** (primary): Next.js 14 App Router, React, Node, Electron
- **Python** (working): scripting, generators and audit tooling, LLM pipelines
- **SQL / PostgreSQL** (working): schema design, Supabase (RLS, Realtime, Storage, Edge Functions), Drizzle, MongoDB
- **Android (Java/Kotlin)** (working): foreground services, GPS reliability, field apps
- **PHP** (basic)
- **REST APIs**, GitHub Actions, Google Apps Script
- **AI-assisted development** (primary workflow): Claude Code, Claude, Cursor, Anthropic Messages API, Gemini API, Tavily

### Domain Expertise
- Warehouse operations and WMS design: inbound/GRN, putaway, picking, serialized inventory, bin location systems
- Last-mile and rider operations: batching dispatch, SLA design, GPS tracking, penalty and payout systems
- Systems design: state machines, RBAC, workflow automation, escalation and SLA design, dashboarding
- Product ownership: PRD and FRD authoring, UAT, defect triage, release documentation, stakeholder handover
- Operations finance: COD reconciliation, unit economics (cost per order, OPEX), procurement, vendor management, cost cases
- Quick-commerce and fashion e-commerce (60-minute delivery, try-and-buy)

### Software & Tools
- Notion, Linear, Airtable, Postman, Git, Google Sheets, Razorpay, Supabase, Vercel

## Publications
- None.

## Awards
- None listed.

## References
- None listed yet. Add here when available.

More references available upon request.
