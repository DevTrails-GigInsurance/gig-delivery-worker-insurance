# Gig Delivery Worker Insurance

---

## Persona-Based Requirement & Workflow

### Persona: Rahul – Gig Delivery Rider

Rahul is a 28-year-old delivery rider in Mumbai working for platforms like Swiggy and Zomato. He works around 8–10 hours daily and earns based on completed deliveries. His income is highly dependent on weather, platform availability, and city regulations.

Because he is part of the gig economy, Rahul does not receive traditional employee benefits like insurance or income protection. When events like heavy rain, floods, platform outages, or curfews occur, deliveries stop and he immediately loses income.

Rahul needs a simple and affordable insurance system that matches his weekly earning cycle and provides automatic compensation when disruptions prevent him from working.

---

### Persona Requirements

- Low-cost insurance suitable for gig workers  
- Weekly premium payment model  
- Automatic claim processing without paperwork  
- Real-time detection of disruption events  
- Quick payout to wallet or bank account

---

### Workflow

1. Rahul registers in the application.
2. The system calculates the weekly premium using risk factors.
3. Rahul buys a weekly insurance plan.
4. The system monitors triggers like rain, platform outages, or curfews.
5. If a disruption occurs, the system verifies worker activity.
6. The system automatically initiates the payout.
7. Rahul receives compensation in his wallet or bank account.

---

### Workflow Diagram

User (Delivery Rider)
        ↓
Register in the App
        ↓
System Calculates Weekly Premium
(Base × ZoneRisk × WorkerRiskScore)
        ↓
User Purchases Weekly Insurance
        ↓
System Monitors Parametric Triggers
(Weather API / Platform Status / Curfew Alerts)
        ↓
Trigger Event Detected
        ↓
System Verifies Worker Activity
        ↓
Automatic Claim Generation
        ↓
Payout Sent to Rider Wallet/Bank

---

## User Journey

Rahul, a delivery rider, opens the insurance app before starting his workday. 
He checks the weekly insurance plan and sees a small premium calculated based 
on his delivery zone and activity history.

Rahul purchases the weekly plan in a few seconds. During the week, the system 
continuously monitors weather alerts, platform outages, and government curfews 
using external APIs.

One evening, a severe flood alert is issued in Rahul’s delivery zone. Because 
deliveries stop in that area, the system automatically detects the trigger 
event and verifies that Rahul was actively working.

Without filing any claim, Rahul receives an automatic payout in his wallet, 
helping him manage the income loss for that day.