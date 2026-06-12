# 🧪 Manual Testing — Jira + Zephyr Scale

**Project under test:** [Cars.UA](https://cars.ua) — car search and dealership registration features  
**Tools:** Jira (bug tracking) · Zephyr Scale (test management)  
**Test type:** Manual functional testing  
**Scope:** Car search functionality + UI navigation + external links

---

## 📋 Test Cases (Zephyr Scale)

| Key | Test Case Name | Steps | Status |
|-----|---------------|-------|--------|
| KAN-T1 | Filter cars by brand | 3 | ✅ Approved / PASS |
| KAN-T2 | Search car by model | 3 | ✅ Approved / PASS |
| KAN-T3 | Search car using lowercase input | 3 | ✅ Approved / FAIL → Bug KAN-1 |

### KAN-T1 — Filter cars by brand

| Step | Action | Test Data | Expected Result |
|------|--------|-----------|----------------|
| 1 | Open the car search page | — | Search page is displayed |
| 2 | Select 'Volkswagen' in the brand filter | Brand = Volkswagen | Filter is applied |
| 3 | Apply the filter | — | Only Volkswagen cars are displayed |

### KAN-T2 — Search car by model

| Step | Action | Test Data | Expected Result |
|------|--------|-----------|----------------|
| 1 | Click on the search field | — | Cursor appears in the search field |
| 2 | Type «Toyota Camry» | "Toyota Camry" | Text is entered correctly |
| 3 | Click the search button | — | Results matching "Toyota Camry" are displayed |

### KAN-T3 — Search car using lowercase input

| Step | Action | Test Data | Expected Result |
|------|--------|-----------|----------------|
| 1 | Click on the search field | — | Cursor appears in the search field |
| 2 | Type «toyota camry» in lowercase | "toyota camry" | Text is entered correctly |
| 3 | Click the search button | — | Results matching "Toyota Camry" are displayed (search is case-insensitive) |

---

## 🔴 Bug Reports

### KAN-1 — Viber Chatbot link in footer does not open after click

| Field | Details |
|-------|---------|
| **ID** | KAN-1 |
| **Summary** | Viber Chatbot link in footer does not open after click |
| **Severity** | Medium |
| **Priority** | Medium |
| **Status** | To Do |
| **Environment** | Chrome 148.0.7778.168 (64-bit) · Windows 10 Pro 22H2 |

**Preconditions:**
1. User opens [cars.ua](https://cars.ua)
2. Page is fully loaded

**Steps to Reproduce:**
1. Scroll the page down to the footer
2. Find the chat-bot block (Viber and Telegram)
3. Click on the Viber chatbot link «car.ua»

**Expected Result:**  
The Viber chatbot link opens correctly and redirects the user to the Viber messenger.

**Actual Result:**  
After clicking the Viber Chatbot link, no page opens and no redirect occurs.

**Console Error:**
```
Failed to launch 'viber://pa?chatURI=carsuabot' because the scheme does not have a registered handler
```

---

### KAN-2 — "Registration" button on "Dealerships" page opens HTTP Error 500

| Field | Details |
|-------|---------|
| **ID** | KAN-2 |
| **Summary** | "Registration" button on "Dealerships" page opens HTTP Error 500 |
| **Severity** | Critical |
| **Priority** | High |
| **Status** | To Do |
| **Environment** | Chrome 148.0.7778.168 (64-bit) · Windows 10 Pro 22H2 |

**Preconditions:**  
Open the main page of [cars.ua](https://cars.ua)

**Steps to Reproduce:**
1. Open [cars.ua](https://cars.ua)
2. Scroll down to the footer
3. Click the «Автоділери» (Dealerships) link
4. On the "Register your dealership for free" page, click the «Реєстрація» (Registration) button

**Expected Result:**  
After clicking "Registration", the user is redirected to the dealership registration page without system errors.

**Actual Result:**  
A page opens with the message: *"Page unavailable. http://Cars.ua cannot process this request. HTTP ERROR 500"*

**Console Error:**
```
(index):1 Unsafe attempt to load URL https://cars.ua/sf/d-dealer-form/ from frame
```

---

## 📊 Test Execution Summary (Zephyr Report)

| Metric | Value |
|--------|-------|
| Total test cases | 3 |
| Executed | 3 (100%) |
| Passed | 2 |
| Failed | 1 |
| Execution time | 19s |
| Bugs filed | 2 (KAN-1, KAN-2) |

> **Result:** 2 out of 3 test cases passed. 1 failure resulted in 2 bug reports filed in Jira.  
> Both bugs are reproducible and confirmed with browser console errors.

---

## 🗂️ Screenshots

| File | Description |
|------|-------------|
| `screenshots/test-cases-list.png` | Zephyr — list of all test cases |
| `screenshots/tc-kan-t1.png` | KAN-T1 test script — Filter by brand |
| `screenshots/tc-kan-t2.png` | KAN-T2 test script — Search by model |
| `screenshots/tc-kan-t3.png` | KAN-T3 test script — Lowercase search |
| `screenshots/test-results-summary.png` | Zephyr — test execution report |
| `screenshots/bug-kan-1.png` | KAN-1 bug report — Viber link broken |
| `screenshots/bug-kan-2.png` | KAN-2 bug report — HTTP 500 on Registration |

---

*Testing performed by Tetiana Titkova · Junior QA Engineer*  
*[LinkedIn](https://www.linkedin.com/in/titkova-889670d) · [GitHub Portfolio](https://github.com/titkovat/QA-Portfolio)*

