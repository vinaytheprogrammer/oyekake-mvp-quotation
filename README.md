# OyeKake MVP Architecture, Quotation & Scaling Roadmap

Official software engineering proposal and Minimum Viable Product (MVP) quotation for the **OyeKake Multi-Vendor Food Delivery Platform**.

- 🌐 **Live Interactive Quotation Website:** [https://vinaytheprogrammer.github.io/oyekake-mvp-quotation/](https://vinaytheprogrammer.github.io/oyekake-mvp-quotation/)
- 💰 **Total Fixed Development Cost:** ₹2,50,000 INR (Flat One-Time Investment)
- 🚫 **Monthly Agency Charges:** ₹0 (All monthly third-party charges eliminated or direct client billing)
- 📍 **Launch Geographic Focus:** Single City (Architected for instant multi-city expansion)
- ⏱️ **Timeline:** 40–45 Working Days
- 🛡️ **Post-Delivery Warranty:** **2 Months (60 Days)** of hands-on technical assistance for requirement-related fixes
- 🔒 **Single Source of Truth (SSOT):** Initially signed scope document serves as the sole contractual benchmark
- 🛠️ **Long-Term SLA:** 1-Year Security Patches & Dependency Version Management

---

> ⚠️ **Important Scope Clarification: Minimum Viable Product (MVP) Notice**  
> This project represents a custom-built **Minimum Viable Product (MVP)**. While the platform incorporates standard, production-ready workflows inspired by platforms such as Swiggy and Domino's (vendor discovery, menu cart checkout, order state alerts, and live GPS map tracking), **it is NOT an exact 1:1 duplication or enterprise clone of Swiggy or Domino's**. Proprietary multi-million-dollar dispatch algorithms, deep gamification, and hyper-custom enterprise features are intentionally excluded to strictly maintain the ₹2,50,000 budget and rapid delivery timeline.

---

## 5 Dedicated User Views & Interfaces

1. **Super Admin Dashboard (Web):** Global revenue, GMV, platform-wide commission take-rates, city-level zone control, global audits, payout reconciliations.
2. **City Admin (Operations Hub) Panel (Web):** Local city order queue monitoring, emergency manual dispatch override, local restaurant KYC/menu approvals, rider verifications.
3. **Vendor / Restaurant Portal (Web / Tablet):** Continuous loud sound alerts for incoming orders, 1-tap accept/reject with preparation timer, live menu manager (stock toggles, variants, pricing), daily sales reports.
4. **Delivery Partner Mobile Application (Android):** Online/offline duty toggle, nearby delivery assignment alerts, restaurant pickup & customer delivery navigation, background GPS streaming, OTP delivery confirmation.
5. **Customer (User) Mobile App & Web (Flutter Android/iOS + Web):** GPS address discovery, rich category browsing, customizable cart, Razorpay/Cashfree online payments & Cash on Delivery, and **Swiggy/Domino's-Style Live Order Tracking**.

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

## Post-Delivery Warranty, Maintenance & SSOT Terms

1. **2 Months Included Assistance:** 60 days of bug fixing, configuration tuning, and minor requirement-related adjustments included in the base ₹2,50,000 fee.
2. **Single Source of Truth (SSOT):** The signed specification acts as the legal source of truth. Any major additions outside this document will be treated as Phase 2 change requests to protect launch timelines.
3. **1-Year Maintenance & Dependency SLA:** Ongoing protection against software rot—Node.js dependencies, npm security vulnerabilities, Flutter SDK updates, and Google Play target API compliance maintained under an annual maintenance contract (starting after Month 2).

---

## Milestone Schedule (₹2,50,000 Total)

- **Milestone 1 (25% - ₹62,500):** UI/UX Design for all 5 roles, PostgreSQL PostGIS DB Schema & Git Setup (8–10 Days)
- **Milestone 2 (25% - ₹62,500):** Backend REST APIs, Super Admin, City Admin & Vendor Portal (12–14 Days)
- **Milestone 3 (25% - ₹62,500):** Customer Apps, Delivery Boy App, Swiggy Live GPS Tracking & Payments (12–14 Days)
- **Milestone 4 (25% - ₹62,500):** QA Testing, VPS Production Deployment, Source Code Handover & **Commencement of 2 Months Free Support** (6–8 Days)
