# Test Cases — cars.ua

Manual test cases for [cars.ua](https://cars.ua) — Ukrainian car marketplace.

**Total test cases: 7**
**Tested functionality:** Car Search, Listing Filters
**Testing type:** Manual / Functional

---

## 🎯 Test Design Techniques Used

| Technique | Applied to |
|---|---|
| Equivalence Partitioning | TC-SEARCH-001, TC-SEARCH-002, TC-SEARCH-003, TC-SEARCH-004, TC-SEARCH-005 |
| Boundary Value Analysis | TC-SEARCH-006, TC-FILTER-001 |

---

## Summary Table

| ID | Title | Type | Priority | Status |
|---|---|---|---|---|
| [TC-SEARCH-001](#tc-search-001) | Search by valid car brand name | Positive | High | Pass |
| [TC-SEARCH-002](#tc-search-002) | Search by car model | Positive | High | Pass |
| [TC-SEARCH-003](#tc-search-003) | Search using lowercase letters | Positive | Medium | Pass |
| [TC-SEARCH-004](#tc-search-004) | Search with non-existent value | Negative | High | Pass |
| [TC-SEARCH-005](#tc-search-005) | Search with special characters | Negative | High | Pass |
| [TC-SEARCH-006](#tc-search-006) | Search with maximum length input | Boundary | Medium | Pass |
| [TC-FILTER-001](#tc-filter-001) | Filter listings by car brand | Positive | High | Pass |

---

## 🔍 Car Search Functionality

### TC-SEARCH-001

**Title:** Search by valid car brand name

| Field | Details |
|---|---|
| **Type** | Positive |
| **Technique** | Equivalence Partitioning |
| **Preconditions** | cars.ua is open |

**Steps to Reproduce:**
1. Click on the search field
2. Enter "BMW"
3. Click the search button

**Expected Result:**
- Listings for BMW cars are displayed
- Results match the entered query

---

### TC-SEARCH-002

**Title:** Search by car model

| Field | Details |
|---|---|
| **Type** | Positive |
| **Technique** | Equivalence Partitioning |
| **Preconditions** | cars.ua is open |

**Steps to Reproduce:**
1. Click on the search field
2. Enter "Toyota Camry"
3. Click the search button

**Expected Result:**
- Listings for Toyota Camry are displayed
- Results match the entered query

---

### TC-SEARCH-003

**Title:** Search using lowercase letters

| Field | Details |
|---|---|
| **Type** | Positive |
| **Technique** | Equivalence Partitioning |
| **Preconditions** | cars.ua is open |

**Steps to Reproduce:**
1. Click on the search field
2. Enter "toyota camry" in lowercase
3. Click the search button

**Expected Result:**
- The system correctly finds Toyota Camry cars regardless of letter case

---

### TC-SEARCH-004

**Title:** Search with non-existent value

| Field | Details |
|---|---|
| **Type** | Negative |
| **Technique** | Equivalence Partitioning |
| **Preconditions** | cars.ua is open |

**Steps to Reproduce:**
1. Click on the search field
2. Enter "abcdef12345"
3. Click the search button

**Expected Result:**
- A "no results found" message is displayed
- The site does not freeze or show an error

---

### TC-SEARCH-005

**Title:** Search with special characters

| Field | Details |
|---|---|
| **Type** | Negative |
| **Technique** | Equivalence Partitioning |
| **Preconditions** | cars.ua is open |

**Steps to Reproduce:**
1. Click on the search field
2. Enter "@@@@@@@"
3. Click the search button

**Expected Result:**
- A "no results found" or "invalid query" message is displayed
- The site does not freeze or show an error

---

### TC-SEARCH-006

**Title:** Search with maximum length input

| Field | Details |
|---|---|
| **Type** | Boundary |
| **Technique** | Boundary Value Analysis |
| **Preconditions** | cars.ua is open |

**Steps to Reproduce:**
1. Click on the search field
2. Enter a very long text (257 characters)
3. Click the search button

**Expected Result:**
- The field handles the input without crashes
- The system does not break
- If applicable, a message about input length limit is displayed

---

## 🔧 Listing Filter Functionality

### TC-FILTER-001

**Title:** Filter listings by car brand

| Field | Details |
|---|---|
| **Type** | Positive |
| **Technique** | Equivalence Partitioning |
| **Preconditions** | cars.ua is open |

**Steps to Reproduce:**
1. Open the car search page
2. Select "Volkswagen" in the brand filter
3. Apply the filter

**Expected Result:**
- Only Volkswagen cars are displayed in the results

---

## 📁 Files in this folder

| File | Description |
|---|---|
| `TEST_CASES.pdf` | Full test cases document |
| `README.md` | Test cases summary (this file) |

