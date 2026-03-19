# Gig Delivery Worker Insurance

---

## Overview

This project introduces an AI-powered parametric insurance platform tailored for gig delivery workers. It delivers affordable, weekly micro-insurance with fully automated payouts triggered by real-world disruption events such as adverse weather, platform outages, and regulatory restrictions.

By replacing traditional claim-based insurance with real-time event-driven automation, the system ensures zero paperwork, instant compensation, and complete transparency, making financial protection accessible to the gig economy.

---

## Problem Statement

Gig delivery workers operate in a highly volatile environment where income is directly impacted by external disruptions such as weather conditions, platform failures, and government-imposed restrictions.

Despite this uncertainty, they lack access to affordable insurance, real-time income protection, and efficient claim mechanisms. Existing insurance solutions are slow, complex, and not designed for dynamic, short-term earning models.

---

## Proposed Solution

We propose a parametric insurance system that leverages real-time data and AI to provide seamless income protection.

- Dynamically calculates premiums based on zone risk and worker activity  
- Continuously monitors external triggers such as weather, outages, and curfews  
- Automatically validates and processes claims without user intervention  
- Instantly disburses payouts to the worker’s wallet or bank account  

This approach ensures fast, fair, and frictionless insurance coverage aligned with the needs of gig workers.
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

## AI (LLM) Integration

The system integrates a Large Language Model (Gemini) to enhance user experience.

### Use Cases

- Chatbot assistance for user queries  
- Premium explanation  
- Claim reasoning  
- Weekly activity reports  

---

### Chatbot Workflow

User Question  
        ↓  
React Interface  
        ↓  
Spring Boot Backend  
        ↓  
Gemini API  
        ↓  
AI Response  
        ↓  
Displayed to User  

---

### Weekly Report Workflow

User Activity Data  
        ↓  
Backend Processing  
        ↓  
Data sent to LLM  
        ↓  
AI generates summary  
        ↓  
Insights displayed  

---

## User Journey

Rahul, a delivery rider, opens the insurance app before starting his workday. He checks the weekly insurance plan and sees a small premium calculated based on his delivery zone and activity history.

Rahul purchases the weekly plan in a few seconds. During the week, the system continuously monitors weather alerts, platform outages, and government curfews using external APIs.

One evening, a severe flood alert is issued in Rahul’s delivery zone. Because deliveries stop in that area, the system automatically detects the trigger event and verifies that Rahul was actively working.

Without filing any claim, Rahul receives an automatic payout in his wallet, helping him manage the income loss for that day.

---

## Key Features

- Low-cost weekly insurance  
- Real-time trigger detection  
- Fully automated claims  
- AI-powered explanations  
- Instant payouts  

---

## Tech Stack

Frontend: React  
Backend: Spring Boot  
Database: MySQL  
AI Model: Google Gemini  
Deployment: AWS  

---

## Backend Structure

```
com.insurance.ai
│
├── controller
│   ├── UserController.java
│   ├── PremiumController.java
│   ├── ClaimController.java
│   └── AIController.java
│
├── service
│   ├── PremiumService.java
│   ├── ClaimService.java
│   ├── RiskService.java
│   ├── FraudService.java
│   └── LLMService.java
│
├── model
│   ├── User.java
│   ├── Policy.java
│   ├── Claim.java
│   └── RiskData.java
│
├── repository
│   ├── UserRepository.java
│   ├── PolicyRepository.java
│   └── ClaimRepository.java
│
└── dto
    ├── ChatRequestDTO.java
    ├── ClaimDTO.java
    └── PremiumDTO.java
```

---

## Frontend Structure

```
src/
│
├── components/
│   ├── Chatbot.jsx
│   ├── Dashboard.jsx
│   ├── Premium.jsx
│   └── Claims.jsx
│
├── pages/
│   ├── Home.jsx
│   ├── Login.jsx
│   └── Register.jsx
│
├── services/
│   └── api.js
```

---

## Future Scope

- Integration with real delivery platforms (Swiggy, Zomato)  
- Advanced ML-based risk prediction  
- Mobile application deployment  
