# OyeKake Lean MVP Architecture & Quotation

Official software engineering proposal and Lean Minimum Viable Product (MVP) quotation for the **OyeKake Food Delivery Platform**.

- 🌐 **Live Interactive Quotation Website:** [https://vinaytheprogrammer.github.io/oyekake-mvp-quotation/](https://vinaytheprogrammer.github.io/oyekake-mvp-quotation/)
- 💻 **Interactive Proof of Concept (POC) Repo:** [https://github.com/vinaytheprogrammer/oyekake-poc](https://github.com/vinaytheprogrammer/oyekake-poc)
- 💰 **Total Fixed Development Cost:** ₹1,20,000 INR (Flat One-Time Investment)
- 🚫 **Monthly Agency Retainer:** ₹0 (All monthly third-party charges eliminated or direct client billing)
- 📍 **Launch Geographic Focus:** Single City (Laser-focused initial operational launch)
- 📱 **Mobile Deliverable:** Single Unified **3-in-1 Android App** (Customer, Vendor & Delivery Partner roles inside one app)
- 💻 **Web Administration:** MERN Web Admin Dashboard (**Super Admin** vs **Admin** operations console)
- ⏱️ **Timeline:** 30–35 Working Days (4–5 Weeks)
- 🛡️ **Post-Delivery Warranty:** **30 Days** of complimentary bug-fixing assistance
- 🔒 **Single Source of Truth (SSOT):** Scope locked to prevent delays and protect project budget

---

> ⚠️ **Scope Optimization Notice (Tailored for ₹1.10L – ₹1.20L Budget)**  
> To deliver a stable, high-performance platform within the client's ₹1.10L – ₹1.20L budget, complex enterprise overheads (such as continuous WebSocket live bicycle map animations, multi-app ecosystems, and iOS builds) have been strategically replaced with streamlined alternatives: **4-Stage Milestone Order Tracking**, **1-Tap External Google Maps Navigation for Riders**, and a **Single Unified 3-in-1 Android Application**.

---

## 📱 3-in-1 Android App & MERN Architecture

1. **Customer Mobile Experience (In-App):**
   - Mobile OTP login & user profile with saved addresses.
   - Restaurant catalog filtered by local city area.
   - Menu browsing (Categories, Veg/Non-Veg indicators, variants, add-ons).
   - Cart & checkout with Razorpay Online Payments (UPI, Cards, Netbanking) & Cash on Delivery (COD).
   - **4-Stage Order Status Tracker:** `Order Placed` ➔ `Preparing in Kitchen` ➔ `Out for Delivery` ➔ `Delivered`.
   - **Secret 4-Digit Delivery OTP:** Displayed on customer screen to give rider on arrival.
   - 1-Tap "Call Delivery Boy" and 1-Tap "WhatsApp Support" buttons.

2. **Vendor / Restaurant Portal (In-App):**
   - Audio chime sound alerts on new incoming orders.
   - 1-Tap "Accept Order" (with food preparation timer) or "Reject Order".
   - 1-Tap "Food Prepared & Ready for Pickup".
   - Menu stock availability manager (toggle items in/out of stock live).
   - Daily orders and revenue summary.

3. **Delivery Partner View (In-App):**
   - Active online/offline shift duty toggle.
   - Incoming delivery assignment alerts with restaurant pickup & customer delivery address.
   - **1-Tap Google Maps Navigation:** Launches the native Google Maps app on the rider's phone with pre-filled destination coordinates (eliminates thousands in custom map SDK charges).
   - 4-Digit OTP customer delivery confirmation to prevent false deliveries.

4. **Web Administration (React.js MERN Web Portal with RBAC):**
   - **👑 Super Admin (Platform Owner):**
     - Master financial dashboard: Gross Merchandise Value (GMV), 15% platform commission take-rate, and net vendor payables.
     - Restaurant onboarding, KYC verification, and commission overrides.
     - Vendor payout approval and exportable bank transfer sheets.
     - Multi-city expansion manager.
   - **🛡️ City Admin (Hub Operations):**
     - Localized live dispatch queue for Kanpur/Lucknow single-city hub.
     - Manual order override (cancellations, rider reassignments).
     - Local delivery fleet on-duty status.

---

## 🛠️ Technology Stack & Zero-Cost Development Workflow

As a **MERN stack developer**, the application is engineered with high-efficiency technologies that avoid native Android development overhead while giving the client 100% native performance:

| Layer | Technology | Operational & Cost Advantage |
| :--- | :--- | :--- |
| **Mobile App** | **React Native with Expo** | Write 100% React.js/JSX. One unified codebase builds the Android app for Customer, Kitchen, and Rider. |
| **Development & Live Debugging** | **Expo Go (Mobile)** | **100% FREE (₹0).** Connects phone to laptop via Wi-Fi with instant Fast Refresh hot-reloading. Unlimited scans, unlimited daily debugging. |
| **Standalone APK / AAB Compilation** | **Expo EAS Build** | **FREE (30 builds/month).** Compiles installable `.apk` and production `.aab` in the cloud without needing Android Studio or Java on developer's machine. |
| **Backend API** | **Node.js + Express** | High-throughput REST API with Server-Sent Events (SSE) and JWT Role-Based Access Control (RBAC). |
| **Database** | **MongoDB Atlas** | Managed cloud database. Free M0 cluster handles up to ~50,000 orders with daily automated backups. |
| **Web Admin Portal** | **React.js + Vite** | Lightweight responsive operations console deployed on global CDN (Vercel / Cloudflare). |

---

## 💰 Technical Deployment & Third-Party Expenses

All professional engineering deployment services are **100% INCLUDED in the ₹1,20,000 fixed price**. Third-party infrastructure accounts are owned directly by the client with zero markups:

| Component | Responsibility / Description | Cost to Client |
|---|---|---|
| **Technical Deployment Service** | Server provisioning, Node.js PM2 runtime, MongoDB database setup, Nginx reverse proxy, and SSL configuration | **₹0 (Included in ₹1.2L Fee)** |
| **Custom `.com` Domain Name** | Dedicated branded domain (e.g. `oyekake.com`) registered under client's corporate name on GoDaddy / Cloudflare | **~₹800 – ₹1,000 / year** (Direct to registrar) |
| **Google Play Console Account** | Official Google Developer Account for Android publishing (Lifetime validity, unlimited apps) | **US$25 one-time lifetime fee** (~₹2,100 direct to Google; ₹0 from Expo) |
| **Cloud VPS / PaaS Server** | Render / Railway / DigitalOcean VPS for single-city launch | **~₹400 – ₹600 / month** (Direct to host) |
| **Cloudflare CDN, DNS & SSL** | Enterprise-grade global edge caching, DDoS mitigation, and auto-renewing SSL | **₹0 (Free Forever)** |

---

## 🎯 Smart Scope Pruning: Why ₹1,20,000 Is Feasible

| Feature Category | High-Budget Approach (Excluded) | Our Lean Smart MVP Solution (Included in ₹1.2L) |
|---|---|---|
| **Delivery Tracking** | Real-time moving bicycle icon streaming GPS over continuous WebSockets ($$$ server bills) | 4-Stage visual milestone tracker (Placed ➔ Cooking ➔ Out for Delivery ➔ Delivered) + 1-Tap "Call Rider" |
| **Rider Navigation** | In-app turn-by-turn map SDK embedded inside the app (costs thousands in API fees) | 1-Tap "Navigate" button that launches native Google Maps app with exact coordinates |
| **Mobile Platforms** | Separate native Android app + separate iOS app ($99/yr Apple account + Mac dev) | Single high-performance Android application built with React Native / Expo covering all 3 user roles |
| **Customer Support** | Custom in-app live chat ticketing system with AI bots | Floating 1-tap WhatsApp support launcher linking directly to your customer service number |
| **Geographic Scope** | Multi-city, multi-state routing with localized tax engines | Laser-focused on 1 initial launch city to ensure operational profitability |

---

## 📅 Milestone Schedule (3 Milestones = ₹1,20,000 Total)

- **Milestone 1 (30% - ₹36,000):** MongoDB Atlas schemas, Express REST APIs, JWT authentication with Role-Based Access Control (RBAC), and React Web Admin Dashboard skeleton (8–10 Working Days).
- **Milestone 2 (40% - ₹48,000):** Unified 3-in-1 Android App development (Customer ordering flow + Vendor order accept/reject with audio alerts + Delivery partner screens with Google Maps & OTP) delivered via test APK (14–16 Working Days).
- **Milestone 3 (30% - ₹36,000):** Razorpay payment gateway integration, server deployment, production `.aab` Google Play Store release handover, and 30-day bug warranty (8–10 Working Days).
