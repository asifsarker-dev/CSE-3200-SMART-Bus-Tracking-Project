# Live Task Tracker & Sprint Backlog

**Course:** CSE 3200 — System Development Project  
**Status Legend:**
- 🟡 `[TODO]` — Planned, awaiting start of sprint.
- 🔵 `[IN PROGRESS]` — Active development or drafting.
- 🟣 `[READY FOR AUDIT]` — Implemented by primary builder; waiting for peer review/audit.
- 🟢 `[DONE]` — Audited, verified, and merged into the main branch.

---

## 📋 Master Task Matrix

### Sprint 1: Problem Definition & Field Elicitation (Weeks 1–2)

| Task ID | Task Description | Req ID | Primary Owner | Reviewer / Auditor | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
| `TSK-101` | Draft Stage 0 Problem Statement (Owners, Users, Benefits) | `DOC-01` | Asif | Galib | 🟢 `[DONE]` |
| `TSK-102` | Conduct regional literature review (*bdtickets*, *Shohoz*, *Akota*) | `DOC-02` | Asif | Galib | 🟢 `[DONE]` |
| `TSK-103` | Prepare comparison matrix & justification for local bus solution | `DOC-02` | Galib | Asif | 🟢 `[DONE]` |
| `TSK-104` | Format & compile Stage 0 & 1 LaTeX Proposal (`Stage0_1_Report.tex`) | `DOC-01` | Asif | Galib | 🟢 `[DONE]` |
| `TSK-105` | Design field survey forms for conductors (5 entries) & commuters (10) | `DOC-03` | Galib | Asif | 🟢 `[DONE]` |
| `TSK-106` | Export printable `.pdf` and `.docx` survey questionnaires | `DOC-03` | Galib | Asif | 🟢 `[DONE]` |
| `TSK-107` | Conduct field visits, take ticket photo artifacts, log field diary | `DOC-04` | Asif & Galib | Both | 🔵 `[IN PROGRESS]` *(Photos/feedback forms to be uploaded)* |

---

### Sprint 2: Requirements Analysis & IEEE SRS (Week 3)

| Task ID | Task Description | Req ID | Primary Owner | Reviewer / Auditor | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
| `TSK-201` | Synthesize field survey responses into key user pain points | `SRS-01` | Galib | Asif | 🟢 `[DONE]` *(In `docs/SRS.md` §2.1)* |
| `TSK-202` | Draft Functional Requirements list (`FR-01` to `FR-12`) | `FR-ALL` | Asif | Galib | 🟢 `[DONE]` *(In `docs/SRS.md` §3.1)* |
| `TSK-203` | Draft Non-Functional Requirements (`NFR-01` to `NFR-06`) | `NFR-ALL` | Galib | Asif | 🟢 `[DONE]` *(In `docs/SRS.md` §3.2)* |
| `TSK-204` | Apply MoSCoW prioritization (Must, Should, Could, Won't) | `SRS-02` | Asif | Galib | 🟢 `[DONE]` *(In `docs/SRS.md` §4)* |
| `TSK-205` | Draw Use Case Diagram & User Stories with acceptance criteria | `SRS-03` | Galib | Asif | 🟢 `[DONE]` *(In `docs/SRS.md` §5 & §6)* |
| `TSK-206` | Compile IEEE-style SRS document draft for instructor review | `SRS-DOC` | Asif | Galib | 🟢 `[DONE]` *(In `docs/SRS.md` & `docs/SRS.tex`)* |

---

### Sprint 3: System Design & Technical Blueprint (Weeks 3–4)

| Task ID | Task Description | Req ID | Primary Owner | Reviewer / Auditor | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
| `TSK-301` | Define Client-Server Architecture (React Native ↔ Express ↔ MongoDB) | `DES-01` | Asif | Galib | 🟡 `[TODO]` |
| `TSK-302` | Design MongoDB Collections schema (`Users`, `Buses`, `Trips`, `Tickets`)| `DES-02` | Asif | Galib | 🟡 `[TODO]` |
| `TSK-303` | Audit DB schema for concurrency, indexing, and fare rule changes | `DES-02` | Galib | Asif | 🟡 `[TODO]` |
| `TSK-304` | Draw Sequence Diagram for conductor tap-to-issue transaction | `DES-03` | Galib | Asif | 🟡 `[TODO]` |
| `TSK-305` | Write Technology Selection Justification Note (React Native/Node) | `DES-04` | Asif | Galib | 🟡 `[TODO]` |

---

### Sprint 4: Core Implementation & "Thin Slice" (Weeks 4–5)

| Task ID | Task Description | Req ID | Primary Owner | Reviewer / Auditor | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
| `TSK-401` | Initialize Expo React Native project with modular folder structure | `IMP-01` | Asif | Galib | 🟡 `[TODO]` |
| `TSK-402` | Initialize Express server with route handlers & MongoDB connection | `IMP-02` | Asif | Galib | 🟡 `[TODO]` |
| `TSK-403` | Implement Conductor Authentication & Route Selection API | `FR-01` | Asif | Galib | 🟡 `[TODO]` |
| `TSK-404` | Build Conductor Mobile UI for Stop-to-Stop Fare selection | `FR-02` | Asif | Galib | 🟡 `[TODO]` |
| `TSK-405` | Implement Ticket Issuance API (`POST /api/tickets/issue`) | `FR-03` | Asif | Galib | 🟡 `[TODO]` |
| `TSK-406` | Audit API input validation, sanitization, and error responses | `SEC-01` | Galib | Asif | 🟡 `[TODO]` |
| `TSK-407` | Verify Thin-Slice end-to-end: Tap → DB Log → Digital Receipt | `VAL-01` | Galib | Asif | 🟡 `[TODO]` |

---

### Sprint 5: Passenger Counting Simulation & Offline Sync (Weeks 6–7)

| Task ID | Task Description | Req ID | Primary Owner | Reviewer / Auditor | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
| `TSK-501` | Build Passenger Counting simulation engine (Mock sensor events) | `FR-07` | Galib | Asif | 🟡 `[TODO]` |
| `TSK-502` | Implement Live Bus Occupancy calculation & API endpoint | `FR-08` | Galib | Asif | 🟡 `[TODO]` |
| `TSK-503` | Build Commuter View in Mobile App: Route status & crowd level | `FR-09` | Asif | Galib | 🟡 `[TODO]` |
| `TSK-504` | Implement Offline Ticket Caching in React Native (`AsyncStorage`) | `NFR-02`| Asif | Galib | 🟡 `[TODO]` |
| `TSK-505` | Implement Offline Sync reconciliation engine upon reconnection | `NFR-02`| Galib | Asif | 🟡 `[TODO]` |
| `TSK-506` | Stress-test offline queue conflict resolution and duplicate checks | `TST-03` | Galib | Asif | 🟡 `[TODO]` |

---

### Sprint 6: Rigorous Testing, RTM & Final Delivery (Weeks 8–9)

| Task ID | Task Description | Req ID | Primary Owner | Reviewer / Auditor | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
| `TSK-601` | Design test suite using Equivalence Partitioning & Boundary Values | `TST-01` | Galib | Asif | 🟡 `[TODO]` |
| `TSK-602` | Build Requirement Traceability Matrix (`RTM.md`) linking FRs to tests | `RTM-01` | Galib | Asif | 🟡 `[TODO]` |
| `TSK-603` | Perform User Acceptance Testing (UAT) with real conductor feedback | `TST-04` | Asif & Galib | Both | 🟡 `[TODO]` |
| `TSK-604` | Optimize mobile performance, UI responsive states, and polish | `POL-01` | Asif | Galib | 🟡 `[TODO]` |
| `TSK-605` | Conduct final code audit, remove debug logs, finalize documentation | `AUD-01` | Galib | Asif | 🟡 `[TODO]` |
| `TSK-606` | Prepare final presentation slides and demo walkthrough recording | `DEL-01` | Asif & Galib | Both | 🟡 `[TODO]` |

---

## 🔄 Status Update Instructions

When working on a task:
1. Switch status to 🔵 `[IN PROGRESS]` and reference the `Task ID` in your Git branch (e.g., `git checkout -b feature/TSK-405-ticket-api`).
2. When the implementation is ready, open a Pull Request, tag your partner, and update status to 🟣 `[READY FOR AUDIT]`.
3. The auditor checks the code, runs boundary tests, verifies the linked Requirement ID, and approves the merge.
4. Update the status to 🟢 `[DONE]` with the merge commit hash.
