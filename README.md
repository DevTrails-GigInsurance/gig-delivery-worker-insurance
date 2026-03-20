# Gig Delivery Worker Insurance

---

## Overview

This project introduces an AI-powered parametric insurance platform tailored for gig delivery workers. It provides affordable, weekly micro-insurance with fully automated payouts triggered by real-world disruption events such as adverse weather, platform outages, and regulatory restrictions.

By replacing traditional claim-based insurance with real-time event-driven automation, the system ensures zero paperwork, instant compensation, and complete transparency, making financial protection accessible to the gig economy.

---

## Problem Statement

Gig delivery workers operate in a highly volatile environment where income is directly impacted by external disruptions such as weather conditions, platform failures, and government-imposed restrictions.

Despite this uncertainty, they lack access to affordable insurance, real-time income protection, and efficient claim mechanisms. Existing insurance solutions are slow, complex, and not designed for dynamic, short-term earning models.

---

## Proposed Solution

We propose a parametric insurance system that leverages real-time data and AI to provide seamless income protection.

- Dynamically calculates premiums based on risk factors  
- Continuously monitors real-time disruption triggers  
- Automatically validates and processes claims  
- Instantly disburses payouts to the worker  

This approach ensures fast, fair, and frictionless insurance coverage aligned with gig workers.

---

## Premium Model

Premium = Base Price × Zone Risk × Worker Risk Score

- **Base Price**: Fixed minimum weekly cost  
- **Zone Risk**: Based on location (rainfall, flood-prone areas, disruption frequency)  
- **Worker Risk Score**: Based on activity level, working hours, and reliability  

This ensures personalized and fair pricing.

---

## Parametric Triggers

The system uses predefined external triggers to initiate claims automatically:

- **Weather Trigger**: Heavy rain / flood alerts via Weather APIs  
- **Platform Trigger**: Delivery platform downtime (e.g., Swiggy/Zomato outages)  
- **Regulatory Trigger**: Government-imposed curfews or restrictions  

Once triggered, claims are processed without user intervention.

---

## Platform Choice

The system is implemented as a **web-based application** to ensure quick accessibility, faster development, and cross-device compatibility.

It can be extended into a **mobile application** in future phases for better user experience.

---

## AI/ML Integration

AI is integrated into the system to improve automation and decision-making:

- Risk scoring for premium calculation  
- Fraud detection during claim validation  
- LLM-based chatbot for user support  
- AI-generated weekly activity insights  

---

## Persona-Based Requirement & Workflow

### Persona: Rahul – Gig Delivery Rider

Rahul is a 28-year-old delivery rider in Mumbai working for platforms like Swiggy and Zomato. He works around 8–10 hours daily and earns based on completed deliveries. His income depends on weather, platform availability, and city regulations.

As a gig worker, Rahul does not receive traditional benefits like insurance. When disruptions occur, his earnings stop immediately.

He needs a simple, low-cost insurance system with automatic payouts.

---

### Persona Requirements

- Low-cost insurance suitable for gig workers  
- Weekly premium payment model  
- Automatic claim processing without paperwork  
- Real-time disruption detection  
- Instant payout to wallet or bank  

---

### Workflow

1. User registers in the application  
2. System calculates weekly premium  
3. User purchases weekly insurance  
4. System monitors real-time triggers  
5. Disruption event detected  
6. System verifies worker activity  
7. Claim generated automatically  
8. Instant payout credited  

---

### Workflow Diagram

```
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
(Weather / Platform / Curfew APIs)
        ↓
Trigger Event Detected
        ↓
System Verifies Worker Activity
        ↓
Automatic Claim Generation
        ↓
Payout Sent to Wallet/Bank
```

---

## AI Chatbot Workflow

```
User Question
        ↓
Frontend (React)
        ↓
Backend (Spring Boot)
        ↓
LLM API
        ↓
AI Response
        ↓
Displayed to User
```

---

## Weekly Report Workflow

```
User Activity Data
        ↓
Backend Processing
        ↓
Sent to LLM
        ↓
AI Generates Summary
        ↓
Insights Displayed
```

---

## User Journey

Rahul opens the app before starting his workday and checks the weekly insurance plan. The premium is calculated based on his location and activity.

He purchases the plan instantly. During the week, the system continuously monitors weather alerts, platform outages, and government restrictions.

One day, a flood alert occurs in his delivery zone. Deliveries stop, and the system detects the disruption. After verifying his activity, a claim is automatically processed.

Rahul receives the payout instantly without filing any request.

---

## Key Features

- Affordable weekly insurance  
- Real-time trigger detection  
- Fully automated claims  
- AI-powered assistance  
- Instant payouts  

---

## Tech Stack

Frontend: React  
Backend: Spring Boot  
Database: MySQL  
AI Model: LLM (Gemini/OpenAI)  
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
