# 👩‍💻 QA Portfolio — Tetiana Titkova

**Junior QA Engineer** · Manual Testing · Test Documentation · Bug Reporting · Jira · Zephyr · API Testing

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Tetiana_Titkova-0077B5?style=flat&logo=linkedin)](https://www.linkedin.com/in/titkova-889670d)
[![GitHub](https://img.shields.io/badge/GitHub-titkovat-181717?style=flat&logo=github)](https://github.com/titkovat)

---

## 🗂️ Portfolio Structure

| Folder | What's inside | Tools |
|--------|--------------|-------|
| [📁 Jira-Zephyr](#-jira--zephyr-scale) | Test cases, bug reports, test execution report for Cars.UA | Jira, Zephyr Scale |
| [📁 Test-Cases](#-test-cases) | Manual test cases in table format | Excel / Google Sheets |
| [📁 Checklists](#-checklists) | Testing checklists for UI and functionality | Markdown / Excel |
| [📁 Bug-Reports](#-bug-reports) | Detailed bug reports with steps, expected/actual results | Jira |
| [📁 API-Testing](#-api-testing) | API test cases for GoRest v2 /users endpoint | Hoppscotch, Postman |

---

## 🐛 Jira + Zephyr Scale

**Project:** [Cars.UA](https://cars.ua) — car marketplace  
**Scope:** Car search functionality, UI navigation, external links, dealership registration

### Test Cases (Zephyr Scale)

| Key | Test Case | Result |
|-----|-----------|--------|
| KAN-T1 | Filter cars by brand (Volkswagen) | ✅ PASS |
| KAN-T2 | Search car by model (Toyota Camry) | ✅ PASS |
| KAN-T3 | Search using lowercase input | ❌ FAIL → [KAN-1] |

### Bug Reports (Jira)

| Key | Summary | Severity | Status |
|-----|---------|----------|--------|
| KAN-1 | Viber Chatbot link in footer does not open | Medium | 🔴 Open |
| KAN-2 | "Registration" button on Dealerships page returns HTTP 500 | Critical | 🔴 Open |

### Test Execution Summary

```
Total: 3  |  Passed: 2  |  Failed: 1  |  Bugs filed: 2
```

📂 Full documentation with screenshots: [Jira-Zephyr/README.md](./Jira-Zephyr/README.md)

---

## 📋 Test Cases

Manual test cases written in table format covering functional scenarios.

**Format:** TC ID · Description · Preconditions · Steps · Expected Result · Actual Result · Status

📂 See: [Test-Cases/](./Test-Cases/)

---

## ✅ Checklists

Testing checklists for quick sanity checks and regression rounds.

📂 See: [Checklists/](./Checklists/)

---

## 🔴 Bug Reports

Detailed bug reports following standard QA format:
- Summary
- Preconditions
- Steps to Reproduce
- Expected vs Actual Result
- Environment
- Console errors / attachments

📂 See: [Bug-Reports/](./Bug-Reports/)

---

## 🔌 API Testing

**API under test:** [GoRest v2](https://gorest.co.in) — public REST API  
**Tool:** Hoppscotch  
**Endpoint:** `POST /public/v2/users`

**Covered scenarios:**

| Method | Scenario | Expected Status |
|--------|----------|----------------|
| POST | Create user — valid data | 201 Created |
| POST | Create user — missing email | 422 Unprocessable |
| POST | Create user — duplicate email | 422 Unprocessable |
| POST | Create user — invalid gender | 422 Unprocessable |
| POST | No auth token | 401 Unauthorized |
| GET | Get list of users | 200 OK |
| GET | Get user by valid id | 200 OK |
| GET | Get user by non-existent id | 404 Not Found |
| PUT | Update user name | 200 OK |
| DELETE | Delete existing user | 204 No Content |
| DELETE | Delete already-deleted user | 404 Not Found |
| GET | Pagination (page + per_page) | 200 OK |

📂 Full test case table: [API-Testing/GoRest_API_Test_Cases.xlsx](./API-Testing/GoRest_API_Test_Cases.xlsx)

---

## 🛠️ Tools & Skills

| Category | Tools |
|----------|-------|
| Test Management | Jira, Zephyr Scale |
| API Testing | Hoppscotch, Postman |
| Documentation | Excel, Google Sheets, Markdown |
| Version Control | GitHub |
| Other | Chrome DevTools, ERP systems |

---

## 📚 Currently Learning

- QA Fundamentals Course — **Sigma Software University** (2025, in progress)
- Completed: QA Tester Course — Diia.Education

---

*Open to Junior QA Engineer opportunities · Remote or Kryvyi Rih, Ukraine*  
📧 titkovat85@ukr.net · [LinkedIn](https://www.linkedin.com/in/titkova-889670d)

