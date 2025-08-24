# MindMend – Chrome Extension for Digital Wellness

MindMend is a **Chrome Extension** built with **Plasmo + React + TypeScript + TailwindCSS** that detects when users are experiencing **screen burnout** and nudges them with **personalized digital breaks** (stretching, breathing, short walks, or fun micro-activities).  

Over time, it **learns from user feedback** and adapts to create a healthier, more productive browsing experience.

---

## Project Overview

### Problem  
People spend excessive time online → fatigue, stress, and reduced productivity.  

### Solution  
MindMend acts as a **personal wellness buddy** inside your browser, nudging you to take breaks **before burnout**.

---

## Features

### MVP (Phase 1) [Working on it right now]
- Detect burnout signals (long screen time, tab switching, endless scrolling).
- Popup UI with curated wellness break suggestions.

### Phase 2
- Reinforcement learning loop → learns from user feedback.
- Personalized break recommendations.

### Phase 3
- Sidepanel + NewTab dashboard with analytics (screen time, break history).
- Gamification: points, streaks, rewards.

### Phase 4 (Future)
- Google Fit / Apple Health API integrations for holistic wellness.
- Cross-device syncing for a full wellness ecosystem.

---

## Tech Stack

**Frontend**
- Plasmo – Chrome extension framework  
- React + TypeScript  
- TailwindCSS + shadcn/ui  
- Framer Motion – animations  

**AI/ML**
- Phase 1 → Rule-based detection (tab time, scroll speed, tab-switch frequency)  
- Phase 2 → Reinforcement Learning (Python: PyTorch / Scikit-learn / TensorFlow)  
- In-browser inference → TensorFlow.js / ONNX.js  

**Integration**
- Chrome Extension APIs → background scripts, content scripts, notifications  
- Local storage → preferences, history, streaks  

---

## Architecture

---

## Workflow
            ┌───────────────┐
            │     User      │
            │ Interacts &   │
            │ gives feedback│
            └───────┬───────┘
                    │
                    ▼
    ┌─────────────────────────────────┐
    │ User Interface (Frontend - UI) │
    │ Popup (React) → shows alerts,  │
    │ suggestions                    │
    └───────────┬────────────────────┘
                │ Collects events
                ▼
    ┌─────────────────────────────────┐
    │     Background Scripts          │
    │ - Track screen usage patterns   │
    │   (time spent, activity signals)│
    │ - Send raw usage data to ML     │
    └───────────┬────────────────────┘
                │ Sends usage data
                ▼
    ┌─────────────────────────────────┐
    │ Backend Services / ML Module    │
    │ - Suggestion engine adapts ideas│
    │ - Feedback loop from user       │
    │ - Local ML or API-based model   │
    └───────────┬────────────────────┘
                │ Sends suggestions
                ▼
    ┌─────────────────────────────────┐
    │ Storage Layer (Database)        │
    │ - Saves preferences, history,   │
    │   streaks, and feedback         │
    │ - Provides personalization      │
    └─────────────────────────────────┘


---

## Roadmap

- Phase 1 → Burnout detection + static break suggestions  
- Phase 2 → Personalized ML with reinforcement learning  
- Phase 3 → Gamification + analytics dashboard  
- Phase 4 → API integrations (Google Fit, Apple Health)  

---


