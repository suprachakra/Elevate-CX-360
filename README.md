# Elevate-CX-360

# Table of Contents

[1. Executive Summary](#1-executive-summary)<br>
&nbsp;&nbsp;&nbsp;[1.1 Purpose & Vision](#11-purpose--vision)<br>
&nbsp;&nbsp;&nbsp;[1.2 Strategic Objectives](#12-strategic-objectives)<br>
[2. Product & Ecosystem Scope](#2-product--ecosystem-scope)<br>
[3. Summary of Key Pain Points](#3-summary-of-key-pain-points)<br>
[4. Proposed OKRs for resolving key Pain Points](#4-proposed-okrs-for-resolving-key-pain-points)<br>
[5. Pain Point-To-Priority mapping](#5-pain-point-to-priority-mapping)<br>
[6. Phased Roadmap & Iterative Validation](#6-phased-roadmap--iterative-validation)<br>
&nbsp;&nbsp;&nbsp;[6.1 Phase 1 (0–3 Months): Quick Wins & Foundational Fixes](#61-phase-1-03-months-quick-wins--foundational-fixes)<br>
&nbsp;&nbsp;&nbsp;[6.2 Phase 2 (3–6 Months): Mid-Term Engagement & Efficiency](#62-phase-2-36-months-mid-term-engagement--efficiency)<br>
&nbsp;&nbsp;&nbsp;[6.3 Phase 3 (6–12 Months): Scaling & Intelligence](#63-phase-3-612-months-scaling--intelligence)<br>
&nbsp;&nbsp;&nbsp;[6.4 Phase 4 (12+ Months): Future Innovations & Continuous Optimization](#64-phase-4-12-months-future-innovations--continuous-optimization)<br>
[7. Brand, Marketing, Communications, Compliance Integration](#7-brand-marketing-communications-compliance-integration)<br>
[8. Risk management & Trade-Offs](#8-risk-management--trade-offs)<br>
[9. Features](#9-Features)<br>
&nbsp;&nbsp;&nbsp;[9.1 Passenger-Facing Features](#91-passenger-facing-features)<br>
&nbsp;&nbsp;&nbsp;[9.2 Driver-Facing Features](#92-driver-facing-features)<br>
&nbsp;&nbsp;&nbsp;[9.3 Payment & Backend Features](#93-payment--backend-features)<br>
&nbsp;&nbsp;&nbsp;[9.4 Operational & Misc. Improvements](#94-operational--misc-improvements)<br>

### **1. Executive Summary**

#### **1.1 Purpose & Vision**  
- **Purpose**: Deliver an industry-defining **Customer Excellence Ecosystem (CEE)** that revolutionizes how passengers, drivers, and our internal teams experience the ride-hailing platform.  
- **Vision**: Become the **global benchmark** in mobility, seamlessly blending **personalized UX**, **proactive driver excellence**, **robust compliance**, and **brand synergy**—all supported by **advanced analytics** and **iterative improvement**.


#### **1.2 Strategic Objectives**

| **Objective**                                     | **Key Result (KR)**                                                                                                |
|---------------------------------------------------|---------------------------------------------------------------------------------------------------------------------|
| **1. Attain Best-in-Class CX Metrics**            | - **KR1.1:** Increase NPS from current baseline to **+20** within 12 months. <br> - **KR1.2:** Maintain **≥90%** CSAT in top markets. |
| **2. Ensure Scalable, Adaptable Architecture**    | - **KR2.1:** Achieve **99.99%** uptime <br> - **KR2.2:** Pass all major **compliance audits** (GDPR, PDPA, CCPA) with **0** critical findings.  |
| **3. Foster Loyal User & Driver Communities**     | - **KR3.1:** Grow monthly active loyal users (≥X rides/mo) by **25%** in 9 months <br> - **KR3.2:** **50%** of new signups come from **referrals** by 12 months. |
| **4. Integrate Advanced Feedback Loops**          | - **KR4.1:** 100% of major features tested via **prototypes, A/B** or **pilot** prior to global rollout <br> - **KR4.2:** 80% of roadmap updates influenced by **data insights** from feedback loops. |

> **Why This Matters**: Ties every initiative to measurable business impact; ensures clarity on expected deliverables and standards for success.

---

### **2. Product & Ecosystem Scope**

#### **2.1 Current State Audit**  
- **User Journeys**: Booking flows, fare transparency, in-ride experience, driver interactions, post-ride feedback & loyalty.  
- **Operational Processes**: Customer Support (CS), driver onboarding, marketing campaigns, QA, compliance checks, brand messaging.  
- **Technology Stack**: Mobile apps (iOS/Android), back-end services, data pipelines, analytics, Mobile Data Terminals, CRM, and legal compliance modules.

#### **2.2 Future State Aspirations**  
- **Seamless, Personalized UX**: Users feel the platform “knows” them, from pick-up preferences to loyalty rewards.  
- **Proactive Support & Driver Excellence**: Issues get resolved before users escalate, drivers are thoroughly trained, monitored, and rewarded.  
- **Global Scalability with Local Compliance**: Region-specific data residency and privacy compliance without hindering growth.  
- **Brand & Marketing Synergy**: A cohesive narrative that reaffirms trust, safety, and user empowerment.

---

### **3. Summary of Key Pain Points**

The table below consolidates **app store feedback** and user complaints, grouped by category. **Names have been removed** to protect user privacy. Where direct quotes are available, we have redacted identifying details.

| **Category**                 | **Pain Point / Issue**                                                               | **User Impact / Example Quotes**                                                                                                                            | **Potential Root Cause**                                                                                                                  |
|------------------------------|---------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------|
| **A. Location & Navigation** | 1. Drivers unable to find pick-up/drop-off locations accurately                      | - “Every time I book and put in the location in the app, the driver still calls me… I had to cancel a ride because he was lost.”<br/>- Some users are late due to navigation errors.    | - App’s location database incomplete or inaccurate <br/>- Communication gap between passenger & driver <br/>- Possibly missing 7-seater option in some areas |
|                              | 2. Destination search not functioning / can’t find addresses                         | - “Destination search not working.”                                                                                                                        | - Inadequate geocoding service <br/>- Lack of robust address coverage <br/>- Potential bugs in search integration                         |
|                              | 3. Drivers complaining the map is slow/confusing                                     | - “The driver was lost and forced me to cancel.”                                                                                                           | - Outdated map data or poor UI design <br/>- Possibly older onboard hardware (MDT)                                                       |
| **B. Booking & Dispatch**    | 1. Long wait times or no driver assigned, rides cancelled last minute                | - “Never get driver on time,” or “He canceled 15 mins before pick-up.”                                                                                     | - Insufficient driver supply <br/>- Poor dispatch algorithm <br/>- No real-time matching or surge mechanism                              |
|                              | 2. Scheduled rides failing at the last moment                                       | - “It was canceled from their side, claiming they couldn’t find a driver.”                                                                                 | - Inadequate scheduling logic <br/>- No fallback or driver incentives for scheduled trips                                                 |
| **C. Fare & Pricing**        | 1. Complaints about high fares or inconsistent pricing                              | - “The fare is noticeably higher than other ride-hailing apps.”                                                                                            | - No transparent fare breakdown <br/>- Possibly outdated or rigid fare structure                                                         |
|                              | 2. Double charge or promo code not applied / “scam” perception                      | - “I get charged in advance, then have to pay full in cash.”                                                                                               | - Poor integration of wallet/promo logic <br/>- Buggy pre-auth and refund flow                                                           |
| **D. Payment & Refund**      | 1. Difficulty adding credit cards, double-charging, delayed refunds                  | - “They charged a small amount each time, but it declined anyway.”                                                                                        | - Unclear payment validation or unsettled pre-auth <br/>- Possibly not integrated with all card networks                                 |
|                              | 2. No easy online payment or certain features missing                               | - “Can’t pay online, can’t book multiple rides.”                                                                                                          | - Payment gateway limitations <br/>- Feature restrictions in back-end architecture                                                       |
| **E. App Performance & UX**  | 1. Slow app, frequent crashes, buggy features                                       | - “The app is super slow… might as well walk.”                                                                                                             | - Possible performance bottlenecks <br/>- Poor front-end optimization <br/>- High server response times                                 |
|                              | 2. Certain features not working (login errors, suspicious activity)                 | - “Can’t login,” “keeps giving suspicious activity error.”                                                                                                 | - Authentication process issues <br/>- Phone verification service failing                                                                |
| **F. Support & Communication** | 1. No direct way to contact driver or complicated IVR system                      | - “There is no way to call the driver; if you call customer care, it’s all press blah blah.”                                                               | - Missing in-app call/chat feature <br/>- Confusing support flow or phone routing system                                                 |
|                              | 2. Support not resolving issues or slow to respond                                  | - “Team does nothing to solve the issue,” “Weak or not working support.”                                                                                   | - Possibly understaffed or overburdened support <br/>- Lacking closed-loop feedback tracking                                             |
| **G. Driver Behavior**       | 1. Drivers cancel for “better fare,” or cheat by longer routes                      | - “Driver canceled on a busy evening for a better fare,” or “They move from big road to charge more.”                                                      | - Driver incentive/motivation structure flawed <br/>- Weak compliance/monitoring system                                                  |
|                              | 2. Unprofessional conduct or frustration from driver side                          | - “Drivers treat you poorly,” “Driver not professional.”                                                                                                   | - Inadequate driver training & guidelines <br/>- No robust rating-based penalty or reward system                                         |
| **H. Vehicle & Service**     | 1. No 7-seater or normal taxi (only limos)                                         | - “No option to book 7 seater public taxi,” or “It’s only private limousines.”                                                                             | - Fleet limitation or app not exposing correct vehicle types <br/>- Possibly not integrated with normal taxi supply                      |
| **I. General Dissatisfaction** | 1. Overall “worst app,” “bad experience,” “garbage,” etc.                          | - “Why is there no zero star?” <br/>- “Worst service,” “Stupid app.”                                                                                      | - Accumulated frustration from the above issues <br/>- Poor brand perception, negative word-of-mouth                                     |

---

### **4. Proposed OKRs for resolving key Pain Points**

| **Objective (O)**                                         | **Key Results (KR)**                                                                                         |
|-----------------------------------------------------------|---------------------------------------------------------------------------------------------------------------|
| **O1. Enhance Location Accuracy & Dispatch Efficiency**   | **KR1.1:** Reduce “driver can’t find location” complaints by **50%** within 9 months <br/>**KR1.2:** Decrease average waiting time to < **5 minutes** for 70% of rides |
| **O2. Provide Clear, Fair, and Transparent Pricing**      | **KR2.1:** Slash fare dispute tickets by **60%** in 3 months <br/>**KR2.2:** Achieve ≤ **2%** double-charge or refund complaints |
| **O3. Improve App Stability & Payment Integration**       | **KR3.1:** < **1%** crash rate across devices within 4 months <br/>**KR3.2:** Decrease “unable to add card” or “payment declined” errors by **70%** in 6 months       |
| **O4. Strengthen Customer Support & Driver Communication**| **KR4.1:** Implement in-app call/chat with drivers, reduce “unable to contact driver” complaints by **80%** <br/>**KR4.2:** **90%** of support tickets resolved or updated within 24 hours |
| **O5. Elevate Driver Satisfaction & Professionalism**      | **KR5.1:** Decrease driver cancellation rate to < **5%** <br/>**KR5.2:** Introduce rating/incentive scheme; driver rating ≥ **4.5/5** for **80%** of drivers          |
| **O6. Expand Service Offering & Vehicle Options**         | **KR6.1:** Launch 7-seater or normal taxi options in-app within 12 months <br/>**KR6.2:** At least **15%** of monthly rides from new vehicle categories                |

---

### **5. Pain Point-To-Priority mapping**

The table below **maps each pain point** to relevant OKRs and assigns **priority** (High, Medium, or Low) based on **customer impact** and **frequency** of complaints. **Recommended Actions** appear in the last column.

| **Pain Point**                                                    | **OKR Link**               | **Priority** | **Recommended Actions**                                                                                                                      |
|-------------------------------------------------------------------|----------------------------|--------------|----------------------------------------------------------------------------------------------------------------------------------------------|
| **A1. Drivers unable to find location**                           | O1 (Location & Dispatch)   | High         | - Upgrade map/geocoding services <br/>- Provide lat/long pin drop <br/>- Possibly add location guidance photos and “report inaccurate map”   |
| **A2. Destination search fails**                                  | O1 (Location & Dispatch)   | High         | - Debug address API coverage <br/>- Allow manual “custom location” if search fails                                                           |
| **B1. Long wait / no driver**                                     | O1 (Location & Dispatch)   | High         | - Refine dispatch algorithm <br/>- Introduce surge or driver incentives at high-demand times                                                 |
| **B2. Failed scheduled rides**                                    | O1 (Location & Dispatch)   | Medium       | - Guaranteed scheduling with fallback driver pool <br/>- Better driver incentives for scheduled pickups                                      |
| **C1. High or inconsistent fares**                                | O2 (Transparent Pricing)   | High         | - Show itemized fare estimate (distance, surcharges) <br/>- Possibly revise base rates or cap surcharges                                     |
| **C2. Double charge / discount glitch**                           | O2 (Transparent Pricing)   | High         | - Fix pre-auth & refund flow <br/>- Validate promo codes upfront <br/>- Show “final amount” at booking                                       |
| **D1. Payment card issues & refunds**                             | O3 (Stability & Payment)   | High         | - Integrate stable payment gateway <br/>- Track & automate refunds <br/>- Provide status updates via push notification                       |
| **D2. No easy online payment**                                    | O3 (Stability & Payment)   | Medium       | - Expand supported payment methods <br/>- Offer e-wallet or saved card functionality                                                         |
| **E1. Slow/buggy app**                                           | O3 (Stability & Payment)   | High         | - Performance optimization & caching <br/>- Update server infra & front-end load times                                                      |
| **E2. Login errors, suspicious activity**                         | O3 (Stability & Payment)   | Medium       | - Revamp phone verification <br/>- Offer multi-factor fallback                                                                              |
| **F1. No direct driver contact**                                  | O4 (Support & Driver Comm) | High         | - Implement in-app call/chat <br/>- Show real-time driver status updates                                                                     |
| **F2. Weak/unhelpful support**                                   | O4 (Support & Driver Comm) | High         | - Closed-loop support system <br/>- SLA for complaint resolution <br/>- Real-time ticket tracking                                            |
| **G1. Driver cancels for better fare**                            | O5 (Driver Satisfaction)    | High         | - Incentive/penalty system <br/>- Tie acceptance rates to driver score <br/>- Possibly surge pay for peak times                              |
| **G2. Unprofessional driver conduct**                             | O5 (Driver Satisfaction)    | Medium       | - Mandatory training, rating feedback <br/>- Warnings or suspensions for repeated unprofessional behavior                                    |
| **H1. No normal taxi or 7-seater**                                | O6 (Expand Services)        | Medium       | - Integrate additional vehicle types <br/>- Onboard partners for 7-seater fleet                                                              |
| **I1. Overall “worst app” frustration**                           | Multiple OKRs              | N/A          | - Symptomatic of above <br/>- Fix root issues systematically                                                                               |

---

### **6. Phased Roadmap & Iterative Validation**

We propose an **agile approach** with short sprints for quick wins, followed by incremental expansions for bigger features. 

---
#### **6.1 Phase 1 (0–3 Months): Quick Wins & Foundational Fixes**
---

- **Location & Search Enhancements**  
  - *Front-end revamp of pin drop*, *Improving PUDO*, “Report Address” feature  
- **Payment & Pricing**  
  - Fix double-charge glitch, refine promo code flow  
  - “Swap Pickup & Drop Off” (quick win)  
- **Basic Support Improvements**  
  - In-app call or chat with driver (MVP)  
- **Driver-Facing**  
  - “Refresh/Quick Check” in driver home screen to mitigate app hang  
  - Simple driver incentive pilot

**Validation**:  
- A/B test new location pin drop vs. old interface  
- Monitor dispute rates & cancellation logs weekly  
- Gather driver and passenger feedback via quick in-app surveys

---
#### **6.2 Phase 2 (3–6 Months): Mid-Term Engagement & Efficiency**
---

- **Transparent Pricing & Surge**  
  - Dynamic pricing for peak times, itemized breakdown in booking  
- **Driver App & Scheduling**  
  - Dispatch algorithm overhaul (efficient matching)  
  - Guaranteed scheduling for advanced bookings  
- **Advanced Payment Options**  
  - E-wallet integration, stable gateway for multiple card networks  
- **Support & Driver Communication**  
  - Fully implement “Closed-Loop Feedback,” driver incentive announcements  

**Validation**:  
- Compare average wait times, NTA rates pre- vs. post-dispatch upgrade  
- Track e-wallet usage & user satisfaction  
- Weekly sprints with pilot test groups for scheduling reliability

---
#### **6.3 Phase 3 (6–12 Months): Scaling & Intelligence**
---

- **Driver Professionalism & Behavior**  
  - Standardized driver training, rating resets, and AR-based modules (if feasible)  
- **Vehicle Options**  
  - Launch 7-seater or normal taxi in select markets  
- **Performance & UX**  
  - Full code audit for slow app issues, scale up server capacity  
  - Possibly release “search location using image” as an innovation pilot

**Validation**:  
- Weekly data scrums analyzing driver rating distribution, user churn, wait times  
- Focus-group feedback on 7-seater or normal taxi usage

---
#### **6.4 Phase 4 (12+ Months): Future Innovations & Continuous Optimization**
---

- **Advanced Features**  
  - AI Chat/Helpdesk for complex queries, voice input for search fully rolled out  
  - Real-time forecast notifications for weather/demand on driver home screen  
- **Global Architecture**  
  - Expand to lat/long dispatch fully if new markets are targeted (postal code fallback only)  
- **Brand & Marketing**  
  - Integrate referral systems for both pax & driver, subscription-based plans at scale

**Validation**:  
- Track OKR completion, especially improved NPS, driver acceptance rate, dynamic pricing uptake  
- Routine compliance checks to ensure no major infractions

---

### **7. Brand, Marketing, Communications, Compliance Integration**

1. **Brand & Marketing**  
   - **Campaign Themes**: Emphasize transparency (“no hidden charges”), innovative app features (7-seater, quiet trip toggle), strong driver training.  
   - **Referral & Loyalty Push**: Use “Subscription-Based Plans,” “Refer-a-Friend” for passengers, and “Refer a Friend for Driver” to boost viral growth.

2. **Communications**  
   - **Crisis Management**: If dynamic pricing triggers negative media coverage, respond with data or revert temporarily.  
   - **Proactive Messaging**: For each major release (e.g., new driver incentives), in-app notifications, push messages, or short “How-to” videos.

3. **Compliance & Data Governance**  
   - **Privacy-by-Design**: Ensure user data for personalization or AI-based helpdesk is anonymized or aggregated.  
   - **Audit Trails**: Log location overrides, fare adjustments for dispute resolution.  
   - **Global Regulations**: If expanding beyond local markets, confirm GDPR/PDPA compliance for data management.

4. **QA & Security**  
   - **Continuous Integration**: Automated test suites for each new feature branch.  
   - **Penetration Testing**: Payment, wallet, and personal data must remain secure.  
   - **Load Testing**: Dynamic pricing or big events might spike traffic; ensure backend scalability.

---

### **8. Risk management & Trade-Offs**

| **Risk**                                    | **Potential Impact**                                        | **Mitigation**                                                                                                 | **Contingency Plan**                                                                              |
|--------------------------------------------|-------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| **Regulatory Shifts**                      | Might require rework of pricing algorithms or data storage | - Maintain compliance squad <br/>- Regularly review local laws                                                  | - Quick compliance sprints if new legislation emerges                                              |
| **Driver Resistance to New Features**      | Low adoption of advanced training, surge acceptance         | - Incentives, gamification, training modules <br/>- Co-create solutions with drivers                            | - Offer “lite” options if drivers refuse <br/>- Delay rollout if pilot adoption is too low         |
| **Performance Bottlenecks**                | Sluggish app or server crashes under load                  | - Cloud auto-scaling <br/>- Pre-deployment load testing                                                         | - Roll back to stable version if performance dips below set threshold                               |
| **Data Overload / Privacy Concerns**       | Bad user trust if data is mismanaged                       | - Store minimal PII <br/>- Clear user consent flows                                                            | - Temporarily disable personalized features if data governance issues arise                        |
| **Competitive Pressure**                   | Users might switch to alternatives                         | - Offer distinctive features (quiet ride, 7-seater, loyalty passes)                                            | - Accelerate new feature releases or dynamic pricing adjustments if competitor’s rates shift       |
| **Driver or Pax Fraud**                    | Fake rides, abuse of referral or promo codes               | - Real-time fraud detection <br/>- Cap promo usage, phone/email verification                                   | - Immediately freeze suspicious accounts <br/>- Fine-tune referral rules to reduce abuse           |

---

### **9. Features**

---

#### **9.1 Passenger-Facing Features**

| **Feature/Idea**                             | **Problem Solved**                                                                                                                                | **Proposed Approach**                                                                                                                                                              | **OKR Link**                              | **Potential Impact**                                                                        | **Priority**            |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------|----------------------------------------------------------------------------------------------|-------------------------|
| **Cancellation Policy**                     | Wasted driver time if passenger cancels; passenger stress if driver cancels.                                                                      | - Define transparent, tiered cancellation fees (both driver & pax).<br/>- Show policy in-app with rationale.                                                                        | **Obj 1 (CS), Obj 3 (Drv)**               | - 10% fewer “unfair cancellation” disputes<br/>- More trust in booking reliability.           | **Small (1–3 Months)** |
| **Dynamic Pricing**                         | Pricing mismatch in peak hours, driver dissatisfaction, passenger struggles.                                                                      | - Surge factors based on supply-demand indicators.<br/>- Display reason for surge.                                                                                                  | **Obj 2 (Ops), Obj 4 (Rev)**              | - 15% improvement in NTA<br/>- Boosts revenue & driver acceptance.                            | **Medium (3–6 Months)** |
| **Front End Revamp of Location Pin Drop**   | Pax can drag pin anywhere, but dispatch only works for addresses in address service.                                                              | - UI snaps pin to valid addresses or “nearest recognized point.”<br/>- Show error if out of coverage.                                                                               | **Obj 1 (CS), Obj 2 (Ops)**               | - Reduces mis-dispatches <br/>- Less driver frustration.                                      | **Small (1–3 Months)** |
| **Improve our PUDO List**                   | Inaccurate lat/long, coverage gaps (complex building entrances).                                                                                  | - Continuously update PUDO database with correct coordinates.<br/>- Crowdsource from drivers/pax.                                                                                  | **Obj 1 (CS), Obj 3 (Drv)**               | - 20% drop in “can’t find you” calls <br/>- Smoother ride starts.                              | **Medium (3–6 Months)** |
| **Subscription-Based Plans**                | Passengers want consistent discounts or assured rides.                                                                                            | - Offer monthly/weekly passes with discounted rides, priority booking, free cancellations.                                                                                        | **Obj 4 (Rev)**                            | - +10–20% recurring revenue <br/>- Strong brand loyalty.                                       | **Medium (3–6 Months)** |
| **Promocode Flow Improvements**             | Current flow fails or confuses users, leading to frustration.                                                                                     | - Validate promo in real-time before “Book Now.”<br/>- Show discount or error up front.                                                                                             | **Obj 1 (CS), Obj 4 (Rev)**               | - +5 points user satisfaction <br/>- Lower cart abandonment.                                   | **Small (1–3 Months)** |
| **Push Notification Revamp**                | Pax confused about ride status (pre-auth, driver confirm, trip start/end).                                                                         | - Event-based push notifications for each key step.<br/>- Clear status in push or in-app alerts.                                                                                    | **Obj 1 (CS)**                             | - 30% fewer “Where is my driver?” queries <br/>- Higher clarity → improved NPS.               | **Small (1–3 Months)** |
| **Silent Trip / “No Talk” Option**          | Some passengers want a quiet ride but hesitate to ask.                                                                                           | - Toggle for “Quiet Trip” or “No music.”<br/>- Discreet driver notification.                                                                                                       | **Obj 1 (CS)**                             | - Enhanced comfort, brand differentiator.                                                     | **Small (1–3 Months)** |
| **Tips Selection After Trip**               | Missed tip opportunities, unrecognized driver service.                                                                                            | - Post-trip tipping screen (preset amounts, custom).<br/>- Show driver rating, then tip prompt.                                                                                     | **Obj 3 (Drv)**                            | - 10–20% of rides yield tips, driver morale.                                                  | **Small (1–3 Months)** |
| **More Vehicle Types (Pet Friendly, Ladies, EV)** | Some passengers want female drivers, need pet-friendly or prefer EV.                                                                                | - Expand vehicle-type filters.<br/>- Ensure verified driver categories.                                                                                                             | **Obj 1 (CS), Obj 3 (Drv)**               | - Capture niche segments (pet owners, women travelers, eco-conscious). <br/>- +15% sign-ups.   | **Medium (3–6 Months)** |
| **Voice Input for Search Bar**              | Elderly or busy users find typing addresses tough.                                                                                                | - Integrate OS-level voice recognition, test adoption vs. typed entry.                                                                                                              | **Obj 1 (CS)**                             | - 5–10% uplift in completed searches, improved accessibility.                                  | **Small (1–3 Months)** |
| **Let Pax Choose the Car in Map or List**   | Some want to pick a specific nearby car instead of random dispatch.                                                                               | - Provide “list of nearby drivers” or a “map click” to pick a certain driver.                                                                                                        | **Obj 1 (CS)**                             | - Unique selling point, sense of user control.                                                 | **Medium (3–6 Months)** |
| **Book Multiple Car Categories**            | Pax can only select 1 category at a time, prolonging search if that category is unavailable.                                                      | - Allow selecting multiple categories (Standard, Premium, EV) in parallel.                                                                                                           | **Obj 1 (CS), Obj 2 (Ops)**               | - Reduced search times, fewer cancellations.                                                  | **Medium (3–6 Months)** |
| **Refer-a-Friend for Pax**                  | Missing referral mechanism, losing viral growth.                                                                                                  | - Add referral codes or “share app” links with immediate credit.                                                                                                                    | **Obj 4 (Rev)**                            | - ~20% jump in signups from referrals.                                                          | **Small (1–3 Months)** |
| **Make Cancel Button Responsive**           | Some users can’t cancel during “searching,” leading to frustration.                                                                               | - Enable quick-cancel or confirm “searching, are you sure?” with short cooldown.                                                                                                    | **Obj 1 (CS)**                             | - More user control, fewer forced rides.                                                        | **Quick Win (2–4 Weeks)** |

---

#### **9.2 Driver-Facing Features**

| **Feature/Idea**                            | **Problem Solved**                                                                                                                  | **Proposed Approach**                                                                                                                                      | **OKR Link**                         | **Potential Impact**                                                                                     | **Priority**                |
|--------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------|----------------------------------------------------------------------------------------------------------------|-----------------------------|
| **Driver Incentive**                        | Drivers lack motivation to accept certain jobs; no structured incentive or tracking.                                               | - Incentive “CMS” to track progress, show how many rides left to bonus.                                                                                     | **Obj 3 (Drv)**                      | - +15% acceptance on less popular routes/times <br/>- Stronger driver loyalty.                                | **Small (1–3 Months)**      |
| **Build an Efficient Dispatch Algorithm**   | High NTA (no taker available), driver wasting time traveling to pickups, mismatch of supply/demand.                                 | - Advanced matching: consider distance, traffic, driver rating. Possibly ML for dynamic optimization.                                                      | **Obj 2 (Ops), Obj 3 (Drv)**         | - 20% drop in NTA <br/>- Faster job confirmations, better resource utilization.                               | **Medium (3–6 Months)**     |
| **Change Postal Code Dependency to Lat/Long** | Postal code only works in certain locales; not scalable for expansions.                                                               | - Migrate location logic to lat/long-based search & pricing. Deprecate postal code usage except as fallback.                                              | **Obj 2 (Ops)**                      | - Scalable for new markets, fewer address mismatches.                                                         | **Large (6+ Months)**       |
| **Driver App Radar → Map**                  | Radar is purely visual, doesn’t help navigation.                                                                                    | - Replace with actual map or “hot zones” insight for drivers.                                                                                               | **Obj 3 (Drv), Obj 2 (Ops)**         | - Drivers feel more informed, less random waiting.                                                             | **Small (1–3 Months)**      |
| **Driver Inbox Enhancement**                | Current driver comms via SMS or external channels → missing updates.                                                                 | - Add “Inbox” in driver app for announcements, policy updates, incentives.                                                                                 | **Obj 3 (Drv)**                      | - Better driver engagement, fewer missed messages.                                                             | **Small (1–3 Months)**      |
| **MDT Replacement**                         | Outdated hardware limiting new features (Google Maps, Waze).                                                                         | - Phase out old MDT with a tablet/smartphone solution. <br/>- Offer hardware lease or subsidy.                                                              | **Obj 2 (Ops), Obj 3 (Drv)**         | - Enables advanced features (AR nav, real-time updates).                                                       | **Large (6+ Months)**       |
| **Driver Schedule & Relocation**            | Drivers stuck in low-demand areas, complaining no jobs.                                                                              | - Show forecast demand zones, encourage relocation. <br/>- Possibly reward drivers who move to underserved areas.                                          | **Obj 2 (Ops), Obj 3 (Drv)**         | - 15% fewer idle drivers, improved coverage in hot spots.                                                      | **Medium (3–6 Months)**     |
| **Driver App System Health Check**          | App hang or stuck jobs cause “no job requests” illusions.                                                                            | - “Refresh” button + background checks to ensure driver’s account is active, no stuck states.                                                               | **Obj 2 (Ops)**                      | - Less driver frustration, fewer support calls.                                                                 | **Small (1–3 Months)**      |
| **In-App Navigation** for Taxi Drivers      | Drivers must toggle to external navigation, risking missed updates.                                                                 | - Integrate major map providers directly in driver app.                                                                                                     | **Obj 2 (Ops), Obj 3 (Drv)**         | - Safer driving, 5% improvement in on-time arrivals.                                                            | **Medium (3–6 Months)**     |
| **Link Ratings to Incentives + Periodic Reset** | Drivers demoralized by permanent low ratings, no chance to improve.                                                                   | - Reset negative contributions after a set period. <br/>- Offer rating-based incentives (priority dispatch, bonuses).                                       | **Obj 3 (Drv)**                      | - Motivates performance improvement, fosters rating recovery.                                                   | **Small (1–3 Months)**      |
| **Allow Driver to Register Directly in App** | Current driver signup is offline, slow, limiting driver supply.                                                                      | - Full digital onboarding: ID verification, license scan, direct bank details.                                                                             | **Obj 2 (Ops), Obj 3 (Drv)**         | - Shortens signup from days to hours, bigger driver pool.                                                       | **Medium (3–6 Months)**     |
| **Driver Marketplace**                       | Potential hirers or leasees can’t easily find relief drivers, reducing usage.                                                        | - In-app marketplace with profiles, ratings, schedules for short/long-term relief.                                                                          | **Obj 3 (Drv)**                      | - Increases taxi availability, fosters driver community.                                                        | **Medium (3–6 Months)**     |

---

#### **9.3 Payment & Backend Features**

| **Feature/Idea**                    | **Problem Solved**                                                                                                   | **Proposed Approach**                                                                                                                                               | **OKR Link**              | **Potential Impact**                                                                  | **Priority**           |
|-------------------------------------|-----------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------|----------------------------------------------------------------------------------------|------------------------|
| **Payment: Pre-Auth & Cancel Auth** | Unclear or partial payment holds/cancellations leading to overcharges or uncharged rides.                             | - Streamline pre-auth: auto-release on cancel or capture only at trip end.<br/>- Add robust “linked job” logic for multi-trip or partial charge scenarios.          | **Obj 1 (CS), Obj 4 (Rev)** | - Fewer disputes, less friction in checkout.                                          | **Medium (3–6 Months)** |
| **E-Wallet Integration**            | Potential new revenue + simpler refunds, cancellations, loyalty usage.                                               | - Create in-app wallet with top-ups (card, bank).<br/>- Integrate loyalty points and promo credits.                                                                 | **Obj 4 (Rev)**           | - Encourages recurring usage, simpler refunds, brand stickiness.                      | **Medium (3–6 Months)** |
| **Smart Call (Pricing & Fare Adjust)** | Drivers say fares are too low; pax say no drivers accept.                                                             | - Implement real-time or near-real-time fare adjustments based on supply/demand.                                                                                    | **Obj 2 (Ops), Obj 3 (Drv)** | - Balances driver satisfaction vs. passenger acceptance.                               | **Medium (3–6 Months)** |
| **Swap Pickup & Drop Off**          | Users sometimes reverse addresses, causing re-entry or confusion.                                                    | - One-click “swap” in booking flow.                                                                                                                                 | **Obj 1 (CS)**            | - Fewer errors, improved booking flow.                                                | **Quick Win (2–4 Weeks)** |
| **Report Address**                  | Some addresses are incomplete or missing, leading to repeated frustration.                                           | - “Report issue” for addresses to store geocoded data for corrections.<br/>- Possibly incentivize accurate reporting by drivers/pax.                                | **Obj 1 (CS), Obj 2 (Ops)** | - Gradually improved address DB, fewer misroutes.                                      | **Small (1–3 Months)** |
| **New Transaction History (Drivers)**| Drivers uncertain about each trip’s payout, current system lumps all together.                                       | - Overhaul statements: itemize each trip, tip, incentive, fee.                                                                                                      | **Obj 3 (Drv)**           | - Improves driver trust, fewer finance-related complaints.                             | **Small (1–3 Months)** |

---

#### **9.4 Operational & Misc. Improvements**

| **Feature/Idea**                                      | **Problem Solved**                                                                                  | **Proposed Approach**                                                                                                          | **OKR Link**                 | **Potential Impact**                                                                        | **Priority**              |
|-------------------------------------------------------|------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------|-----------------------------|--------------------------------------------------------------------------------------------|---------------------------|
| **Streethail Pairing**                                | Slow or confusing pairing for on-street pick-ups.                                                   | - Optimize pairing logic, instant update in passenger app <br/>- Simplify error messages                                       | **Obj 1 (CS), Obj 3 (Drv)**  | - Faster on-street matching, less frustration.                                             | **Small (1–3 Months)**    |
| **Pax Push Notification Enhancement**                  | Pax not informed of final capture or pre-auth hold release.                                          | - Add final capture push, clarify any hold release.                                                                            | **Obj 1 (CS)**              | - 30% fewer “why was I charged?” queries                                                   | **Small (1–3 Months)**    |
| **Search Location Using Image**                        | Some users can’t articulate addresses, can show a photo.                                             | - Integrate basic image recognition or manual curation for known landmarks.                                                   | **Obj 1 (CS)**              | - Unique feature for tourists or visually oriented users.                                  | **Large (6+ Months)**     |
| **Some popular pickup points show guide photos**       | Confusion at large malls, airports, etc.                                                             | - Attach official or user-submitted photo guides to PUDO.                                                                      | **Obj 1 (CS), Obj 3 (Drv)** | - Smoother pickups, fewer “wrong entrance” calls.                                          | **Small (1–3 Months)**    |
| **Inaccurate Mapping or Address**                      | Poor directions or inability to find location.                                                       | - Upgrade map provider or refresh data <br/>- Encourage driver “report inaccurate map.”                                        | **Obj 1 (CS), Obj 2 (Ops)** | - Lower arrival times, fewer cancellations, improved trust.                                | **Medium (3–6 Months)**   |
| **Event Notifications to Drivers**                     | Drivers unaware of high-demand event venues or weather-based spikes.                                 | - Integrate weather & event data. <br/>- “Heads up” notifications for local demands.                                          | **Obj 2 (Ops), Obj 3 (Drv)**| - 20% better distribution of drivers in needed areas, reducing wait times & NTAs.          | **Small (1–3 Months)**    |
| **Supply Planning with Drivers**                       | Low supply at peak times.                                                                            | - Historical demand forecasting, driver shift scheduling <br/>- Incentives for covering underserved timeslots.                | **Obj 2 (Ops), Obj 3 (Drv)**| - Better supply coverage, ~15% improved acceptance rates.                                   | **Medium (3–6 Months)**   |
| **AJ Workflow Review**                                 | Advanced booking “AJ” not user-friendly; unclear notifications.                                      | - Redesign push flow for clear driver assignment <br/>- Possibly allow T+0 immediate advanced requests.                        | **Obj 1 (CS), Obj 2 (Ops)** | - 25% fewer “Where is my advanced booking?” calls.                                         | **Small (1–3 Months)**    |
| **Driver Onboarding**                                  | Takes 3 days, especially for short-term rental drivers, limiting supply.                             | - Digitize KYC, license checks (like competitors). <br/>- Offer e-contracts, fast approvals.                                   | **Obj 2 (Ops), Obj 3 (Drv)**| - 20–30% more monthly signups, faster ramp-up.                                             | **Small (1–3 Months)**    |
| **Login Revamp**                                       | Users lose accounts or payment info upon device change, re-creating user ID.                          | - Phone/email-based unique ID, store payment backend.                                                                          | **Obj 1 (CS), Obj 4 (Rev)** | - Fewer duplicates, improved continuity across devices.                                    | **Small (1–3 Months)**    |
| **Tie Payment to User ID**                             | Payment details vanish if app is deleted or user logs out.                                           | - Keep card/e-wallet info securely on server side <br/>- On re-login, auto-sync payment.                                      | **Obj 1 (CS), Obj 4 (Rev)** | - Less friction re-adding payment, fosters loyalty.                                        | **Small (1–3 Months)**    |
| **In-App AI Chat/Helpdesk**                            | No quick solution for Pax or Drivers, slow calls or IVR.                                             | - Build or integrate AI helpbot with escalation to real chat.                                                                 | **Obj 1 (CS)**             | - 40% less call center load, faster resolution.                                            | **Medium (3–6 Months)**   |
| **Refresh + Quick Function Check in Driver Home**       | Drivers fear no jobs due to potential app freeze, not actual supply shortage.                         | - “Refresh now” button to re-initiate connection, flush any stuck queue.                                                      | **Obj 3 (Drv)**            | - Reduced anxiety, fewer “why no jobs?” calls.                                             | **Quick Win (2–4 Weeks)** |
| **Make essential driver app functions persistent On-Call** | Hard to access Chat/Help/Cancel on multi-destination rides.                                            | - Pin these essential buttons at top or bottom.                                                                               | **Obj 3 (Drv)**            | - Safer driving, less UI fiddling mid-trip.                                                | **Small (1–3 Months)**    |
| **Incentive Announcement & Tracking**                   | Drivers not aware of new incentives or how close they are to achieving them.                           | - Real-time display: “X rides to get $Y bonus.” <br/>- In-app notifications or panel.                                         | **Obj 3 (Drv)**            | - +10% acceptance on incentive-based trips, clarity for drivers.                           | **Small (1–3 Months)**    |
| **Include Red Prompt for Payment at End Trip**          | Some taxi drivers forget to collect onboard payments.                                                 | - Explicit “Collect Payment” prompt on driver app after “End Trip.”                                                            | **Obj 3 (Drv), Obj 4 (Rev)**| - Minimizes unpaid rides, better driver earnings.                                          | **Quick Win (2–4 Weeks)** |
| **Provide Demand & Weather Forecast on Driver Home**     | Drivers unaware of upcoming demand spikes or storms.                                                  | - Show 30-min forecast for weather + typical demand spikes.                                                                    | **Obj 2 (Ops), Obj 3 (Drv)**| - Better distribution of supply, shorter wait times, improved driver earnings.             | **Small (1–3 Months)**    |
| **Improve Formatting for PUDO Display**                 | PUDO addresses in ALL CAPS or too long, causing confusion.                                             | - Standardize format, break lines logically, add icons for malls/airports.                                                    | **Obj 1 (CS)**             | - Clearer instructions, fewer misunderstandings.                                           | **Quick Win (2–4 Weeks)** |
| **Allow Drivers to Report Bad/Missing Locations**        | Some pick-up points off-limits or unlisted.                                                            | - “Report location” button in driver app, automatically flagged for map DB update.                                            | **Obj 2 (Ops)**            | - Gradual improvement in location data.                                                   | **Small (1–3 Months)**    |
| **Refer a Friend for Driver**                           | No referral system for drivers to bring in new recruits.                                               | - Similar to passenger referral: unique driver code + bonus for both.                                                         | **Obj 3 (Drv)**            | - +10–15% driver growth from word-of-mouth.                                               | **Small (1–3 Months)**    |
| **Driver Onboarding via App**                           | Offline driver sign-up is slower vs. competitors.                                                      | - KYC doc uploads, e-sign contracts, near-instant approvals or manual review.                                                 | **Obj 3 (Drv)**            | - Faster ramp-up, more driver availability.                                              | **Small (1–3 Months)**    |

---


---

### **NEXT STEPS**

1. **Cross-Functional Sign-Off**: PRD to Product, Marketing, Engineering, Legal/Compliance, and Operations. Collect feedback, finalize.  
2. **Detailed Sprint/PI Planning**: Translate the identified features and timelines into actual SAFe sprint or PI backlog items.  
3. **Pilot Execution**: Select initial regions or user segments for pilot programs (e.g., fare transparency, loyalty revamp) to validate immediate assumptions.  
4. **Monitoring & Course-Correction**: Continuously monitor metrics. If they deviate from targets, adapt quickly in the next iteration or sprint.

---
