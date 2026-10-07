# OYO Product Teardown: Group Booking Experience (OYO Trips)

**Author:** Arnav Jain | B.Tech (IT), NSUT Delhi  
**Role:** APM Candidate @ PRISM (OYO)  
**Date:** July 2026  

> *Exploring the group travel opportunity in OYO's booking experience — and designing a feature to unlock it.*

*(Note: Full slide deck and Figma wireframes to be uploaded here shortly)*

---

## 📌 1. The Problem: OYO is built for exactly one person.
Despite being India's dominant budget hospitality platform, OYO's booking infrastructure entirely ignores its highest-frequency demographic: **Young Group Travellers**. 

The moment two or more friends try to book a trip, the product abandons them.
- No group room selection from the start.
- No split payment natively in-app.
- No shared confirmation (everyone gets separate booking IDs).

**Goal:** Build a shared group booking experience that drives multi-room **GBV (Gross Booking Value) per session** and increases repeat usage among college students and young professionals.

---

## 🔍 2. User Research & Validation (Pain in Numbers)
*Based on secondary research via Play Store reviews, Reddit (r/india, r/travel), and user interviews.*

- **73%** of budget travelers plan group trips but cannot book together on a single platform.
- **68%** say they've had to make multiple separate bookings for the same trip.
- **4.2 rooms** is the average size of a group trip booking.

**User Evidence:**
> *"Tried booking 3 rooms for Manali with friends. Had to make separate bookings. One didn't even get the same hotel. Completely chaotic."* — Reddit User

> *"Why is there no 'book for a group' option? Had to screenshot my booking and send it to everyone to UPI me. This is 2025."* — Play Store Review

---

## 👤 3. User Personas
**1. Arjun Mehta, 26 | Software Engineer, Bengaluru (The Organizer)**
- **Behaviour:** Searches and selects hotels alone, screenshots booking page, feels burdened by lead-up.
- **Pain Points:** Pays full amount (e.g., ₹15,000) upfront, no split payment on OYO, communication overhead on WhatsApp.
- **Needs:** Shared group planning space, in-app sharing of booking details.

**2. Riya Sharma, 24 | Marketing Executive, Mumbai (The Invitee)**
- **Behaviour:** Prefers to be told what to do, ignores WhatsApp groups until trip is near.
- **Pain Points:** Constant payment reminders, no visibility on booking, feels guilty about causing Arjun stress.
- **Needs:** Her own direct payment link, personal booking confirmation pushed to her directly.

---

## 🛑 4. Booking Journey (As-Is Flow)
*How 5 friends try to book OYO today:*

1. **SEARCH:** Opens OYO, searches for Manali. *(Fails to find a "group size" filter).*
2. **SELECT:** Finds a hotel, but can only select 1 room in the flow.
3. **BOOK:** Clicks "Book Now." No option to add more rooms for friends.
4. **PAY:** Pays the full amount alone (e.g., ₹12,000). *(Major friction point).*
5. **COORDINATE:** Screenshots booking ID, sends to friends on WhatsApp to beg for UPI transfers.

---

## ⚔️ 5. Market Gap
*What are travelers switching to when OYO fails them?*

| Feature | OYO | Airbnb | MakeMyTrip |
|---|---|---|---|
| **Group Booking** | 🔴 Not Built | 🟢 Supported | 🟢 Supported |
| **Split Pay** | 🔴 Not Built | 🟢 Supported | 🔴 Not Built |
| **Group Confirmation**| 🔴 Not Built | 🟢 Supported | 🔴 Not Built |

**OUR GOAL: BUILD "OYO TRIPS"**
- **Shared Space:** Let users invite friends to plan and decide together.
- **Split Payments:** Allow everyone to pay their own exact share via UPI directly.
- **Group Visibility:** Give every invited member their own booking confirmation. 

---

## 🚀 6. The Feature: OYO Trips
**A native group booking experience built into OYO. Three screens. One seamless flow.**

**How it works:**
1. **SCREEN 1: Group Search:** A **Group Mode Toggle** switches the entire app to a multi-room booking flow.
2. **SCREEN 2: Hotel & Room Pick:** A **Room Stepper** allows selecting how many rooms the group needs.
3. **SCREEN 3: Group Checkout:** 
   - **Guest Assignment:** Each member gets their own UPI payment link.
   - **Per-Person Pricing:** Each room shows cost split per member.

---

## 📈 7. Success Metrics

**North Star Metric:** 
**Group Bookings as % of Total Bookings** (Target: 15% within 12 months)

**Primary Metrics:**
- **Adoption Rate:** 20% of all 3+ room bookings use OYO Trips feature.
- **Avg Order Value:** ₹8,000+ per group booking (vs ₹1,200 solo avg).
- **Split Pay Completion:** 85%+ of group payments collected in-app within 24hrs.
- **90-Day Retention:** 40%+ of group bookers return for next trip via OYO.

**Guardrail Metrics:**
- Solo booking conversion rate must not drop (baseline ±2%).
- Payment-related support tickets must decrease by 30%.
- App crash rate on group flow must stay below 0.5%.
