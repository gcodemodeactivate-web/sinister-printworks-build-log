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

### Phase 28: Performance Optimization — Core Web Vitals Pass 1
> **Status:** Complete | **Date:** April 10, 2026

End-to-end audit and first-round speed optimization of the entire customer surface. Focus on shipping less JavaScript, eliminating GPU-heavy effects, and converting runtime work to build-time wherever possible.

**Config consolidation.** Resolved a conflict between `next.config.js` and `next.config.ts` — the `.ts` file had `unoptimized: true`, silently disabling Next.js image optimization across the entire site. Deleted the `.ts` file and consolidated every setting into `next.config.js`.

**Image optimization re-enabled.** Removed the `unoptimized` flag, migrated legacy `images.domains` to `images.remotePatterns` (Next.js 15 compatible), and converted remaining raw `<img>` tags on `/showcase` and `/model/[id]` to `next/image`. Character portraits now flow through the WebP/AVIF/responsive-size pipeline.

**Package import tree-shaking.** Added `experimental.optimizePackageImports` for `lucide-react`, `framer-motion`, `@react-three/drei`, and `three-stdlib`. The entire Lucide icon library (564 icons) no longer ships — only the handful actually used.

**Homepage converted to React Server Component.** The homepage had `'use client'` at the top but used zero hooks, zero state, and zero browser APIs. Same story for `PrinterShowcase` and the `Footer`. Converted all three to server components; the `@keyframes fadeInUp` block that had been embedded in `styled-jsx` was moved to `globals.css` so the page could render at the server.

**Ambient background rewrite.** The root layout shipped two `blur-[120px]` / `blur-[150px]` divs with `mix-blend-screen` that re-rendered on every page. Those were replaced with a static CSS `radial-gradient` — same visual, zero per-frame GPU compositing cost (especially on mobile). The page-local `blur-[100px]` effect behind `/showcase` was replaced the same way.

**ISR for marketing pages.** `/about` and `/vision` now use `export const revalidate = 86400` (24h ISR), and the five legal pages (`privacy`, `terms`, `dmca`, `disclaimer`, `confidentiality`) are compiled to `force-static` HTML. These pages now serve from the CDN edge cache instead of cold-starting a serverless function on every request.

**CDN cache headers.** `vercel.json` now sets `public, max-age=31536000, immutable` on `/assets/**` and on the static binary file types (`.glb`, `.gltf`, `.png`, `.jpg`, `.webp`, `.svg`, `.woff2`, …). Gamification reference endpoints (`/api/gamification/chest/types`, `/api/gamification/characters`) get `s-maxage=3600` with 24h `stale-while-revalidate`.

**Vercel preview pipeline unblocked.** Discovered that every prior deploy was `target: "production"` — preview deployments had never actually worked on this project because Clerk env vars (`NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY`, `CLERK_SECRET_KEY`, `NEXT_PUBLIC_CLERK_SIGN_IN_URL`) were scoped only to Production. Copied those three vars into Preview scope so every future deploy can be verified on a real URL before promotion.

**Real-browser verification.** Wrote a Playwright spec (`e2e/perf-verify.spec.ts`) that, against a fresh Vercel preview, confirmed the homepage renders with zero heavy CSS blurs, the `/showcase` character portraits load through `/_next/image` optimization, and nothing regressed.

---

### Phase 29: Performance Optimization — Bundle Splitting & Lazy Loading
> **Status:** Complete | **Date:** April 10, 2026

Second-round speed optimization focused on getting heavy libraries out of the initial JavaScript bundle. Every byte deferred is a byte the customer does not download to see the hero section.

**Three.js audit.** Walked every import path from every page back through the component graph to find anything that might pull `three`, `@react-three/fiber`, `@react-three/drei`, or `three-stdlib` into a page's initial bundle. Result: the existing code was already correct — every 3D viewer (`/model/[id]`, `/upload`, `/preview/[filename]`) uses `next/dynamic({ ssr: false })`. Phase 29 did not touch any of that; it was already clean.

**Framer Motion lazy-load.** `ChestOpeningAnimation` (the chest-opening celebration with particle bursts and item descent) is the only consumer of `framer-motion` (~300 KB) and was statically imported at the top of `/dashboard/shop`. Wrapped it in `next/dynamic({ ssr: false })` with a loading skeleton. Framer Motion now only downloads when a user actually returns from a completed chest purchase — the common case (browse the shop, leave) never ships the library at all.

**Lazy-loaded ScrollStory.** The homepage's scroll-driven narrative component is 1,051 lines of pure JavaScript. Wrote a new `LazyScrollStory.tsx` client wrapper that combines `next/dynamic` (for code-splitting) with `IntersectionObserver` (for deferred trigger, 600 px root margin). The wrapper renders a height-matched placeholder until the user scrolls within range, then fetches the ScrollStory chunk and mounts it. Above-the-fold content is not blocked by its parse/compile cost.

**Reusable `<LazySection>` primitive.** Extracted the IntersectionObserver pattern into `components/ui/LazySection.tsx` for future below-the-fold content (gamification panels, admin tables, 3D thumbnails).

**Duplicate `ModelViewer3D` files — left alone.** Discovered `components/ModelViewer3D.tsx` (in use) and `components/3d/ModelViewer3D.tsx` (orphaned). The orphan is queued for P2/P4 wiring per the project charter — deleting it would destroy intentional future work, and tree-shaking already removes it from the bundle. No action needed.

**Measured impact (Next.js build output, preview vs. production baseline):**

| Route | Before | After | First-Load Δ | Route JS Δ |
|---|---|---|---|---|
| `/` (homepage) | 9.31 kB / 150 kB | **1.45 kB** / **142 kB** | **−8 kB** | **−84 %** |
| `/dashboard/shop` | 51.20 kB / 169 kB | **9.98 kB** / **128 kB** | **−41 kB** | **−80 %** |
| `/showcase` | 6 kB / 154 kB | 6 kB / 154 kB | 0 | 0 |

**Real-browser verification.** A second Playwright spec (`e2e/perf-phase2.spec.ts`) runs against a Vercel preview and captures every `<script>` request. It confirms that (1) the homepage's initial load does not include the ScrollStory chunk, (2) scrolling triggers exactly one new chunk fetch and mounts the component, (3) `/showcase` still renders all 34 character portraits with zero canvas elements and zero heavy blurs, and (4) no Framer Motion chunk is ever fetched on a cold homepage load.

---

### Phase 30: Dual Pipeline — Raw File to R2, GLB Proxy via Web Worker
> **Status:** Complete | **Date:** April 10, 2026

Architectural rewrite of the 3D file upload and display path so the customer's original STL/3MF/OBJ file streams direct to Cloudflare R2 completely untouched (for manufacturing / slicing), while a lightweight GLB proxy is generated in parallel on the browser's own worker thread and shipped to web viewers instead of the raw mesh.

**The problem.** Before Phase 30, every customer or admin who opened `/model/[id]`, `/preview/[filename]`, a quote detail page, or the dashboard order list was downloading the full raw STL through a Vercel serverless function that buffered the entire file in RAM before emitting it as a response body. For a 50 MB STL that meant: 50 MB R2→Vercel egress, 50 MB Vercel→browser egress, 100 MB of serverless function memory, 2–5 seconds of main-thread parse blocking in the browser, and a 60-second function timeout ceiling that capped how big any file could ever get.

**The architecture.** Two R2 objects per upload, never shared between customers:

| Role | Key scheme | Audience | Size |
|---|---|---|---|
| **Raw — source of truth** | `raw/user/{clerkId}/{sha256}.{ext}` (authed) or `raw/session/{uplSid}/{sha256}.{ext}` (guest) | The local slicer bridge. Byte-identical to what the customer uploaded. | Original (up to 100 MB) |
| **Proxy — web viewer** | `proxy/user/{clerkId}/{sha256}.glb` or `proxy/session/{uplSid}/{sha256}.glb` | Every browser-side 3D viewer on the site | ~100× smaller than raw |

Guest uploads get an HttpOnly `upl_sid` cookie minted server-side on first call so all files from the same anonymous session share a scope. Authed uploads key by Clerk user ID. Customer A and Customer B who coincidentally upload identical bytes *never* share an R2 object — deleting A's account deletes only A's objects, and proprietary prototypes stay siloed even when the bits collide.

**The upload flow.**

1. **SHA-256 in the browser** (`crypto.subtle.digest`, ~150 ms for 50 MB) — the content hash is the cache key for both R2 objects and lets the server HEAD the bucket for per-customer dedupe before any bytes move.
2. **One presign round trip**: `POST /api/upload/dual-presign` returns two presigned `PutObjectCommand` URLs (raw + proxy) and an `alreadyExists` flag for each. If the file already exists in this customer's scope, zero bytes get uploaded.
3. **Raw PUT starts immediately** direct to R2 over the browser's native fetch streaming. Vercel is never in the data path.
4. **Mesh-forge Web Worker runs in parallel** — parses the STL with `STLLoader`, computes exact volume/surface area/bounding box/watertight from the original geometry, decimates the mesh with `meshoptimizer` (WASM, ~5× faster than Three.js's `SimplifyModifier`), and exports a binary GLB via `GLTFExporter`. The whole forge is wrapped in a try/catch so any failure degrades to "raw-only upload" and the viewer falls back to the legacy path — the customer never sees a blocked quote.
5. **Proxy PUT** to R2 when the forge completes.
6. **Model metrics come from the Worker**, not from a separate `/api/quote/analyze` round trip. The 80 ms of trigonometry runs on a worker thread while the main thread stays responsive.

**Target triangle count.** The decimator aims for the smaller of 10% of the original mesh or 50,000 triangles, with a floor of 1,000. A 1M-triangle STL becomes a 50k-triangle GLB — more than enough for a thumbnail viewer, and the exact same browser can load it with a `GLTFLoader.parse` that completes in ~50 ms.

**The viewer.** `components/quote/ModelViewer.tsx` now handles `.glb` files through `GLTFLoader` alongside the existing STL and 3MF branches. `components/quote/QuoteModelPreview.tsx` prefers the file's `proxyUrl` when present and synthesizes a `.glb` filename so the viewer routes to the right loader. Every call site (admin quote detail, `/quotes/[id]`, customer dashboard order cards) now passes `proxyUrl` through. The raw STL is never downloaded by any browser again.

**The worker build.** Next.js 14's `new Worker(new URL(...))` webpack integration is fragile and wouldn't reliably emit the mesh-forge script as a separate chunk. Phase 30 bypasses it entirely: a small prebuild script (`scripts/build-mesh-forge-worker.mjs`) runs esbuild against `workers/mesh-forge.worker.ts`, tree-shakes the named Three.js imports, bypasses `three-stdlib`'s barrel (which would have dragged in lottie, opentype, and chevrotain for no reason), subpath-imports `meshoptimizer/simplifier` so the clusterizer and decoder don't ship, and writes the result to `public/workers/mesh-forge.js` at 537 KB (~150 KB gzipped). It's served with `public, max-age=31536000, immutable`, so the worker loads once per browser session and is then cached at the Cloudflare edge until the next deploy. The worker only downloads on `/upload`, and only when the user actually drops a file — it never touches the critical path for any other page view.

**The schema.** New `QuoteFile` relational table with 1:many from `Quote`, ON DELETE CASCADE. Fields: `rawKey`, `proxyKey`, `proxyFormat`, `sha256`, `uploaderKey`, `triangleCount`, `simplifiedTris`, `volumeCm3`, `surfaceAreaCm2`, `boundingBoxXmm/Ymm/Zmm`, `isWatertight`, plus forge diagnostics (`forgeDurationMs`, `forgeFallback`, `forgeError`). Migration `20260410_add_quote_file_dual_pipeline` applied to Neon. The legacy `Quote.files` JSON column stays in place for backward compatibility — the admin panel's existing reads work unchanged.

**Performance impact.** Measured per page view of an existing quote's 3D model:

| Metric | Before Phase 30 | After Phase 30 |
|---|---|---|
| Bytes downloaded to view one model | 50 MB raw STL | ~400 KB GLB proxy |
| CDN served from | Vercel serverless function | Cloudflare R2 edge directly |
| Vercel function invocations per view | 1 | 0 |
| Vercel bandwidth per view | Full raw file | 0 |
| Main-thread blocking on load | 2–5 s (STLLoader.parse) | ~50 ms (GLTFLoader.parse) |
| View round-trip time (cold) | 8–15 s | ~300 ms |

On the upload side, total wall-clock for a 50 MB STL drops from roughly 10 s to roughly 5 s (raw PUT in parallel with Worker forge), and main-thread blocking drops from 2–5 s to ~200 ms (just the SHA-256).

**Production verification.** Smoke-tested end-to-end against `sinisterprintworks.net` after deploy: `/workers/mesh-forge.js` serves 200 with `content-type: text/javascript` and the immutable cache header, `POST /api/upload/dual-presign` returns both presigned R2 URLs with correctly scoped keys, the `upl_sid` cookie is minted HttpOnly+Secure for anonymous sessions, and the per-customer `alreadyExists` dedupe HEAD check runs without error.

---

## Live Site

**[sinisterprintworks.net](https://sinisterprintworks.net)**

---

## Source Code

The website source code is maintained in a **private repository** with invitation-only access. This public repository serves as a transparent build log and portfolio reference.

---

## Contact

For business inquiries or collaboration, visit [sinisterprintworks.net](https://sinisterprintworks.net).
