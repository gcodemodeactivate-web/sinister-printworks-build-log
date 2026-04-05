# Sinister Printworks Website

**Customer-facing website for Sinister Printworks 3D printing services.**

[![Live Site](https://img.shields.io/badge/Live%20Site-sinisterprintworks.net-FF4500?style=for-the-badge&logo=vercel&logoColor=white)](https://sinisterprintworks.net)

---

## About

Sinister Printworks is a 3D printing services company offering custom prints, prototyping, and manufacturing solutions. This repository documents the public-facing build log for the company website — a full-stack application built from the ground up with modern web technologies.

The source code is maintained in a separate private repository with invitation-only access.

---

## Tech Stack

| Technology | Purpose |
|---|---|
| **Next.js 14** | React framework with App Router, server components, and API routes |
| **Tailwind CSS** | Utility-first styling with custom design system |
| **Clerk Auth** | User authentication, session management, and role-based access |
| **Stripe Payments** | Payment processing, donation checkout, and NDA purchases |
| **Prisma ORM** | Type-safe database client and schema management |
| **Supabase** | PostgreSQL database hosting and real-time capabilities |
| **Vercel** | Production deployment, edge functions, and CI/CD |

---

## Build Log

### Phase 1: Repository & Infrastructure Setup
> **Status:** Complete | **Date:** April 4, 2026

Established the private GitHub repository with proper `.gitignore` configuration for sensitive files (environment variables, API keys, Clerk secrets). Set up build log tracking and development workflow with Vercel CI/CD integration.

---

### Phase 2: Social Media Integration
> **Status:** Complete | **Date:** April 4, 2026

Connected all social media profiles (Instagram, Pinterest, YouTube) across the website footer. Replaced placeholder links with verified profile URLs to establish brand presence across platforms.

---

### Phase 3: Search Engine Branding (Favicon & Open Graph)
> **Status:** Complete | **Date:** April 4, 2026

Generated and configured complete favicon set (`favicon.ico`, `apple-touch-icon.png`) and Open Graph images (`og-image.png`) for proper branding in Google Search results, social media link previews, and browser tabs. Configured `metadata` exports in the root layout for SEO optimization.

---

### Phase 4: Vision & Goals Page
> **Status:** Complete | **Date:** April 4, 2026

Built the `/vision` page featuring the company mission statement, long-term vision, and a roadmap of upcoming capabilities. Designed with the brand's dark aesthetic and responsive layout. Serves as a public-facing declaration of company direction and ambitions.

---

### Phase 5: Equipment Contribution Page with Stripe Integration
> **Status:** Complete | **Date:** April 4, 2026

Created the `/contribute` page with live progress bars for three equipment funding goals:
- **Formlabs Fuse 1+** — Industrial SLS 3D printer
- **Bambu Lab P2S** — High-speed FDM printer
- **Flashforge CJ270** — Large-format resin printer

Integrated Stripe Checkout for direct donations. Revenue from sales and quote orders also contributes to equipment goal progress. Built with real-time progress tracking and transparent funding visibility.

---

### Phase 6: Legal Disclaimer (IP Liability)
> **Status:** Complete | **Date:** April 4, 2026

Authored a comprehensive IP liability disclaimer at `/legal/disclaimer` covering:
- Customer responsibility for file licensing and intellectual property rights
- DMCA compliance and takedown procedures
- Common carrier doctrine applicability to 3D printing services
- Limitation of liability for printed reproductions

Researched federal copyright law, DMCA safe harbor provisions, and industry-standard disclaimer language to ensure legal compliance.

---

### Phase 7: Confidentiality Agreement (NDA) System
> **Status:** Complete | **Date:** April 4, 2026

Built a bilateral NDA system at `/legal/confidentiality` with Stripe-integrated purchase flow:
- Minimum $100 base NDA charge
- Scales with project complexity and scope
- Legally structured as a mutual confidentiality agreement
- Integrated into the checkout flow so customers can add NDA protection during order placement

---

## Live Site

**[sinisterprintworks.net](https://sinisterprintworks.net)**

---

## Source Code

The website source code is maintained in a **private repository** with invitation-only access. This public repository serves as a transparent build log and portfolio reference.

---

## Contact

For business inquiries or collaboration, visit [sinisterprintworks.net](https://sinisterprintworks.net).
