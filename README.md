# SauceDemo Manual Testing Project

Details about the project structure, modules covered, and tools used.

```plaintext
SauceDemo_Manual_QA_Project/
│
├── 📂 1_Test_Plan/              # Test strategy, scope, and planning
│   └── SauceDemo_TestPlan.docx
│
├── 📂 2_Test_Cases/             # Manual test cases for key modules
│   ├── Login_Module_TestCases.xlsx
│   ├── Cart_Module_TestCases.xlsx
│   └── Checkout_Module_TestCases.xlsx
│
├── 📂 3_Test_Execution_Reports/ # Test results with status and comments
│   └── TestExecutionReport.xlsx
│
├── 📂 4_Bug_Reports/            # Reported issues and bug tracking
│   ├── BugReport_Template.docx
│   ├── BugReport_#101_LoginError.docx
│   └── BugReport_#102_CheckoutFail.docx
│
├── 📂 5_Test_Scenarios/         # High-level test scenario outlines
│   └── SauceDemo_TestScenarios.xlsx
│
├── 📂 6_Traceability_Matrix/    # RTM mapping requirements to test cases
│   └── RTM_SauceDemo.xlsx
│
├── 📂 7_README/                 # Project documentation
│   └── README.md
│
├── 📄 .gitignore                # Git ignore rules (optional)
└── 📄 README.md                 # Project summary and documentation

```





























## 📌 Step-by-Step Manual Testing Process:

### ✅ 1. Requirement Analysis
Analyze the SauceDemo website: https://www.saucedemo.com/

**Core Modules:**
- Login
- Product Listing
- Cart Management
- Checkout
- Order Confirmation
- Logout

### ✅ 2. Test Plan Creation
📁 `1_Test_Plan/SauceDemo_TestPlan.docx`

**Contents of Test Plan:**
- Objective & Scope
- In-scope and Out-of-scope
- Test Environment
- Assumptions & Constraints
- Test Deliverables
- Entry/Exit Criteria
- Schedule and Timeline
- Roles & Responsibilities

### ✅ 3. Test Scenario Design
📁 `5_Test_Scenarios/SauceDemo_TestScenarios.xlsx`

| Module       | Test Scenario                               | Priority |
|--------------|---------------------------------------------|----------|
| Login        | Verify login with valid credentials         | High     |
| Login        | Verify error message with invalid credentials| High     |
| Product Page | Add multiple products to the cart           | Medium   |
| Cart         | Remove a product from the cart              | Medium   |
| Checkout     | Complete checkout with valid data           | High     |
| Logout       | Verify user is logged out properly          | Low      |

### ✅ 4. Test Case Design
📁 `2_Test_Cases/`

Example: `Login_Module_TestCases.xlsx`

| TC ID | Test Scenario     | Steps to Execute                      | Test Data                 | Expected Result                          | Status |
|-------|-------------------|---------------------------------------|---------------------------|------------------------------------------|--------|
| TC001 | Valid Login       | Open URL, Enter credentials, Login    | standard_user / secret_sauce | Redirect to Inventory page          | Pass   |
| TC002 | Invalid Password  | Enter valid username, wrong password  | standard_user / wrong_pass | Show error message                    | Fail   |

### ✅ 5. Test Execution
📁 `3_Test_Execution_Reports/TestExecutionReport.xlsx`

| Test Case ID | Status | Comments                    |
|--------------|--------|-----------------------------|
| TC001        | Pass   | As expected                 |
| TC002        | Fail   | Incorrect error message     |
| TC003        | Pass   | Cart updated successfully   |

### ✅ 6. Bug Reporting
📁 `4_Bug_Reports/`

Example: `BugReport_#101_LoginError.docx`

**Bug Report:**
- Bug ID: 101
- Module: Login
- Severity: High
- Priority: High
- Description: Login fails with valid credentials on Firefox
- Steps to Reproduce:
  1. Go to login page
  2. Enter valid credentials
  3. Click login
- Expected Result: Redirect to inventory page
- Actual Result: Page reloads with no action
- Status: Open
- Reported By: Tushar
- Date: 10-July-2025

📁 `BugReport_Template.docx` — Reusable bug format

### ✅ 7. Requirement Traceability Matrix (RTM)
📁 `6_Traceability_Matrix/RTM_SauceDemo.xlsx`

| Requirement ID | Scenario ID | Test Case ID | Status |
|----------------|-------------|--------------|--------|
| REQ001         | TS001       | TC001        | Pass   |
| REQ002         | TS002       | TC002        | Fail   |

### ✅ 8. Final Summary Report
- Total Test Cases: 20
- Passed: 18
- Failed: 2
- Bug Reports Raised: 3
- Blockers: None
- Status: Testing Complete

### ✅ 9. README.md
📁 `7_README/README.md`

## Tools Used
- Excel
- MS Word
- Browser DevTools
