# Bug Reports — cars.ua

Manual testing of [cars.ua](https://cars.ua) — Ukrainian car marketplace.

**Total bugs found: 3**
**Environment:** Chrome 148.0.7778.168 (Official Build) (64-bit), Windows 10 Pro Version 22H2
**Testing type:** Manual / Exploratory

---

## Summary Table

| ID | Title | Priority | Severity | Status |
|---|---|---|---|---|
| [BUG-001](#bug-001) | Viber Chatbot link does not open | High | Medium | Open |
| [BUG-002](#bug-002) | Registration page returns HTTP 500 | High | Critical | Open |
| [BUG-003](#bug-003) | City names displayed in Russian on Ukrainian version | Medium | Low | Open |

---

## BUG-001

**Title:** Viber Chatbot link does not open after clicking

| Field | Details |
|---|---|
| **Priority** | High |
| **Severity** | Medium |

**Preconditions:**
1. User has opened cars.ua
2. Page is fully loaded

**Steps to Reproduce:**
1. Open cars.ua
2. Scroll down to the footer
3. Find the chatbot block (Viber and Telegram)
4. Click on the Viber chatbot "car.ua"

**Actual Result:**
After clicking the Viber Chatbot link, no page opens and no redirect occurs.

**Expected Result:**
The Viber chatbot link should open correctly and redirect the user to the Viber messenger.

**Attachment:**

![BUG-001 Screenshot](screenshots/BUG-001_viber_link.png)

---

## BUG-002

**Title:** Registration button on "For Dealers" page returns HTTP 500

| Field | Details |
|---|---|
| **Priority** | High |
| **Severity** | Critical |

**Preconditions:**
1. cars.ua homepage is open

**Steps to Reproduce:**
1. Open cars.ua
2. Scroll down to the footer
3. Click the "For Dealers" link
4. On the "Register your dealership for free" page, click the "Registration" button

**Actual Result:**
A page opens with the message: "Page unavailable. Cars.ua cannot process this request at the moment. HTTP ERROR 500."

**Expected Result:**
After clicking "Registration", the user should be redirected to the dealership registration page without any system errors.

**Attachment:**

![BUG-002 Screenshot](screenshots/BUG-002_http500.png)

---

## BUG-003

**Title:** City names displayed in Russian in the filter dropdown on Ukrainian version

| Field | Details |
|---|---|
| **Priority** | Medium |
| **Severity** | Low |

**Preconditions:**
1. Ukrainian version of cars.ua is open
2. Homepage is fully loaded

**Steps to Reproduce:**
1. Open cars.ua
2. Find the filters block on the homepage
3. Click on the "All cities" dropdown

**Actual Result:**
The site interface is displayed in Ukrainian, but city names in the dropdown are shown in Russian.

**Expected Result:**
City names should be displayed in Ukrainian, consistent with the site's localization.

**Attachment:**

![BUG-003 Screenshot](screenshots/BUG-003_russian_cities.png)

---

## 📁 Files in this folder

| File | Description |
|---|---|
| `CarsUA_Bug_Reports.xlsx` | Full bug reports in Excel format with screenshots |
| `README.md` | Bug report summary (this file) |
| `screenshots/` | Screenshots for each bug |



