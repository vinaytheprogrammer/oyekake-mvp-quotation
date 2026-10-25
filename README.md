# OyeKake MVP Architecture, Quotation & Scaling Roadmap

Official software engineering proposal and Minimum Viable Product (MVP) quotation for the **OyeKake Multi-Vendor Food Delivery Platform**.

- 🌐 **Live Interactive Quotation Website:** [https://vinaytheprogrammer.github.io/oyekake-mvp-quotation/](https://vinaytheprogrammer.github.io/oyekake-mvp-quotation/)
- 💰 **Total Fixed Development Cost:** ₹2,50,000 INR (Flat One-Time Investment)
- 🚫 **Monthly Agency Retainer:** ₹0 (All monthly third-party charges eliminated or direct client billing)
- 📍 **Launch Geographic Focus:** Single City (Architected for instant multi-city expansion)
- 📱 **Mobile Deliverables:** Native-performance **Android App** (`.aab`/`.apk`) & **iOS App** (`.ipa`/TestFlight)
- 💻 **Web Portals:** Customer Ordering Website & Dedicated **Service, Support & Maintenance Administration Website**
- 🔑 **Access Control:** Multi-tier Role-Based Access Control (**Super Admin** vs **City Admin / Operations**)
- ⏱️ **Timeline:** 40–45 Working Days
- 🛡️ **Post-Delivery Warranty:** **2 Months (60 Days)** of hands-on technical assistance for requirement-related fixes
- 🔒 **Single Source of Truth (SSOT):** Initially signed scope document serves as the sole contractual benchmark
- 🛠️ **Long-Term SLA:** 1-Year Security Patches & Dependency Version Management

---

> ⚠️ **Important Scope Clarification: Minimum Viable Product (MVP) Notice**  
> This project represents a custom-built **Minimum Viable Product (MVP)**. While the platform incorporates standard, production-ready workflows inspired by platforms such as Swiggy and Domino's (vendor discovery, menu cart checkout, order state alerts, and live GPS map tracking), **it is NOT an exact 1:1 duplication or enterprise clone of Swiggy or Domino's**. Proprietary multi-million-dollar dispatch algorithms, deep gamification, and hyper-custom enterprise features are intentionally excluded to strictly maintain the ₹2,50,000 budget and rapid delivery timeline.

---

## Technical Deliverables: Android, iOS & Web Architecture

1. **Android Customer & Delivery Applications:**
   - Flutter Dart native compile with hardware-accelerated rendering.
   - Built to target latest Google Play API levels.
   - Deliverables: Release `.aab` (Android App Bundle) signed for Google Play Store + standalone `.apk` for internal testing.
2. **iOS Customer Application:**
   - Production-ready iOS build package and Xcode archive.
   - Tested for iOS guidelines, ready for TestFlight beta testing and App Store distribution.
3. **Customer Responsive Ordering Website:**
   - Fast React / Next.js web application functioning across desktop, tablet, and mobile browsers without requiring app downloads.
4. **Service, Support & Maintenance Administration Website (RBAC):**
   - **Super Admin Role:**
     - Master control over all system settings, global database maintenance, and commission take-rate configurations.
     - Multi-city and regional franchise management.
     - Payment gateway credentials, webhook secrets, and financial payout reconciliation.
     - System-wide security audit logs and administrative delegation.
   - **City Admin (Operations Hub) Role:**
     - Local city-level order queue monitoring (unassigned, delayed, or stuck orders).
     - Manual dispatch and emergency rider re-assignment.
     - Local restaurant KYC document verification, menu moderation, and temporary store deactivation.
     - Delivery partner document checks (driving license, vehicle registration).
     - Customer grievance tickets and operational escalation.

---

## Deployment Charges & Infrastructure Accounts

All professional engineering deployment services are **100% INCLUDED in the ₹2,50,000 fixed price**. External store accounts and domain registrations are client-owned directly with zero developer markups:

| Component | Responsibility / Description | Cost to Client |
|---|---|---|
| **Technical Deployment Service** | Server provisioning, Docker containerization, PostgreSQL/PostGIS database setup, Nginx reverse proxy, PM2 cluster, and automated SSL | **₹0 (Included in ₹2.5L Fee)** |
| **Store Submission Assistance** | Android keystore signing, Play Store upload, iOS certificates & provisioning profiles setup | **₹0 (Included in ₹2.5L Fee)** |
| **Custom `.com` Domain Name** | Dedicated branded domain (e.g. `oyekake.com`) registered under client's corporate name on GoDaddy / Cloudflare Registrar | **~₹800 – ₹1,200 / year** (Direct to registrar) |
| **Google Play Console Account** | Official Google Play Developer Account for Android publishing | **US$25 one-time lifetime fee** (~₹2,100 direct to Google) |
| **Apple Developer Program** | Official Apple Developer Account for iOS App Store publishing (optional if launching Android-first) | **US$99 / year** (~₹8,300/yr direct to Apple) |
| **Cloudflare DNS & SSL** | Enterprise-grade global CDN, DDoS mitigation, and auto-renewing SSL certificates | **₹0 (Free Forever)** |
| **Cloud VPS Server** | DigitalOcean / Hetzner / Hostinger high-performance VPS for single-city launch | **~₹400 – ₹800 / month** (Direct to host) |

---

## Swiggy / Domino's-Grade Live Tracking Engine

- **5-Stage Order Tracker:** Order Placed ➔ Food Preparing ➔ Rider Assigned ➔ Out for Delivery (Live Moving Vehicle on Map) ➔ Delivered (via OTP).
- **Cost-Optimized Coordinate Streaming:** Raw coordinates streamed over lightweight WebSockets with client-side bearing interpolation. Smooth, realistic vehicle movement without triggering excessive Google Maps API queries (operating within Google Maps $200 free monthly credit).

---

## Geographic Focus & Scaling Roadmap

| Expansion Tier | Footprint | Technical Mechanism | Cloud Infra Cost |
|---|---|---|---|
| **Phase 1: Launch (MVP)** | **1 Focus City** | Single High-Performance VPS + PostgreSQL PostGIS + WebSockets | **~₹500 – ₹1,000 / mo** |
| **Phase 2: Regional** | 3–5 Nearby Cities | Redis Cache for Rider Location Pub/Sub + DB Read Replicas | **~₹3,500 – ₹6,000 / mo** |
| **Phase 3: National** | 20+ Cities / Pan-India | Docker/K8s Cluster + Kafka/RabbitMQ Event Queue + Auto Dispatch | **~₹15,000 – ₹35,000 / mo** |

---

## Automated Billing, Taxation & Refund Management System

1. **Smart Cart & Tax Engine:** Automated server-side calculation of item base prices + size variants + add-ons, transparent restaurant GST/tax breakdown, distance-based dynamic delivery fee matrix, platform convenience fees, and coupon code deductions with digital receipt generation.
2. **Cancellation & Payment Gateway Refund Engine:** Configurable cancellation policy (free before restaurant acceptance), 1-click admin refund initiation, direct integration with Razorpay/Cashfree Refund APIs for automatic return of funds to customer UPI/Card/Netbanking accounts, and live customer refund status tracking (*Initiated ➔ Processing ➔ Credited*).
3. **Vendor Commission & Settlement Ledger:** Automated deduction of platform take-rate % per order, complete ledger bookkeeping (`Net Payout = Gross Sales - Platform Commission - Refunds`), and exportable settlement sheets (CSV/PDF) for executing bank transfers.

---

## Post-Delivery Warranty, Maintenance & SSOT Terms

1. **2 Months Included Assistance:** 60 days of bug fixing, configuration tuning, and minor requirement-related adjustments included in the base ₹2,50,000 fee.
2. **Single Source of Truth (SSOT):** The signed specification acts as the legal source of truth. Any major additions outside this document will be treated as Phase 2 change requests to protect launch timelines.
3. **1-Year Maintenance & Dependency SLA:** Ongoing protection against software rot—Node.js dependencies, npm security vulnerabilities, Flutter SDK updates, and Google Play target API compliance maintained under an annual maintenance contract (starting after Month 2).

---

## Milestone Schedule (₹2,50,000 Total)

- **Milestone 1 (25% - ₹62,500):** UI/UX Design for all roles, PostgreSQL PostGIS DB Schema & Git Setup (8–10 Days)
- **Milestone 2 (25% - ₹62,500):** Backend REST APIs, Super Admin, City Admin & Vendor Portal (12–14 Days)
- **Milestone 3 (25% - ₹62,500):** Customer Android & iOS Apps, Delivery Boy App, Swiggy Live GPS Tracking & Payments (12–14 Days)
- **Milestone 4 (25% - ₹62,500):** QA Testing, VPS Production Deployment, Domain & Store Setup, Source Code Handover & **Commencement of 2 Months Free Support** (6–8 Days)
