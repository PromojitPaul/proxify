# 📌 Proxify Testing Documentation  & Bug Report
## 📝 Overview
This repository contains detailed bug reports, test cases, and UI issues found during the testing of the **Proxify** platform. The primary focus was on functionality, UI responsiveness, and payment flow.

## 📂 Project Structure
```
📦 Proxify-Testing
├── 🐞 Bug Reports
│   ├── UI_issues.md
│   ├── Payment_Flow_Bugs.md
│   └── Layout_Bugs.md
├── ✅ Test Cases
│   ├── TestCases_PlanPage.md
│   ├── TestCases_Payment.md
│   └── TestCases_Invoice.md
├── 📸 Screenshots
│   ├── Plans_Page_Issue.png
│   ├── Invoice_Page_Issue.png
│   ├── Payment_Button_Disabled.png
│   └── UI_Button_Bug.png
└── README.md
```

---

## 🛠️ Identified Bugs & Issues
### 1️⃣ **Buy Now Button UI Issue**
- **Description:** Clicking one **Buy Now** button triggers a click animation on all Buy Now buttons.
- **Steps to Reproduce:**
  1. Go to the "Plans" page.
  2. Click on any "Buy Now" button.
  3. Observe that all Buy Now buttons appear to be clicked.
- **Expected Result:** Only the clicked button should show the animation.
- **Actual Result:** All buttons show the click animation.
- **Severity:** Medium
- **Priority:** High

### 2️⃣ **Payment Options Disabled Issue**
- **Description:** When redirected to the payment page, **Pay with Cryptomus**, **WalletConnect**, and **Pay by Card** buttons are disabled.
- **Steps to Reproduce:**
  1. Click "Buy Now" on any plan.
  2. Proceed to the payment page.
  3. Select **Crypto** as a payment method.
  4. Observe that payment options are disabled.
- **Expected Result:** All payment options should be enabled for selection.
- **Actual Result:** Sometimes only **WalletConnect** works; other options remain disabled.
- **Severity:** High
- **Priority:** Critical

### 3️⃣ **Plans & Invoice Page Layout Issues**
- **Description:** Misalignment and overlapping UI elements on the **Plans** and **Invoice** pages.
- **Steps to Reproduce:**
  1. Navigate to the "Plans" page.
  2. Observe layout and alignment issues.
  3. Navigate to the "Invoice" page.
  4. Observe similar layout inconsistencies.
- **Expected Result:** The layout should be properly structured and aligned.
- **Actual Result:** UI elements appear misaligned or overlapped.
- **Severity:** Medium
- **Priority:** Medium

---

## 📋 Test Cases
| Test Case ID | Test Scenario | Test Case Description | Pre-requisites | Test Steps | Test Data | Expected Result (ER) | Actual Result | Result |
|-------------|--------------|----------------------|---------------|------------|----------|-------------------|--------------|--------|
| TC-001 | Buy Now Button UI Issue | Check if clicking one "Buy Now" button affects others | Access to "Plans" page | Click on "Buy Now" button | N/A | Only the clicked button shows animation | All buttons show animation | ❌ Fail |
| TC-002 | Payment Options Availability | Verify that all payment options are enabled | Access to payment page | Click "Buy Now", choose Crypto, proceed | N/A | All options are enabled | Some options disabled | ❌ Fail |
| TC-003 | Layout Issues on Plans Page | Check for UI alignment issues | Access to "Plans" page | Navigate to "Plans" page | N/A | Properly structured layout | Misalignment issues found | ❌ Fail |
| TC-004 | Layout Issues on Invoice Page | Check for UI alignment issues | Access to "Invoice" page | Navigate to "Invoice" page | N/A | Properly structured layout | Misalignment issues found | ❌ Fail |

---

## 📷 Screenshots
| Bug Description | Screenshot |
|----------------|------------|
| Buy Now Button UI Issue | ![Buy Now Issue](Screenshots/UI_Button_Bug.png) |
| Payment Options Disabled | ![Payment Issue](Screenshots/Payment_Button_Disabled.png) |
| Plans Page Layout Issue | ![Plans Issue](Screenshots/Plans_Page_Issue.png) |
| Invoice Page Layout Issue | ![Invoice Issue](Screenshots/Invoice_Page_Issue.png) |

---

## 🚀 How to Report New Issues
1. Go to the **Issues** tab in this repository.
2. Click **New Issue**.
3. Provide a clear title and description.
4. Add **steps to reproduce**, **expected vs actual results**, and **screenshots** if applicable.
5. Assign the issue to a relevant category (**UI Bug**, **Functional Bug**, **Payment Issue**, etc.).

---

## 🔧 Tools Used
- **Browser:** Chrome, Firefox
- **Testing Tools:** Bugasura, Jira
- **Automation:** Selenium (for UI automation testing)

📧 **For any queries, contact:** support@proxify.gg

**Contributors:** [PromojitPaul](https://github.com/PromojitPaul)
