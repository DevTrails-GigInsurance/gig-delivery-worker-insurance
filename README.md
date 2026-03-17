🛡️ Gig Delivery Worker Insurance
AI-Powered Parametric Insurance for Gig Workers
📌 Overview

This project presents an AI-powered parametric insurance platform designed for gig delivery workers. The system provides affordable weekly insurance coverage and ensures automatic payouts during disruption events such as adverse weather conditions, platform outages, and government-imposed restrictions.

Unlike traditional insurance systems, this solution eliminates manual claim filing by leveraging real-time event detection and intelligent automation, ensuring a seamless and transparent user experience.

👤 Persona-Based Requirement
Persona: Rahul – Gig Delivery Rider

Rahul is a 28-year-old delivery rider in Mumbai working with platforms like Swiggy and Zomato. He works approximately 8–10 hours daily and earns based on completed deliveries.

His income is highly dependent on:

Weather conditions (rain, floods)

Platform availability

City regulations

As a gig worker, Rahul does not receive traditional employment benefits such as insurance or income protection. When disruptions occur, his earnings stop immediately.

🎯 Problem Statement

Gig delivery workers face:

Lack of affordable insurance solutions

No income protection during disruptions

Complex and slow claim processes

Absence of real-time risk-based coverage

💡 Proposed Solution

A parametric insurance system that:

Calculates premiums based on dynamic risk factors

Uses real-time triggers (weather, outages, curfews)

Enables automatic claim processing without paperwork

Provides instant payouts to the worker

This ensures financial stability for gig workers during uncertain conditions.

🧾 Key Features

💰 Low-cost weekly insurance model

⚡ Automatic claim processing (no manual intervention)

📡 Real-time trigger detection using external APIs

🤖 AI-powered explanations and insights using LLM

💳 Instant payout to wallet or bank account

🔄 System Workflow
Step-by-Step Process

User registers in the application

System calculates weekly premium using risk factors

User purchases a weekly insurance plan

System continuously monitors parametric triggers

A disruption event is detected

System verifies user activity

Claim is automatically generated

Payout is credited instantly

🔁 Workflow Diagram
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
🤖 AI (LLM) Integration

The system integrates a Large Language Model (LLM) to enhance user experience and provide intelligent insights.

Use Cases:

💬 Chatbot Assistance – Answers user queries

📊 Premium Explanation – Explains pricing decisions

🔍 Claim Analysis – Provides reasoning for claim outcomes

📝 Weekly Reports – Generates personalized activity summaries

🔄 Chatbot Workflow
User Question
     ↓
React Chat Interface
     ↓
Spring Boot Backend (AI Controller)
     ↓
Gemini API (LLM)
     ↓
AI Response Generated
     ↓
Displayed to User
📝 Weekly Report Workflow
User Activity Data
        ↓
Backend Processing
        ↓
Data Sent to LLM (Gemini)
        ↓
AI Generates Summary
        ↓
Weekly Insights Displayed
🧭 User Journey

Rahul opens the application before starting his workday and checks the weekly insurance plan. The premium is calculated based on his delivery zone and activity history.

He purchases the plan within seconds. During the week, the system continuously monitors real-time events such as weather alerts, platform outages, and government restrictions.

One evening, a severe flood alert is issued in Rahul’s delivery zone. Deliveries are halted, and the system detects this disruption. After verifying Rahul’s activity, an automatic payout is initiated.

Without filing any claim, Rahul receives compensation directly in his wallet, helping him manage income loss efficiently.

⚙️ Tech Stack

Frontend: React

Backend: Spring Boot

Database: MySQL

AI Model: Google Gemini (LLM)

Deployment: AWS

🏗️ Backend Structure
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
🎨 Frontend Structure
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
