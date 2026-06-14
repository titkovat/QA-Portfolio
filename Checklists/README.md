# Checklist — cars.ua

Manual testing checklist for [cars.ua](https://cars.ua) — Ukrainian car marketplace.

**Total checks: 15**
**Modules covered:** UI, Login Validation, Filters
**Testing type:** Manual / Functional / Cross-browser

---

## Summary Table

| Module | Total Checks | Passed | Failed | Not Tested |
|---|---|---|---|---|
| UI | 7 | 1 | 0 | 6 |
| Login Validation | 6 | 0 | 0 | 6 |
| Checking Filters | 1 | 0 | 0 | 1 |
| **Total** | **15** | **1** | **0** | **14** |

---

## ✅ Module 1 — UI

| # | Test | Status | Test Data | Comments |
|---|---|---|---|---|
| 1 | Homepage loads correctly | Passed | URL: cars.ua | Page loads without errors |
| 2 | Search field is displayed | — | — | Search field is available for input |
| 3 | Site logo is displayed | — | — | Logo is visible in the header |
| 4 | Search button is active | — | — | Button is clickable |
| 5 | Banners and images load | — | — | No broken images |
| 6 | "Login" button click | — | — | Redirects to the login page |
| 7 | Telegram icon in footer is active | — | — | Button is clickable |

---

## ✅ Module 2 — Login Validation

| # | Test | Status | Test Data | Comments |
|---|---|---|---|---|
| 1 | Login with valid phone number | — | 380991112233 | User successfully authenticates |
| 2 | "Login" button is active | — | — | Button is available for clicking |
| 3 | Phone number field accepts valid number | — | 380991112233 | Number is entered correctly |
| 4 | Field does not accept too long number | — | 380991112233445 | Error message: "incorrect phone number" |
| 5 | Field does not accept special characters | — | \*\*\*\*\*\*\* | Error message: "incorrect phone number" |
| 6 | Clicking "Login" after entering valid number | — | Valid number | Opens SMS code verification page |

---

## ✅ Module 3 — Checking Filters

| # | Test | Status | Test Data | Comments |
|---|---|---|---|---|
| 1 | Check "All brands" filter | — | Honda | Search runs successfully, all Honda cars are displayed |

---

## 🌐 Cross-browser Testing

| Browser | Version | Result |
|---|---|---|
| Google Chrome | Latest | ✅ Tested |
| Mozilla Firefox | Latest | — |
| Safari | Latest | — |
| Microsoft Edge | Latest | — |

---

## 📁 Files in this folder

| File | Description |
|---|---|
| `Checklist_CarsUA.xlsx` | Full checklist in Excel format |
| `README.md` | Checklist summary (this file) |

