# 🚀 EventFlow AI: The Smart Event Concierge

[![Rank](https://img.shields.io/badge/PromptWars_2026-cyan?style=for-the-badge)](https://hack2skill.com)
[![Build](https://img.shields.io/badge/Built_With-Google_Antigravity-violet?style=for-the-badge)](https://google.com)
[![Deployment](https://img.shields.io/badge/Deployed_To-Google_Cloud_Run-4285F4?style=for-the-badge)](https://cloud.google.com)

## 📌 Project Overview
**EventFlow AI** is an intelligent "Physical Event Concierge" designed to solve the chaos of large-scale sporting and tech events. By leveraging **Google Gemini (Vertex AI)**, it provides attendees with real-time crowd navigation, instant FAQ support, and AI-driven networking matches to transform the offline event experience.

### 🎯 The Problem
Large events suffer from:
- **Crowd Congestion:** Attendees don't know which zones are busy.
- **Information Gap:** Difficulty finding schedules, food stalls, or restrooms.
- **Missed Networking:** High-value connections are lost in the crowd.

### ✨ The Solution
- **AI Event Concierge:** A Gemini-powered chat interface that knows the event schedule and venue layout inside out.
- **Smart Networking:** An AI matching engine that connects attendees based on shared tech stacks or interests.
- **Real-time Coordination:** Seamless updates on session changes and crowd movement.

---

## 🛠️ Tech Stack & Google Services
This project is built to be "Cloud-Native" using the Google ecosystem:

| Category | Technology | Purpose |
| :--- | :--- | :--- |
| **Development** | **Google Antigravity** | Core logic generation and agentic code architecture. |
| **Frontend** | **React.js** | Glassmorphic, dark-themed UI for a premium mobile experience. |
| **Backend** | **Node.js (Express)** | Scalable API gateway running on Port 8080. |
| **AI Engine** | **Vertex AI (Gemini)** | Large Language Model for real-time concierge intelligence. |
| **Security** | **Cloud Secret Manager** | Securely handling API keys and Firebase credentials. |
| **Database** | **Firebase / Firestore** | Real-time data sync for networking and event updates. |
| **Hosting** | **Google Cloud Run** | Containerized deployment using Docker for high availability. |

---

## 🏗️ Architecture
The system follows a modern microservices approach:
1. **Frontend:** React application served as a static build or through the Node server.
2. **API:** Node.js server containerized with **Docker**.
3. **Security:** Runtime injection of secrets from **Google Cloud Secret Manager**.
4. **Logic:** **Antigravity-assisted** code patterns for optimized performance and testing.

---

## 🚀 Getting Started

### Prerequisites
- Node.js & Docker installed.
- A Google Cloud Project with Billing and Vertex AI API enabled.
- Google Cloud SDK (`gcloud`) configured.

### Local Installation
1. Clone the repo:
   ```bash
   git clone [https://github.com/SAYANui/Event-aura-AI.git](https://github.com/SAYANui/Event-aura-AI.git)
   
### 🧠 Prompt Engineering Strategy
To ensure the Concierge provides accurate, non-hallucinated event data, we implemented:
- **System Instructions:** Grounding Gemini in the specific event PDF/Schedule.
- **Few-Shot Prompting:** Training the model to handle "Where is the nearest restroom?" vs "When is the next MERN workshop?" differently.
- **Safety Filters:** Utilizing Vertex AI safety settings to block inappropriate content during the physical event.

### 🔐 Security & Infrastructure (GCP Native)
- **Identity:** Managed Service Accounts are used for Cloud Run to access Secret Manager.
- **Secret Injection:** API keys are fetched at runtime; no `.env` files exist in the production image.
- **CI/CD:** Automated builds via Artifact Registry to ensure container integrity.

   
