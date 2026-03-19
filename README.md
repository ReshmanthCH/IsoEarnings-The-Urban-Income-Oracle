# IsoEarnings-The-Urban-Income-Oracle
AI-powered parametric insurance platform for gig workers that provides real-time, income-based payouts using dual-trigger validation and intelligent risk modeling.


## 1. Problem Statement

India’s platform-based delivery partners (food, grocery, e-commerce) lose 20–30% of their weekly earnings due to uncontrollable external disruptions such as extreme weather, pollution, and mobility restrictions. Traditional insurance products do not cover *loss of working time* or *inability to earn*, leaving gig workers without a financial safety net for non-personal disruptions.

**Core Gap:** Events are insured; *income loss is not*.

---

## 2. Persona & Scenario

**Primary User:** Urban food delivery partner (e.g., Swiggy/Zomato) in a city like Chennai.

**Profile:**

* Works in peak time slots (e.g., 7–10 PM)
* Earnings depend on deliveries per hour
* Highly sensitive to weather and traffic

**Scenario:**
A delivery partner typically earns ₹120/hour during peak time. Due to heavy rain, deliveries drop drastically. Over 3 hours:

* Expected earnings: ₹360
* Actual earnings: ₹120
* Income loss: ₹240

Our system detects this and automatically compensates a portion of the loss.

---

## 3. Solution Overview

We propose an **AI-powered parametric insurance platform** that provides **automatic, income-based compensation** when workers lose earnings due to real-world disruptions.

### Key Differentiators

* Dual-trigger system (event + income validation)
* Income-based payouts (not fixed payouts)
* Zero-touch automated claims
* Built-in fraud prevention

---

## 4. System Workflow

User → Selects weekly plan → System monitors environment + activity → Disruption occurs → Opportunity Loss detected → Fraud checks → Income loss calculated → Payout triggered

---

## 5. Parametric Trigger System

### Core Logic

A payout is triggered only when:

1. A real-world disruption occurs
2. Opportunity Loss > 50% (drop in earning potential vs 7-day baseline)

### Triggers

* Rain/Flood
* Heatwave
* Pollution
* Traffic disruption
* Cluster-based inactivity

### Safety Incentive

During Red Alert conditions (extreme weather), the 50% rule is waived to prioritize worker safety.

### Surge Adjustment

If platform surge pricing is active, payouts are reduced to avoid double compensation.

---

## 6. Weekly Premium Model

The system follows a **weekly subscription model** aligned with gig worker earnings.

### Premium Structure

* Base: ₹20/week
* +₹10 (high-risk area)
* +₹5 (peak-hour heavy usage)

### Justification

* Affordable and aligned with weekly earning cycles
* Dynamic pricing based on risk ensures sustainability

---

## 7. Income-Based Payout Logic

Expected Earnings = Avg (orders/hour × avg order value)
(based on last 7 days, same time slot)

Income Loss = Expected – Actual

Payout = 70–80% of loss (with caps)

---

## 8. AI/ML Integration Plan

AI is used in three key areas:

### 1. Risk-Based Premium Calculation

* Inputs: location, weather history, disruption frequency
* Output: risk score → premium adjustment

### 2. Opportunity Loss Detection

* Predict expected earnings using historical patterns

### 3. Fraud Detection

* Detect anomalies using:

  * GPS patterns
  * motion data
  * cluster validation

---

## 9. Platform Choice (Web vs Mobile)

We choose a **mobile-first approach** because:

* Delivery workers primarily use smartphones
* Real-time tracking and GPS integration are easier
* Better user accessibility during work hours

---

## 10. Tech Stack

* Frontend: React / Flutter
* Backend: Node.js / Python
* AI/ML: Python (Scikit-learn)
* APIs: Weather, AQI, Traffic (mock/real)

---

## 11. Development Plan

### Phase 1

* Finalize idea, triggers, pricing, and workflow

### Phase 2

* Build core system:

  * User onboarding
  * Trigger detection
  * Income calculation

### Phase 3

* Add advanced features:

  * Fraud detection
  * Dashboard
  * Payment simulation

---

## 12. Data Strategy

* Delivery data: simulated (synthetic datasets)
* External data: APIs (weather, AQI, traffic)

---

## 13. Future Scope

* Supply-side disruption detection (merchant outages)
* Real platform integration
* Predictive alerts before disruptions

---

## 14. Key Insight

**We do not insure events — we insure actual income loss.**
