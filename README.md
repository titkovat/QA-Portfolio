#  QA Portfolio — Tetiana Titkova

**Junior QA Engineer · Manual Testing · Test Documentation · Bug Reporting · API Testing · Jira · Zephyr Scale**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Tetiana%20Titkova-blue)](https://www.linkedin.com/in/tetiana-titkova)
[![GitHub](https://img.shields.io/badge/GitHub-titkovat-black)](https://github.com/titkovat)

---

##  Portfolio Structure

| Folder | What's inside | Tools |
|---|---|---|
| 📂 [Jira-Zephyr](./Jira-Zephyr) | Test cases, bug reports, test execution report for Cars.UA | Jira, Zephyr Scale |
| 📂 [Test-Cases](./Test-Cases) | Manual test cases with test design techniques | Excel |
| 📂 [Checklists](./Checklists) | UI and functional testing checklists | Excel |
| 📂 [Bug-Reports](./Bug-Reports) | Detailed bug reports with steps, screenshots | Jira |
| 📂 [API Testing Postman](./API%20Testing%20Postman) | REST API testing with automated assertions | Postman, JSON |
| 📂 [Test-Plan](./Test-Plan) | Full test plan for TableTime booking system | — |

---

##  Jira + Zephyr Scale

**Project:** [Cars.UA](https://cars.ua) — car marketplace
**Scope:** Car search functionality, UI navigation, external links, dealership registration
**Tools:** Jira (bug tracking) · Zephyr Scale (test management)

| Key | Test Case | Status |
|---|---|---|
| KAN-T1 | Filter cars by brand | ✅ PASS |
| KAN-T2 | Search car by model | ✅ PASS |
| KAN-T3 | Search car using lowercase input | ❌ FAIL → Bug KAN-1 |

> See full details in [Jira-Zephyr](./Jira-Zephyr) folder.

---

## Test Cases

Manual test cases written for **cars.ua** covering search and filter functionality.

| ID | Title | Type | Technique |
|---|---|---|---|
| TC-SEARCH-001 | Search by valid car brand (BMW) | Positive | Equivalence Partitioning |
| TC-SEARCH-002 | Search by car model (Toyota Camry) | Positive | Equivalence Partitioning |
| TC-SEARCH-003 | Search using lowercase letters | Positive | Equivalence Partitioning |
| TC-SEARCH-004 | Search with non-existent value | Negative | Equivalence Partitioning |
| TC-SEARCH-005 | Search with special characters | Negative | Equivalence Partitioning |
| TC-SEARCH-006 | Search with maximum length input (257 chars) | Boundary | Boundary Value Analysis |
| TC-FILTER-001 | Filter listings by car brand (Volkswagen) | Positive | Equivalence Partitioning |

> See full details in [Test-Cases](./Test-Cases) folder.

---

##  Checklists

UI and functional checklists for **cars.ua**:

| Module | Checks |
|---|---|
| UI | Homepage load, search field, logo, search button, banners, login button, Telegram icon |
| Login Validation | Valid phone, too long number, special characters, SMS redirect |
| Filters | Brand filter (Honda) |
| Cross-browser | Chrome, Firefox, Safari, Edge |

> See full details in [Checklists](./Checklists) folder.

---

##  Bug Reports

3 bugs found and documented during manual testing of **cars.ua**:

| ID | Title | Priority | Severity |
|---|---|---|---|
| BUG-001 | Viber Chatbot link does not open | High | Medium |
| BUG-002 | Registration page returns HTTP 500 | High | Critical |
| BUG-003 | City names displayed in Russian on Ukrainian version | Medium | Low |

> See full details in [Bug-Reports](./Bug-Reports) folder.

---

##  API Testing with Postman

**APIs tested:** cars.ua API + GoRest public API

| Method | Endpoint | Status | Assertions |
|---|---|---|---|
| GET | cars.ua/api/v2/model/records?make_id=9 | ✅ 200 OK | 3/3 |
| POST | gorest.co.in/public/v2/users | ✅ 201 Created | 3/3 |
| PATCH | gorest.co.in/public/v2/users/{id} | ✅ 200 OK | 2/2 |
| DELETE | gorest.co.in/public/v2/users/{id} | ✅ 204 No Content | 1/1 |
| GET | gorest.co.in/public/v2/users/{id} | ✅ 404 Not Found | confirmed |

**Total: 9/9 automated assertions passed**

> See screenshots, scripts and full details in [API Testing Postman](./API%20Testing%20Postman) folder.

---

##  Test Plan

Full test plan created for **TableTime** — online table and event hall booking system.

| Field | Details |
|---|---|
| Scope | Booking, payment, cancellation, email confirmation, mobile web |
| Test Types | Functional, Regression, Smoke, Sanity, UI/UX, Cross-browser, Responsive |
| Techniques | Equivalence Partitioning, Boundary Value Analysis, Decision Table, State Transition |
| Tools | Jira, TestRail, Postman, BrowserStack, Mailtrap |

> See full document in [Test-Plan](./Test-Plan) folder.

---

##  Tools & Skills

| Category | Tools |
|---|---|
| Bug Tracking | Jira |
| Test Management | Zephyr Scale |
| API Testing | Postman, Chrome DevTools |
| Test Design Techniques | Equivalence Partitioning, Boundary Value Analysis, Decision Table, State Transition |
| Documentation | Excel, Markdown |
| Data Formats | JSON, REST API |
| Scripting | JavaScript (Postman Scripts) |
| Cross-browser Testing | Chrome, Firefox, Safari, Edge |

---

 **Certificate:** QA Manual (SSWU QA001) — Sigma Software University, June 2026
