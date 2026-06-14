# Test Plan — TableTime Booking System

| Field | Details |
|---|---|
| **Project** | TableTime |
| **Version** | Web & Mobile Web |
| **Date** | November 4, 2026 |
| **Author** | Tetiana Titkova |

---

## 1. 🎯 Test Objectives

Verify system stability after implementing updates, including:

- Validate correct operation of all core and new system features
- Validate booking business logic (tables and event halls)
- Verify online payment and refund processes
- Ensure correct operation of the cancellation feature (24-hour policy)
- Verify integrations (email notifications, payment systems)
- Identify defects before product release
- Evaluate usability and interface responsiveness

**Goal:** Confirm that new features work correctly and that key business processes (search, booking, payment) are not broken.

---

## 2. 📋 Scope of Testing

### ✅ In Scope

- Online table booking
- Hall booking for events
- Date, time, and guest count selection
- Booking type selection ("table" or "hall")
- Online payment
- Booking confirmation via email
- Booking cancellation (up to 24 hours before)
- Automatic refund processing
- Booking management from user profile page
- Mobile Web responsiveness

### ❌ Out of Scope

- User registration and authentication
- Customer support system (chat, feedback form)
- Mobile push notifications

---

## 3. 🔬 Test Levels

| Level | Description |
|---|---|
| **Unit Testing** | Performed by developers. Verifies individual components (e.g., cancellation time calculation, refund logic) |
| **Integration Testing** | Verifies interactions between: payment systems (Apple Pay / Google Pay), booking + payment, booking + email |
| **System Testing** | Full system testing as a single product. End-to-end scenarios from booking creation to cancellation |
| **Acceptance Testing (UAT)** | Verifies compliance with business requirements. Performed by the client or business analysts |

---

## 4. 🧪 Types of Testing

| Type | Description |
|---|---|
| **Functional** | Verify all features according to requirements |
| **Non-functional** | Performance (booking processing speed), Security (payment data protection), Usability |
| **Regression** | Ensure new features (halls, payment, cancellation) have not broken existing functionality |
| **Smoke Testing** | Quick check of core functionality after each new build |
| **Sanity Testing** | Targeted check of specific changes (e.g., cancellation feature only) |
| **UI/UX Testing** | Interface element display, ease of use |
| **Cross-browser Testing** | Verify functionality across different browsers |
| **Responsive Testing** | Verify behavior on different screen sizes (mobile devices) |

---

## 5. 📐 Test Approach

### Strategy
Combination of manual and automated testing with primary focus on critical business processes:
- Booking
- Payment
- Cancellation

### Manual Testing
Used for:
- UI/UX checks
- Exploratory testing
- Complex business scenarios

### Automated Testing
Used for:
- Regression tests
- Smoke tests
- API testing

### Test Prioritization

| Priority | Areas |
|---|---|
| 🔴 High | Payment, refunds, booking |
| 🟡 Medium | Email confirmation, user profile |
| 🟢 Low | UI details |

### Defect Management
- All defects logged in **Jira**
- Priority levels: `Blocker` → `Critical` → `Major` → `Minor`

### Test Design Techniques
- Equivalence Partitioning
- Boundary Value Analysis
- Decision Table Testing
- State Transition Testing

---

## 6. 🖥️ Test Environment

### Hardware
- Desktop PCs and laptops
- Smartphones and tablets

### Software

| Category | Details |
|---|---|
| **OS** | Windows, macOS, Android, iOS |
| **Browsers** | Google Chrome, Mozilla Firefox, Safari, Microsoft Edge (latest versions) |

### Tools

| Tool | Purpose |
|---|---|
| **Jira** | Bug tracking and defect management |
| **TestRail / Google Sheets** | Test case creation and management |
| **Postman** | API testing (booking, payment, refunds) |
| **BrowserStack / real devices** | Cross-browser and mobile testing |
| **Mailtrap / test email** | Email confirmation verification |

---

## 7. 👥 Resources

| Role | Count | Responsibilities |
|---|---|---|
| Senior QA | 1 | Planning, reporting |
| QA Engineer | 1 | Test execution, bug reporting |
| Developer | 2 | Defect fixes, environment support |

---

## 8. 📅 Schedule

| Phase | Period |
|---|---|
| Test case preparation | November 4–6 |
| Test execution | November 7–10 |
| Regression testing | November 11–12 |
| Reporting | November 13 |

---

## 9. ⚠️ Risks

| Risk | Mitigation |
|---|---|
| Insufficient test data may slow down testing | Prepare test data in advance |

---

## 10. ✅ Exit Criteria

1. All critical and high-priority defects are fixed
2. 100% of critical test cases have been executed
3. No blocking defects remain open
4. Test results are documented in TestRail
5. Final summary report with release recommendation is prepared
