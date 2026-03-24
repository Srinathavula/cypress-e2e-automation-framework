<div align="center">

<h1>  Cypress E2E Automation Framework</h1>

<p><strong>Enterprise-Grade UI · API · End-to-End Test Automation</strong></p>

[![Cypress](https://img.shields.io/badge/Cypress-17202C?style=for-the-badge&logo=cypress&logoColor=white)](https://cypress.io)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://nodejs.org)
[![Mochawesome](https://img.shields.io/badge/Reports-Mochawesome-blueviolet?style=for-the-badge)](https://github.com/adamgruber/mochawesome)
[![POM](https://img.shields.io/badge/Pattern-Page%20Object%20Model-blue?style=for-the-badge)]()
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)]()

<p>A scalable, maintainable, and production-ready test automation framework built with <strong>Cypress</strong> — covering real-world UI, API, and integrated End-to-End testing across multiple industry domains.</p>

⭐ If this project helped you, consider giving it a star — it motivates continued improvement!

</div>

---

## 📌 Overview

This framework simulates how QA automation is handled in real software companies. It is built to validate complete user journeys — from backend API responses to UI behaviour — across **Healthcare** and **E-Learning** platforms.

The project goes beyond simple UI clicks. It integrates **API-layer validation**, **backend-to-frontend data consistency checks**, and **end-to-end workflow automation**, all structured using the **Page Object Model (POM)** design pattern — the industry standard for scalable test architecture.

> 💡 **Goal:** Demonstrate production-level QA engineering skills — framework design, API + UI integration testing, and real-world test coverage — in a way that is immediately recognizable to hiring teams.

---

## 🛠️ Tech Stack

| Category | Technology |
|---|---|
| **Automation Framework** | Cypress 13.x |
| **Language** | JavaScript (ES6+) |
| **Design Pattern** | Page Object Model (POM) |
| **Test Reporting** | Mochawesome (HTML + JSON) |
| **API Testing** | Cypress `cy.request()` |
| **Package Manager** | Node.js / npm |
| **Version Control** | Git & GitHub |
| **CI Ready** | Headless execution supported |

---

## ✅ Features Implemented

### 🖥️ UI Test Automation
- End-to-end login flow validation with positive and negative scenarios
- Appointment booking workflow automation (CURA Healthcare)
- Course navigation and learner journey testing (Alison E-Learning)
- Form field validation — required fields, error messages, boundary inputs
- Dynamic element handling and UI state assertions

### 🔌 API Test Automation
- REST API login validation using `cy.request()`
- HTTP status code assertions (200, 401, 403, 404)
- Response body schema and field-level validation
- Authentication token extraction and session handling
- Pre-condition setup via API to reduce test dependency on UI

### 🔄 End-to-End Integration (API → UI)
- Backend login triggered via API; session carried into UI layer
- API response data used to assert corresponding UI state
- Cross-layer data consistency validation (what API returns = what UI displays)
- Reduced flakiness by eliminating redundant UI steps using API setup

---

## 🌐 Applications Under Test

<details>
<summary><b>🏥 CURA Healthcare Application</b></summary>

**URL:** https://katalon-demo-cura.herokuapp.com

| Area | What Was Tested |
|---|---|
| Authentication | Login with valid/invalid credentials |
| Appointment Booking | Facility selection, date, comment, submission |
| Booking Confirmation | Verified confirmation page data against input |
| UI Validation | Field-level error messages, mandatory field checks |
| API Integration | Backend login → session used in UI booking flow |

</details>

<details>
<summary><b>🎓 Alison E-Learning Platform</b></summary>

**URL:** https://alison.com

| Area | What Was Tested |
|---|---|
| Authentication | Login validation with multiple credential sets |
| Course Navigation | Homepage → Category → Course page flow |
| UI Behaviour | Element visibility, page load assertions |
| User Journey | End-to-end learner flow from login to course landing |

</details>

---

## 🧪 Test Scenarios Covered

### Authentication & Login
- ✅ Valid login with correct credentials
- ✅ Invalid login — wrong password (error message assertion)
- ✅ Invalid login — unregistered user
- ✅ Empty field submission validation
- ✅ API login validation and token assertion

### Appointment Booking (CURA)
- ✅ Complete booking flow — facility, date, type, comment
- ✅ Booking confirmation data validation
- ✅ Mandatory field error handling
- ✅ Date picker interaction and validation

### Navigation & UI Validation
- ✅ Post-login redirection assertion
- ✅ Page element visibility checks
- ✅ Dynamic content loading validation
- ✅ Navigation between pages and sections

### API → UI Integration
- ✅ API-authenticated session used to drive UI test
- ✅ API response fields matched against UI-rendered values
- ✅ Backend error states reflected correctly in frontend

---

## 📊 Reporting & Debugging

| Capability | Implementation |
|---|---|
| 📄 **HTML Reports** | Mochawesome — visual pass/fail dashboard per spec |
| 🗂️ **JSON Reports** | Machine-readable output for CI/CD pipeline integration |
| 📸 **Screenshots** | Auto-captured on test failure for instant root cause analysis |
| 🎥 **Video Recording** | Full execution video per spec file for debugging flaky tests |
| 🖥️ **Interactive Runner** | Cypress Test Runner for live step-by-step execution |

> Mochawesome reports enabled faster defect identification and reduced debugging time by providing visual, organized test execution summaries.

---

## 📂 Project Structure
```
cypress-e2e-automation-framework/
│
├── cypress/
│   ├── e2e/                    # Test specification files
│   │   ├── healthcare/         # CURA Healthcare test suites
│   │   └── elearning/          # Alison E-Learning test suites
│   │
│   ├── pages/                  # Page Object Model classes
│   │   ├── LoginPage.js
│   │   ├── AppointmentPage.js
│   │   └── CoursePage.js
│   │
│   ├── fixtures/               # External test data (JSON)
│   │   ├── users.json
│   │   └── appointments.json
│   │
│   ├── support/
│   │   ├── commands.js         # Custom Cypress commands
│   │   └── e2e.js              # Global hooks and config
│   │
│   ├── reports/                # Mochawesome HTML + JSON reports
│   ├── screenshots/            # Failure screenshots (auto-generated)
│   └── videos/                 # Execution recordings (auto-generated)
│
├── cypress.config.js           # Cypress configuration
├── package.json                # Dependencies and scripts
└── README.md
```

---

## ▶️ Getting Started

### Prerequisites
- Node.js v16+ installed
- npm v8+ installed
- Git installed

### Installation & Run

**1. Clone the repository**
```bash
git clone https://github.com/Srinath0041/cypress-e2e-automation-framework.git
cd cypress-e2e-automation-framework
```

**2. Install dependencies**
```bash
npm install
```

**3. Open interactive Cypress Test Runner**
```bash
npx cypress open
```

**4. Run all tests in headless mode**
```bash
npx cypress run
```

**5. Run a specific test suite**
```bash
npx cypress run --spec "cypress/e2e/healthcare/**"
```

**6. Generate Mochawesome report**
```bash
npx cypress run --reporter mochawesome
```

---

## 💡 Key Highlights

| # | Highlight |
|---|---|
| 🏗️ | Designed a **scalable POM-based framework** that reduces code duplication and speeds up new test creation |
| 🔌 | Integrated **API testing with UI automation** — enabling true end-to-end validation across application layers |
| 🐛 | Reduced debugging time through **automated screenshots and video capture** on failure |
| 📊 | Improved test visibility with **Mochawesome HTML reports** — enabling quick pass/fail analysis |
| 🌐 | Achieved **multi-domain test coverage** across Healthcare and E-Learning industries |
| ⚡ | Enabled **faster regression cycles** by replacing manual testing with automated E2E flows |
| 🔁 | Used **API-layer setup** to reduce UI dependencies and improve test reliability |

---

## 🎯 Why This Project

Most fresher portfolios contain only basic login scripts. This project is different.

It demonstrates:

- **Framework thinking** — not just writing tests, but architecting a maintainable, scalable system using POM
- **API + UI integration** — understanding that real QA covers the full stack, not just the browser
- **Industry-standard tooling** — Cypress, Mochawesome, Page Object Model, fixture-driven test data
- **Debugging discipline** — screenshots, videos, and structured reports like production QA teams use
- **Domain awareness** — test coverage across Healthcare and E-Learning reflects adaptability across industries

> This is the difference between someone who learned to click through a UI and someone who understands how to **build and own a QA automation system**.

---

## 📈 Outcome

| Metric | Impact |
|---|---|
| Manual test effort | Significantly reduced through full E2E automation |
| Defect detection speed | Improved via instant screenshot + video capture |
| Test maintainability | Enhanced through POM — one change propagates across all tests |
| Framework reusability | New test cases added with minimal code changes |
| Recruiter signal | Demonstrates real-world automation engineering skills |

---

## 👤 Author

<div align="center">

**Srinath Avula**
*QA Automation Engineer · Cypress · Selenium · API Testing · Java · JavaScript*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/srinathavula)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Srinath0041)
[![Portfolio](https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge&logo=google-chrome&logoColor=white)](https://srinathavula.github.io/My-web-Pages/)

---

*Open to QA Automation / SDET opportunities — feel free to connect!*

</div>
