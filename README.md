<div align="center">

# 🧪 QA Automation Framework
### Cypress · End-to-End · API Testing · Page Object Model

[![Cypress](https://img.shields.io/badge/Cypress-17202C?style=for-the-badge&logo=cypress&logoColor=white)](https://cypress.io)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://nodejs.org)
[![Mochawesome](https://img.shields.io/badge/Mochawesome-Reports-blueviolet?style=for-the-badge)](https://github.com/adamgruber/mochawesome)

*A real-world automation framework covering UI, API, and integrated E2E testing*

</div>

---

## 📌 Overview

This project is a **production-grade, end-to-end automation testing framework** built with Cypress. It covers UI testing, REST API validation, and seamless backend-to-UI integration testing across two real-world applications:

| Application | Domain |
|---|---|
| 🏥 **CURA Healthcare** | Patient portal, appointment booking |
| 🎓 **Alison E-Learning** | Course navigation, user journeys |

The framework follows the **Page Object Model (POM)** design pattern to maximize scalability, reusability, and maintainability — aligned with industry standards.

---

## 🛠️ Tech Stack

| Layer | Tools |
|---|---|
| **Test Framework** | Cypress |
| **Language** | JavaScript |
| **Design Pattern** | Page Object Model (POM) |
| **Reporting** | Mochawesome (HTML + JSON) |
| **Runtime** | Node.js |
| **API Testing** | Cypress + Postman concepts |

---

## ✅ Features

### 🖥️ UI Automation
- Login functionality testing across multiple apps
- Appointment booking workflow (CURA Healthcare)
- Course navigation and user interaction (Alison)
- Form validation and UI element verification

### 🔌 API Testing
- Automated login API validation
- Authentication response and status code assertions
- Backend response verification before UI interaction
- Data consistency checks between API and UI layers

### 🔄 End-to-End (API → UI Flow)
- Triggered login via backend API
- Session/token used for UI state validation
- Verified seamless frontend-backend integration

---

## 🌐 Applications Tested

<details>
<summary><b>🏥 CURA Healthcare Application</b></summary>

- Automated patient login and appointment booking
- Validated complete user workflows
- Verified UI elements and form behaviour
- Ensured functional correctness of the booking system

</details>

<details>
<summary><b>🎓 Alison E-Learning Platform</b></summary>

- Automated login and course navigation
- Verified UI behaviour across user journeys
- Tested real-world learner flows end-to-end

</details>

---

## 📂 Project Structure
```
cypress/
├── e2e/            # Test spec files
├── pages/          # Page Object Model classes
├── fixtures/       # Test data (JSON)
├── reports/        # Mochawesome HTML & JSON reports
├── screenshots/    # Captured on test failure
└── videos/         # Full execution recordings
```

---

## 📊 Reporting & Debugging

| Feature | Details |
|---|---|
| 📄 **HTML Reports** | Mochawesome visual reports |
| 🗂️ **JSON Reports** | Machine-readable test output |
| 📸 **Screenshots** | Auto-captured on failure |
| 🎥 **Video Recording** | Full execution playback |

---

## ▶️ Getting Started

**1. Clone the repository**
```bash
git clone https://github.com/Srinath0041/cypress-e2e-automation-framework.git
cd cypress-e2e-automation-framework
```

**2. Install dependencies**
```bash
npm install
```

**3. Open Cypress Test Runner (Interactive)**
```bash
npx cypress open
```

**4. Run all tests headlessly**
```bash
npx cypress run
```

---

## 💡 Key Highlights

- ✅ Scalable framework using **Cypress + POM** design
- ✅ Integrated **API testing** with UI automation
- ✅ Real-world **E2E test coverage** across two apps
- ✅ Rich debugging via **reports, screenshots & videos**
- ✅ Clean, maintainable code structure for team collaboration

---

## 🎯 Outcome

This framework demonstrates practical, hands-on expertise in **automation engineering** — from API layer validation to full UI test coverage. It reflects the ability to architect maintainable, scalable QA solutions suitable for professional software delivery teams.

---

<div align="center">

**Built by [Srinath Avula](https://linkedin.com/in/srinathavula)**

*QA Automation Enthusiast · Selenium · Cypress · API Testing · Java · JavaScript*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/srinathavula)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Srinath0041)

</div>
