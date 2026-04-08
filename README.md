# Sinister Printworks Website

**Full-stack 3D printing e-commerce platform — built from the ground up.**

[![Live Site](https://img.shields.io/badge/Live%20Site-sinisterprintworks.net-FF4500?style=for-the-badge&logo=vercel&logoColor=white)](https://sinisterprintworks.net)

---

## About

Sinister Printworks is a 3D printing services company offering custom prints, prototyping, and on-demand manufacturing. This repository is the public build log for the company website — a full-stack application with 33+ pages, 90+ API endpoints, and 22 database models.

The source code is maintained in a separate private repository with invitation-only access.

---

## Platform Statistics

| Metric | Count |
|--------|-------|
| Pages | 33+ |
| API Endpoints | 90+ |
| Database Models | 22 |
| Enum Types | 14 |
| Third-Party Integrations | 12+ |
| Gamification Tiers | 10 |

---

## Tech Stack

| Technology | Purpose |
|---|---|
| **Next.js 14** | React framework with App Router, server components, API routes |
| **TypeScript** | Type-safe development across entire codebase |
| **React 18** | UI components with server and client rendering |
| **Tailwind CSS** | Utility-first styling with custom dark theme design system |
| **Clerk** | Authentication, session management, role-based access (CUSTOMER/OWNER) |
| **Stripe** | Payment processing, checkout sessions, webhooks, coupon generation |
| **Prisma ORM v7** | Type-safe database client with PostgreSQL adapter |
| **PostgreSQL (Neon)** | Serverless PostgreSQL with connection pooling |
| **EasyPost** | Shipping rate calculation, label generation, tracking webhooks |
| **Cloudflare R2** | Object storage for 3D files, images, and uploads |
| **Resend** | Transactional email delivery (welcome, rank-up, promotions) |
| **Three.js / React Three Fiber** | Real-time 3D model visualization (STL/3MF) |
| **Vercel** | Production hosting, serverless functions, CI/CD, cron jobs |
| **Serper.dev** | Multi-platform 3D model search API |
| **Google Gemini AI** | AI-powered model analysis and pricing suggestions |
| **VirusTotal** | File security scanning for uploaded 3D models |
| **Bambu Lab / MQTT** | 3D printer cloud connectivity and status monitoring |

---

## Build Log

### Phase 1: Repository & Infrastructure Setup
> **Status:** Complete | **Date:** April 4, 2026

Private GitHub repository with `.gitignore` for secrets. Vercel CI/CD integration with automatic deployments on push. Environment variable management across development, preview, and production.

---

### Phase 2: Social Media Integration
> **Status:** Complete | **Date:** April 4, 2026

Connected Instagram, Pinterest, and YouTube profiles in website footer with verified brand URLs.

---

### Phase 3: Search Engine Branding (Favicon & Open Graph)
> **Status:** Complete | **Date:** April 4, 2026

Custom favicon set, Open Graph images, apple-touch-icon, and comprehensive SEO metadata in the root layout for Google Search and social media link previews.

---

### Phase 4: Vision & Goals Page
> **Status:** Complete | **Date:** April 4, 2026

`/vision` page with mission statement, core values, and Coming Soon product roadmap (SLS nylon, full-color printing, CNC machining). Equipment contribution CTAs.

---

### Phase 5: Equipment Contribution System
> **Status:** Complete | **Date:** April 4, 2026

`/contribute` page with interactive progress bars for equipment fundraising goals (Formlabs Fuse 1+, Bambu Lab P2S, Full-Color Printer, CNC Laser Cutter). Stripe Checkout for donations. 25% revenue allocation from sales/quotes. Contribution tracking and impact descriptions.

---

### Phase 6: Legal Disclaimer (IP Liability)
> **Status:** Complete | **Date:** April 4, 2026

`/legal/disclaimer` covering intellectual property responsibility, DMCA compliance, common carrier doctrine, and limitation of liability.

---

### Phase 7: Confidentiality Agreement (NDA) System
> **Status:** Complete | **Date:** April 4, 2026

Bilateral NDA with Stripe-gated purchase flow ($100-$1000 pricing tiers based on order value). E-signature capture via SignatureCanvas component. Unique NDA numbering (NDA-YYYYMMDD-XXXX). Status tracking and 5-year term. Routes: `/nda`, `/legal/confidentiality`.

---

### Phase 8: Public Build Log
> **Status:** Complete | **Date:** April 4, 2026

This repository — transparent build history for portfolio and investor reference.

---

### Phase 9: 3D Model Meta-Search Engine
> **Status:** Complete | **Date:** April 5, 2026

`/search` page with multi-platform search across Printables, Cults3D, Thangs, Thingiverse, and MyMiniFactory. Powered by Serper.dev API. BM25 ranking, source filtering, pagination, and save-to-archive functionality.

---

### Phase 10: Quote-to-Fulfillment Pipeline
> **Status:** Complete | **Date:** April 5, 2026

`/upload` page with drag-and-drop STL/3MF upload. Automatic model analysis (volume, weight, surface area, watertight check). Material selection with color palettes. Multi-color AMS support with purge fees. Instant price estimation. Guest checkout without account requirement. Real-time 3D preview via Three.js.

---

### Phase 11: Admin Dashboard & Quote Management
> **Status:** Complete | **Date:** April 6, 2026

`/admin` with full quote lifecycle management. Status pipeline: PENDING_REVIEW → PRICED → PAID → SLICING → PRINTING → QUALITY_CHECK → AWAITING_SHIPMENT → SHIPPED → FULFILLED. QuotePricer for manual pricing override. FulfillmentPanel for production tracking. Bulk quote operations. Material stock alerts.

---

### Phase 12: Stripe Payment Integration
> **Status:** Complete | **Date:** April 6, 2026

Checkout sessions, payment intents, and webhook handling (checkout.session.completed, charge.refunded). Automatic quote status updates on payment. Stripe customer ID tracking. Invoice generation. Guest checkout support for unauthenticated users.

---

### Phase 13: Shipping Pipeline (EasyPost)
> **Status:** Complete | **Date:** April 6, 2026

Real-time shipping rate calculation, automatic label generation, webhook tracking updates. Carrier integration (USPS, UPS, FedEx). Address verification. Box dimension calculation from STL model bounds. Manual label fallback for reliability.

---

### Phase 14: 3D Visualization Engine
> **Status:** Complete | **Date:** April 6, 2026

Real-time STL/3MF viewer using Three.js, @react-three/fiber, and @react-three/drei. ModelViewer3D and ModelViewerEngine components. Interactive rotation/zoom, color preview for multi-color prints, model bounds visualization. Mobile-responsive rendering.

---

### Phase 15: Material Inventory Management
> **Status:** Complete | **Date:** April 7, 2026

`/admin/inventory` with spool tracking (brand, type, color, weight remaining percentage). Status management (in-stock, low, out-of-stock, on-order). Shelf and AMS slot location tracking. Amazon reorder links. Low-stock alerts on admin dashboard.

---

### Phase 16: Archive & Print Lists
> **Status:** Complete | **Date:** April 7, 2026

`/archive` with user-created print lists. Add models from search results. Public/private visibility toggle. Unique share tokens for public list access. List management (name, description, items).

---

### Phase 17: NDA System Overhaul
> **Status:** Complete | **Date:** April 8, 2026

Enhanced `/nda` with dual-party e-signature workflow (customer signs → owner counter-signs). SignatureCanvas component for digital signatures. PDF generation and download. Status lifecycle: PENDING_PAYMENT → PENDING_CUSTOMER_SIGNATURE → PENDING_OWNER_SIGNATURE → ACTIVE → EXPIRED/VOIDED. Admin NDA management at `/admin/ndas`.

---

### Phase 18: DMCA Policy Page
> **Status:** Complete | **Date:** April 7, 2026

`/legal/dmca` with registered agent information and DMCA compliance procedures.

---

### Phase 19: Privacy Policy & Terms of Service
> **Status:** Complete | **Date:** April 7, 2026

`/legal/privacy` covering data collection, model storage, and payment processing. `/legal/terms` with service terms and conditions.

---

### Phase 20: File Security Pipeline
> **Status:** Complete | **Date:** April 7, 2026

VirusTotal integration for malware scanning of uploaded 3D files. Cloudflare R2 storage with presigned URLs for secure upload/download. File hash tracking for deduplication. Automatic 30-day deletion. Encryption-at-rest.

---

### Phase 21: Bambu Lab Printer Integration
> **Status:** Complete | **Date:** April 7, 2026

MQTT cloud connectivity via Bambu.cloud for live printer status monitoring. Remote job monitoring. Multi-color AMS support with automatic color palette mapping. OrcaSlicer command-line integration for G-code generation.

---

### Phase 22: Homepage Overhaul & Eagle Rising Animation
> **Status:** Complete | **Date:** April 7, 2026

Apple-style ScrollStory component with scroll-driven animations. PrinterShowcase and MaterialsScrollStory components. Heraldic eagle SVG with animated entrance. Dark aesthetic with Sinister Orange/Red color scheme. Trust bar and "How It Works" 3-step flow.

---

### Phase 23: Two-Sided Dashboards
> **Status:** Complete | **Date:** April 8, 2026

Customer "Command Center" at `/dashboard` with work order mini stepper (WorkOrderMiniStepper), quote tracking, NDA section, and order history. Admin command center with full quote management, fulfillment, and inventory tools. Dark-themed authentication pages via Clerk.

---

### Phase 24: Gamification Loyalty System
> **Status:** Complete | **Date:** April 8, 2026

10-tier rank progression system:

| Tier | Points | Discount |
|------|--------|----------|
| Ash-grubber | 0 | 0% |
| Initiate | 50 | 2% |
| Spark-catcher | 150 | 3% |
| Apprentice | 300 | 5% |
| Journeyman | 500 | 6% |
| Artisan | 750 | 8% |
| Master Craftsman | 1,000 | 10% |
| Soul-smith | 1,300 | 12% |
| Divine Craftsman | 1,600 | 13% |
| Sinister Forge Master | 2,000 | 15% |

Points earned from purchases (1 pt/$1), donations (2 pt/$1), and social proof (25-50 pts per review/follow). Auto-generated Stripe coupon codes on rank-up. Social media verification workflow: submit proof → admin review → approve/reject. Customer dashboard integration with EarnPointsSection. Admin panel at `/admin/gamification`.

---

### Phase 25: Automated Email Pipeline
> **Status:** Complete | **Date:** April 8, 2026

Resend.io integration for welcome emails, quote confirmations, payment receipts, shipping notifications, and rank-up congratulations. Bi-weekly promotional cron job (1st and 15th of each month) with personalized tier progress updates, active discount codes, and engagement CTAs.

---

### Phase 26: About Us Page
> **Status:** Complete | **Date:** April 8, 2026

`/about` with MaterialsScrollStory component showcasing manufacturing capabilities and company information.

---

### Phase 27: Gamification V2 — Characters, Chests, Boosts & Inventory
> **Status:** Complete | **Date:** April 9, 2026

Major gamification expansion:

**Character System** — 10 unique 16-bit dark pixel art characters, one per tier (The Cinder Rat → The Abyssal Architect). Each tier's character is dramatically more impressive. Equipped armor/items display on characters.

**Chest / Loot Box System** — 4 chest tiers (Bronze $5, Silver $12, Gold $25, Sinister $50) with weighted random drops. Items include XP boosts (1.25x–3x), armor (timed XP multipliers), discount consumables (5–25% off), and timed discount buffs.

**XP Boost System** — Activatable XP multipliers from chests or purchases. Only highest active boost applies (no multiplicative stacking). Hard-capped at 3x maximum.

**Player Inventory** — Full inventory management with equip/unequip armor, activate XP boosts, and use discount consumables (generates Stripe coupon codes).

**Forge Shop** — `/dashboard/shop` for chest purchases via Stripe checkout. Three.js-powered chest opening animation with rarity-colored particle effects and divine item descent.

**Web Push Notifications** — Free browser notifications for rank-up alerts, weekly rank progress reminders, and promotional updates. No SMS costs.

**Admin Enhancements** — Player inventory viewer, chest revenue statistics, and notification logs in `/admin/gamification`.

---

## Live Site

**[sinisterprintworks.net](https://sinisterprintworks.net)**

---

## Source Code

The website source code is maintained in a **private repository** with invitation-only access. This public repository serves as a transparent build log and portfolio reference.

---

## Contact

For business inquiries or collaboration, visit [sinisterprintworks.net](https://sinisterprintworks.net).
