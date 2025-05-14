# 🧪 [Session 13: Writing Test Scenarios, Test Cases & Test Data for E-Commerce App](https://www.youtube.com/watch?v=Z5-c0Wh2ZKM&list=PLsjUcU8CQXGGguAbeip-Q_ZckElVGUwxQ&index=13)

## ✅ What is a Test Scenario?

> A **test scenario** is a high-level documentation of what to test — it defines **what functionality** or **feature** needs to be verified.

- Also called **Test Condition**
- Example:
  - "Verify user can log in with valid credentials"
  - "Verify user can add product to cart"
 
# 🧪 Test Scenario Document

## 📘 Module: Shopping Cart

| Scenario ID | Test Scenario Description                          | Priority | Test Type      | Preconditions                        | Expected Result                             |
|-------------|----------------------------------------------------|----------|----------------|---------------------------------------|----------------------------------------------|
| TC_SC_001   | Verify adding a single item to the shopping cart   | High     | Functional     | User is logged in                     | Item should be added and displayed in cart   |
| TC_SC_002   | Verify removing an item from the shopping cart     | Medium   | Functional     | Item already added to cart            | Item should be removed from the cart         |
| TC_SC_003   | Verify updating quantity in the cart               | High     | Functional     | Item added to cart                    | Quantity should be updated successfully      |
| TC_SC_004   | Verify cart persists after user logs out and in    | Low      | Usability      | Item in cart before logging out       | Cart should retain items after login         |
| TC_SC_005   | Verify empty cart message is shown appropriately   | Medium   | UI/Functional  | No item in cart                       | "Your cart is empty" message should display  |

---

## 📘 Module: Checkout Process

| Scenario ID | Test Scenario Description                          | Priority | Test Type      | Preconditions                        | Expected Result                             |
|-------------|----------------------------------------------------|----------|----------------|---------------------------------------|----------------------------------------------|
| TC_CO_001   | Verify user is able to proceed to checkout         | High     | Functional     | At least one item in cart             | User is redirected to checkout page          |
| TC_CO_002   | Verify checkout fails with invalid card details    | High     | Negative       | User on payment screen                | Error message should be displayed            |
| TC_CO_003   | Verify successful checkout with valid details      | High     | Functional     | All valid data entered                | Order confirmation page should display       |
| TC_CO_004   | Verify order summary before payment                | Medium   | UI             | Items present in checkout             | Summary should list item, quantity, and cost |

---

> 🧾 **Note**: Test scenarios are high-level and focus on *what to test*. Detailed **test cases** will follow these scenarios and define *how to test*.


## ✅ What is a Test Case?

> A **test case** is a detailed document that describes **how** to test a particular scenario with **step-by-step actions**, **test data**, and **expected results**.

| Field             | Description |
|------------------|-------------|
| Test Case ID     | Unique identifier (e.g., TC_Login_001) |
| Test Scenario    | Linked high-level test scenario |
| Test Steps       | Actions to perform |
| Test Data        | Data used for testing |
| Expected Result  | What should happen |
| Actual Result    | What happened during testing |
| Status           | Pass / Fail |
| Comments         | Notes, defects, observations |

---

## 🛍️ E-Commerce Use Case for Practice

### 🔍 Scenario: User Registration on E-Commerce Site

#### 🎯 Test Scenarios:
1. Verify user can register with valid details.
2. Verify error message for duplicate email.
3. Verify mandatory field validations.

#### 🧾 Test Case: Registration with Valid Details

| Field           | Value |
|----------------|-------|
| Test Case ID   | TC_REG_001 |
| Test Scenario  | Verify user can register with valid details |
| Test Steps     | 1. Open Registration page <br> 2. Fill Name, Email, Password <br> 3. Click 'Register' |
| Test Data      | Name: John <br> Email: john@email.com <br> Password: 123456 |
| Expected Result| User is redirected to the homepage with a success message |
| Actual Result  | As expected |
| Status         | ✅ Pass |
| Comments       | - |

---

## 🛒 Real-Time Practice Topics (From Video)

### 🧪 Sample Test Scenarios Covered:

| Module               | Test Scenarios |
|----------------------|----------------|
| **Login**            | Valid login, invalid login, password masking, Forgot Password link |
| **Registration**     | Mandatory fields, valid data, duplicate email |
| **Search Product**   | Search by name, partial name, invalid term |
| **Product Details Page** | Verify image, title, price, Add to Cart button |
| **Cart**             | Add, remove, quantity update, price calculation |
| **Checkout**         | Shipping address, payment method, success message |

---

## 🛠️ Pro Tips:

- Use **Excel** or **Test Management Tools** (like TestRail, PractiTest) to maintain test cases.
- Always map **Test Cases** to **Requirements/User Stories**.
- Use a consistent naming convention for Test Case IDs.

### Excel : [Link](https://excel.cloud.microsoft/open/onedrive/?docId=FE91843380CEF79D%21s6bf102230bc14326965f1ce684538891&driveId=FE91843380CEF79D)
### GoogleSheet: [Link](https://docs.google.com/spreadsheets/d/1Q3Btcow5NZVd_WU5Nzdod1dwaT3Th51MuNKc6EVp0iM/edit?gid=0#gid=0)
### Template : [Link](https://drive.google.com/file/d/1c4hA9yyECvHqJnmtPRx0QfhnkjISzWXF/view)

