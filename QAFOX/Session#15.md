# 🧪 Registration Page Test Cases – QAFOX Live Project (Session 14)

This document contains test cases for validating the Registration Page of the eCommerce application, as demonstrated in QAFOX's live project training series.

---

## ✅ Mandatory Field Validations

### 🔹 TC_001: All Mandatory Fields Validation
- **Test Steps**:
  1. Keep all fields empty (First Name, Last Name, Email, Telephone, Password, Confirm Password).
  2. Click on **Continue**.
- **Expected Result**:
  - Error messages should appear for all mandatory fields.

---

### 🔹 TC_002: First Name Field - Only Spaces
- **Test Steps**:
  1. Enter only spaces in the First Name field.
  2. Click on **Continue**.
- **Expected Result**:
  - Error: _"First Name must be between 1 and 32 characters!"_

---

### 🔹 TC_003: First Name - Length Boundary Check
- **Test Steps**:
  1. Enter 1 character in First Name.
  2. Click **Continue**.
- **Expected Result**:
  - Success (if the character is valid).
  <br>
  <br>
  1. Enter 33 characters in First Name.
  2. Click **Continue**.
- **Expected Result**:
  - Error: _"First Name must be between 1 and 32 characters!"_

---

### 🔹 TC_004: Telephone Field - Invalid Format
- **Test Steps**:
  1. Enter special characters or alphabets in Telephone field (e.g., "abc@123").
  2. Click **Continue**.
- **Expected Result**:
  - Error: _"Telephone must be between 3 and 32 characters!"_ (based on business rules)

---

### 🔹 TC_005: Email Field - Invalid Format
- **Test Steps**:
  1. Enter malformed emails (e.g., "user@", "user.com", "@domain.com").
  2. Click **Continue**.
- **Expected Result**:
  - Proper email validation should trigger an error like: _"E-Mail Address does not appear to be valid!"_

---

### 🔹 TC_006: Password - Less than 4 Characters
- **Test Steps**:
  1. Enter "123" in Password and Confirm Password.
  2. Click **Continue**.
- **Expected Result**:
  - Error: _"Password must be between 4 and 20 characters!"_

---

## ✅ Duplicate Email Validation

### 🔹 TC_007: Registering with Existing Email
- **Test Steps**:
  1. Use an email address that is already registered.
  2. Fill other fields correctly.
  3. Click **Continue**.
- **Expected Result**:
  - Error: _"Warning: E-Mail Address is already registered!"_

---

## ✅ Password Confirmation Validation

### 🔹 TC_008: Password and Confirm Password Mismatch
- **Test Steps**:
  1. Enter "Password123!" in Password.
  2. Enter "Password321!" in Confirm Password.
  3. Click **Continue**.
- **Expected Result**:
  - Error: _"Password confirmation does not match password!"_

---

## ✅ Field UI, Formatting & Trimming

### 🔹 TC_009: Password Complexity Requirements
- **Test Steps**:
  1. Enter "12345" in Password and Confirm Password.
  2. Click **Continue**.
- **Expected Result**:
  - Error: Password should contain:
    - At least 8 characters
    - 1 uppercase letter
    - 1 lowercase letter
    - 1 number
    - 1 special character

---

### 🔹 TC_010: UI Alignment and Properties Check
- **Test Steps**:
  1. Check width, height, font, and consistency of all input fields.
  2. Check alignment as per client design spec.
- **Expected Result**:
  - All fields should adhere to the design requirements.

---

### 🔹 TC_011: Trimming Leading & Trailing Spaces
- **Test Steps**:
  1. Enter valid data with leading/trailing spaces (e.g., "  John  ") in all fields.
  2. Click **Continue**.
- **Expected Result**:
  - Application should trim spaces before saving or processing.

---

## ✅ Optional Test Case: Database Validation (For Advanced)

### 🔹 TC_012: Verify Data Stored in DB
- **Test Steps**:
  1. Register a user with valid data.
  2. Query the DB for the newly registered email/user.
- **Expected Result**:
  - Data should be saved correctly in all required columns.

---

## 📝 Notes:
- Email validations include checking valid format, uniqueness, and proper error messaging.
- All test cases are applicable for both manual and automated testing.
- UI validations are subject to change based on client-provided design specs.

---
# 🧪 Test Case Document – Registration Page

## 📄 Module: Registration Page  
**Project**: E-Commerce Web Application  
**Prepared From**: QAFOX Live Project – Session 14  
**Prepared By**: QA Learner  
**Date**: 2025-05-16  

---

## ✅ Test Cases

| TC ID     | Title                                            | Precondition                     | Test Steps                                                                                                                                 | Test Data                          | Expected Result                                                                 |
|-----------|--------------------------------------------------|----------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------|----------------------------------------------------------------------------------|
| TC_001    | Validate all mandatory fields                    | Registration page is open        | 1. Leave all fields empty<br>2. Click on "Continue"                                                                                         | N/A                                | Error messages for all mandatory fields should display                          |
| TC_002    | First Name with only spaces                      | Registration page is open        | 1. Enter only spaces in First Name<br>2. Click on "Continue"                                                                               | "     "                            | Error: "First Name must be between 1 and 32 characters!"                        |
| TC_003A   | First Name minimum length                        | Registration page is open        | 1. Enter 1 character in First Name<br>2. Click on "Continue"                                                                               | "J"                                | First Name should be accepted                                                   |
| TC_003B   | First Name exceeding max length                  | Registration page is open        | 1. Enter 33 characters in First Name<br>2. Click on "Continue"                                                                             | "A...A" (33 chars)                 | Error: "First Name must be between 1 and 32 characters!"                        |
| TC_004    | Telephone with invalid characters                | Registration page is open        | 1. Enter "abc@123" in Telephone<br>2. Click on "Continue"                                                                                   | "abc@123"                          | Error: "Telephone must be between 3 and 32 characters!"                         |
| TC_005    | Invalid email format                             | Registration page is open        | 1. Enter malformed emails like "user@", "user.com"<br>2. Click on "Continue"                                                               | Various invalid emails             | Error: "E-Mail Address does not appear to be valid!"                            |
| TC_006    | Password less than 4 characters                  | Registration page is open        | 1. Enter "123" as Password and Confirm Password<br>2. Click on "Continue"                                                                  | "123"                              | Error: "Password must be between 4 and 20 characters!"                          |
| TC_007    | Duplicate email registration                     | Registration page is open        | 1. Enter a valid but already registered email<br>2. Fill all fields<br>3. Click "Continue"                                                 | Existing email                     | Error: "Warning: E-Mail Address is already registered!"                         |
| TC_008    | Password and confirm password mismatch           | Registration page is open        | 1. Enter "Password123" in Password<br>2. Enter "Password321" in Confirm Password<br>3. Click "Continue"                                   | Password: Password123<br>Confirm: Password321 | Error: "Password confirmation does not match password!"         |
| TC_009    | Password does not meet complexity requirements   | Registration page is open        | 1. Enter "12345" in Password and Confirm Password<br>2. Click on "Continue"                                                                | "12345"                            | Error: Should enforce password complexity (e.g. upper/lower/special/length)     |
| TC_010    | UI field alignment and consistency               | Registration page is open        | 1. Observe all input fields<br>2. Verify font, size, spacing, alignment                                                                    | N/A                                | All input fields should be consistent and match design specs                    |
| TC_011    | Trim leading/trailing spaces                     | Registration page is open        | 1. Enter spaces before/after text in all fields<br>2. Click "Continue"                                                                     | "  John  ", "  user@mail.com  "    | Spaces should be trimmed before processing                                      |
| TC_012    | Database validation for newly registered user    | DB access enabled                | 1. Register a new user<br>2. Query DB with email<br>3. Verify field values                                                                 | Valid user info                    | All values should be stored correctly in DB                                     |

---

## 🗂️ Notes:
- Mandatory fields include: First Name, Last Name, Email, Telephone, Password, Confirm Password.
- UI checks depend on the client’s design documents.
- Some validations (e.g., DB) may require backend access and are suitable for integration testing.


