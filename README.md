# Smart Public Bus E-Ticketing & Passenger Counting System

**Course:** CSE 3200 — System Development Project  
**Institution:** Rajshahi University of Engineering & Technology (RUET)  
**Department:** Computer Science & Engineering (CSE)

---

## 👥 Project Team

| Name | Roll | Role |
| :--- | :--- | :--- |
| **Md Asif Sarker** | `2203131` | Lead Builder & System Architect |
| **Wahid Galib** | `2203121` | Quality Auditor, Reviewer & Co-Developer |

---

## 📌 Project Overview

In urban public transportation, manual paper tickets and cash-based fare collection create persistent operational issues:
- **Fare disputes & delays:** Manual change counting and lack of transparent fare rules cause friction between conductors and commuters.
- **Revenue leakage:** Bus operators lack verifiable digital logs for daily trip income.
- **Overcrowding & blind scheduling:** Authorities have no real-time passenger occupancy data to adjust bus dispatch schedules.

This project delivers a **dedicated software solution (mobile-first)** to digitize the entire ticketing and passenger monitoring lifecycle without requiring expensive specialized hardware.

---

## 🚀 Key Features

1. **Conductor Mobile App (React Native / Expo):**
   - Rapid tap-to-issue digital ticketing for distance-based fares.
   - Offline ticket caching with automatic synchronization when network reconnects.
   - On-device daily summary and trip fare totals.

2. **Passenger Interface:**
   - Digital ticket receipt with QR verification.
   - Live route view and estimated bus crowd levels.

3. **Passenger Counting Engine:**
   - Simulated boarding/alighting events via dedicated API and interactive control panel.
   - Real-time seat occupancy and crowd status updates.

4. **Operator / Authority Dashboard:**
   - Aggregated trip revenue logs and route analytics.
   - Audit trail preventing ticket reuse or underreporting.

---

## 🛠️ Technology Stack

- **Mobile Client:** React Native (Expo framework)
- **Backend Server:** Node.js + Express.js (REST API architecture)
- **Database:** MongoDB (optimised trip collections & fare schemas)
- **State Management & Networking:** React Context / Zustand + Axios
- **Offline Storage:** AsyncStorage / SQLite (mobile local cache)
- **Simulation Suite:** Node.js mock sensor generator & test scripts

---

## 📂 Repository Layout

```text
├── client/                     # React Native (Expo) mobile application
├── server/                     # Node.js + Express REST API backend
├── simulation/                 # Automated passenger count & sensor simulation
├── planning/                   # Project roadmap, sprint boards & agent protocols
│   ├── README.md               # Master plan and workflow guide
│   ├── SPRINTS.md              # Detailed sprint breakdown (Sprints 1 - 6)
│   ├── TASK_TRACKER.md         # Live task status board
│   └── AGENT_COLLABORATION_PROTOCOL.md # Guidelines for AI agents (Asif & Galib)
├── docs/                       # Academic reports, SRS, and survey forms
├── .gitignore
└── README.md
```

> **Note:** The `planning/` directory coordinates sprint execution and collaborative workflows between both teammates and their AI agents. It will be archived or removed prior to final academic submission.

---

## 🚦 Getting Started

### Prerequisites
- Node.js (v18 or higher)
- npm or yarn
- Expo Go app on Android/iOS (for mobile testing) or Android Studio emulator
- MongoDB instance (local or MongoDB Atlas)

### Setup Instructions
1. **Clone the repository:**
   ```bash
   git clone https://github.com/asifsarker-dev/CSE-3200-SMART-Bus-Tracking-Project.git
   cd CSE-3200-SMART-Bus-Tracking-Project
   ```
2. **Review the sprint plan:**
   Check [`planning/TASK_TRACKER.md`](planning/TASK_TRACKER.md) to inspect current sprint objectives and active deliverables.
