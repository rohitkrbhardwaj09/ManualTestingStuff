## 🛒 Shopping Cart & Gift Certificate Flow in E-Commerce Website (Tutorials Ninja)

### 🎁 Gift Certificate Functionality

* After adding a product to the cart and applying shipping, you can also apply a **gift certificate**.
* **Gift Certificate Scenario**:

  * Your friend gifts you a \$100 gift card on your birthday.
  * This gift card is from the same application (Tutorials Ninja) and includes a code like `ABC1XZ`.
  * You enter this code in the "Gift Certificate" field and click "Apply Gift Certificate".
  * \$100 will be deducted from the total amount.
  * For example, if the total amount is \$145, after applying the \$100 gift certificate, you only need to pay \$45.

### 🔍 Additional Notes

* Gift cards can be purchased by anyone and gifted to others.
* These are commonly used in platforms like Amazon, Flipkart, etc.
* During testing, if the system doesn't provide test data (gift card codes), raise a **query to the client**:

  * *"Can you share some gift card codes for testing purposes?"*

---

## 🔁 Continue Shopping vs Checkout

### 🛍 Continue Shopping

* Used when user wants to add more products before purchasing.
* Takes the user back to **homepage**.

### ⚠️ Defects Identified

* Canon product page:

  * Mandatory dropdown options not displaying. **(UI Bug)**
  * Defect Note: *"Options not getting displayed in the mandatory dropdown for Canon camera."*
* Shipping Rate Issue:

  * After applying the flat shipping rate, if user clicks "Continue Shopping" and returns, the rate is **lost**.
  * Query to Client:

    * *"After applying flat shipping rate, it is getting lost when navigating back. Is this expected behavior?"*

---

## 🔄 Navigating to Checkout Page

### ✅ Methods to Navigate

1. **Checkout button** on shopping cart page.
2. **Checkout option** from header.
3. From **shopping cart total dropdown**, then clicking "Checkout".

---

## 🔐 Checkout Page (Signed-in Checkout)

### 📋 Type of Checkout

* **Signed-in Checkout**: Logged-in user adds items and proceeds to checkout.

### 🧾 Billing Details Section

* Fields to fill:

  * Address, Country, State, etc.
  * Click **Continue** to proceed.

### 🚚 Delivery Details Section

* Two options:

  1. **Same as Billing Address**
  2. **Different Address** (e.g., gifting to someone at a different location)
* **Test Scenarios**:

  * Test both "Same" and "Different" address options.

### 📦 Delivery Method Section

* Only one option: **Flat Shipping Rate**
* Real-time applications may have multiple delivery types (e.g., one-day, standard, etc.)
* **Additional Comments Field**:

  * Provide delivery instructions.
  * Example: *"My house is beside the petrol pump and HDFC Bank."*

### 📝 Summary of Delivery Method Section

* **Shipping Type**: Flat Shipping
* **Comments**: Additional instructions for delivery person

> 🔍 Note: Some features may not be present due to application limitations. Focus only on available functionalities.

---

✅ Continue exploring remaining checkout steps (payment, order confirmation, etc.) in the next section.

---

📌 **Tip for QA Testers**:

* Use collapsible sections in test documentation.
* Track defects and client queries during exploratory testing.
* Maintain checklist of testable UI paths (e.g., buttons, dropdowns, breadcrumbs).

