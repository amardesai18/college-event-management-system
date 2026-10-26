# College Event Management System (CEMS)
### SVERI's College of Engineering, Pandharpur (An Autonomous Institute)
**Department of Computer Science and Engineering | Academic Year: 2026-27**

---

## 👥 Project Team & Credentials
- **Student Authors:**
  1. **Amar Dattatray Desai** (PRN: `2024ET11161`)
  2. **Gaurav Pramod Kamble** (PRN: `2024ET11192`)
  3. **Kunal Dinesh Pawar** (PRN: `2024ET11230`)
- **Project Guide:** **Mrs. S. V. Saraf**
- **Head of Department (CSE):** **Dr. V. D. Jadhav**
- **Principal:** **Dr. B. P. Ronge**

---

## 🌟 Overview
This repository contains the interactive web application and digital report presentation for the **College Event Management System (CEMS)**, built in accordance with the project specification report.

The system addresses the challenges of fragmented campus event announcements (notice boards, messaging groups, spreadsheets) by delivering a unified, role-based platform that coordinates the complete event lifecycle: from proposal and venue conflict verification to student registration, digital QR ticketing, organizer check-in, and administrative audit logging.

---

## 🚀 Key Modules & Implemented Features

### 1. Dual Mode System Navigation
- **Interactive Portal:** Live dashboard featuring the exact layout and metrics from **Figure 2** of the report.
- **Project Report & Documentation:** A complete, beautifully styled academic viewer containing the entire mini project report (Cover Page, Certificate, Acknowledgement, Abstract, Chapters 1–5, and Figure 1 SVG Flowchart) with one-click **Print / Save as PDF** support.

### 2. Role-Based Access Control (RBAC)
Effortlessly switch between roles in the top navigation to test role permissions:
- 🎓 **Student Mode (Amar Desai):**
  - Search and filter published events by category (*Technical, Academic, Cultural, Sports*) and venue.
  - 1-Click Event Registration with real-time capacity decrement.
  - Generates a **Digital Pass** featuring student details, PRN, and an authentic SVG QR Code.
  - Self-service cancellation (frees slot back to the pool).
  - Priority waitlist placement when an event is full.
- 📋 **Organizer Mode (Gaurav Kamble):**
  - **Organizer Overview Panel** showing personal event statistics (*Drafts, Awaiting Review, Approved, Registered Participants*).
  - **Create Event Proposal Form:** Includes live, client-side **Venue Conflict Detection** that alerts organizers if another event is scheduled for the same venue and date.
  - **Attendance Check-In Manager:** Searchable participant roster, 1-click check-in verification, operator logging, and automated timestamps.
- 🛡️ **Administrator Mode (Dr. V. D. Jadhav):**
  - **Review Queue:** Review pending proposals with conflict alerts.
  - Actions to **Approve** (publishes event instantly to the student catalogue) or **Return for Revision** (prompts for feedback/reason and moves proposal to draft).
  - Complete **System Audit Trail** logging all significant administrative actions.

### 3. Figure 2 Dashboard Fidelity
- **Metric Cards:**
  - `UPCOMING EVENTS: 12`
  - `MY REGISTRATIONS: 3`
  - `PENDING APPROVALS: 4`
  - `EVENTS THIS MONTH: 8`
- **Pre-Seeded Catalog Events:**
  - *Annual Technical Symposium* (18 Nov 2026 | Main Auditorium | `OPEN`)
  - *Inter-College Debate* (22 Nov 2026 | Seminar Hall | `OPEN`)
  - *Cultural Evening* (29 Nov 2026 | Open Ground | `FULL`)
  - *Python Workshop* (04 Dec 2026 | Lab 2 | `REGISTERED`)
  - *Sports Meet* (10 Dec 2026 | Sports Complex | `OPEN`)
- **Organizer Stats:**
  - `Draft events: 2`
  - `Awaiting review: 1`
  - `Approved events: 5`
  - `Participants registered: 186`

---

## 💻 Tech Stack
- **Frontend Presentation:** Semantic HTML5, Modular CSS3 (Design Tokens, Grid, Flexbox, Glassmorphism), Native ES6+ JavaScript.
- **Data Persistence:** Client-side `localStorage` caching with automatic fallback to pre-seeded defaults, enabling realistic mutations (new registrations, new proposals, approvals, attendance toggles) that persist across page reloads.
- **Architecture Flow:** High-precision SVG implementation of the **Event Lifecycle (Figure 1)**.
- **Zero External Dependencies Required:** Completely self-contained; runs offline in any standard web browser without requiring Node.js, Python, or external packages.

---

## 🏃‍♂️ How to Run

1. Simply double-click **`index.html`** or open it in any modern browser (Google Chrome, Microsoft Edge, Mozilla Firefox, Safari).
2. Use the top right role switcher to explore permissions as a **Student**, **Organizer**, or **Administrator**.
3. Click the **Project Report** tab in the navigation bar to inspect the complete academic report, view the architecture flowchart, or print the document.
4. If you want to reset all test data back to the original demo values, click the **Reset Demo** button in the System Audit Trail panel.
