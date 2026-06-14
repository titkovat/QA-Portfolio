# 🧪 QA Portfolio — Tetiana Titkova

**Junior QA Engineer · Manual Testing · Test Documentation · Bug Reporting · Jira · Zephyr · API Testing**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Tetiana%20Titkova-blue)](https://www.linkedin.com/in/tetiana-titkova)
[![GitHub](https://img.shields.io/badge/GitHub-titkovat-black)](https://github.com/titkovat)

---

## 📁 Portfolio Structure

| Folder | What's inside | Tools |
|---|---|---|
| 📂 [Jira-Zephyr](./Jira-Zephyr) | Test cases, bug reports, test execution report for Cars.UA | Jira, Zephyr Scale |
| 📂 [Test-Cases](./Test-Cases) | Manual test cases in table format | Excel / Google Sheets |
| 📂 [Checklists](./Checklists) | Testing checklists for UI and functionality | Markdown / Excel |
| 📂 [Bug-Reports](./Bug-Reports) | Detailed bug reports with steps, expected/actual results | Jira |
| 📂 [API Testing Postman](./API%20Testing%20Postman) | REST API testing with automated assertions | Postman, JSON |

---

## 🔌 Jira + Zephyr Scale

**Project:** [Cars.UA](https://cars.ua) — car marketplace
**Scope:** Car search functionality, UI navigation, external links, dealership registration

### Test Cases (Zephyr Scale)

> See full details in [Jira-Zephyr](./Jira-Zephyr) folder.

---

## 📝 Test Cases

Manual test cases written for **cars.ua** covering:
- Search functionality (equivalence classes + boundary values)
- Filter functionality
- UI elements

**Techniques used:** Equivalence Partitioning · Boundary Value Analysis

> See full details in [Test-Cases](./Test-Cases) folder.

---

## ✅ Checklists

UI and functional checklists for cars.ua:
- Homepage UI elements
- Login & phone number validation
- Cross-browser testing (Chrome, Firefox, Safari, Edge)
- Filter functionality

> See full details in [Checklists](./Checklists) folder.

---

## 🐛 Bug Reports

3 bug reports found and documented during manual testing of cars.ua:

| ID | Title | Priority | Severity |
|---|---|---|---|
| BUG-001 | Viber Chatbot link does not open | High | Medium |
| BUG-002 | Registration button returns HTTP 500 | High | Critical |
| BUG-003 | City names displayed in Russian on Ukrainian version | Medium | Low |

> See full details in [Bug-Reports](./Bug-Reports) folder.

---

## 🔌 API Testing with Postman

**Project:** REST API testing for two real APIs

### cars.ua API
- `GET /api/v2/model/records?make_id=9` — retrieve BMW models
- Discovered via Chrome DevTools → Network tab
- Verified: status 200 OK, JSON format, correct make_id in response

### GoRest API — Full CRUD Cycle

| Method | Endpoint | Expected Status | Assertions |
|---|---|---|---|
| POST | `/users` | 201 Created | 3/3 ✅ |
| PATCH | `/users/{id}` | 200 OK | 2/2 ✅ |
| DELETE | `/users/{id}` | 204 No Content | 1/1 ✅ |
| GET | `/users/{id}` | 404 Not Found | ✅ Confirmed |

**Total: 9/9 automated assertions passed**

Postman collection exported as JSON and available in the folder.

> See screenshots, scripts and full details in [API Testing Postman](./API%20Testing%20Postman) folder.

---

## 🛠 Tools & Skills

| Category | Tools |
|---|---|
| Bug Tracking | Jira |
| Test Management | Zephyr Scale |
| API Testing | Postman, Chrome DevTools |
| Test Design Techniques | Equivalence Partitioning, Boundary Value Analysis |
| Documentation | Excel, Markdown |
| Data Formats | JSON, REST API |
| Scripting | JavaScript (Postman Scripts) |
| Cross-browser Testing | Chrome, Firefox, Safari, Edge |

---

📜 Certificate: QA Manual (SSWU QA001) — Sigma Software University, June 2026

