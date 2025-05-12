# 🛒 E-Commerce Domain Notes for Testing & Interview Preparation

## 🔍 What is E-Commerce?
E-Commerce (Electronic Commerce) refers to the buying and selling of goods or services using the internet, including the transfer of money and data to execute these transactions.

---

## 🧩 Types of E-Commerce Business Models

| Model | Description | Example |
|-------|-------------|---------|
| **B2B** (Business to Business) | Transactions between businesses | Alibaba, IndiaMART |
| **B2C** (Business to Consumer) | Business sells directly to consumers | Amazon, Flipkart |
| **C2C** (Consumer to Consumer) | Individuals sell to other individuals | OLX, eBay |
| **C2B** (Consumer to Business) | Individuals offer products or services to businesses | Freelance platforms like Fiverr |

---

## 📱 Types of E-Commerce Applications

| Application Type | Description |
|------------------|-------------|
| **Web Application** | Browser-based interface (e.g., Amazon.com) |
| **Mobile Application** | Android/iOS apps (e.g., Amazon app, Myntra app) |
| **Hybrid Application** | Cross-platform apps serving both web and mobile users |
| **Single Vendor Marketplace** | A platform owned by a single seller (e.g., Dell.com) |
| **Multi-Vendor Marketplace** | A platform where multiple vendors sell (e.g., Amazon, Flipkart) |

---

## 🧾 Product-Related Terminology

| Term | Description |
|------|-------------|
| **Product Code / SKU** | Unique identifier for each product |
| **Product Description** | Details like features, specifications, and usage |
| **Product Categories** | Groupings such as Electronics, Fashion, Groceries, Books |
| **Product Images** | Visual galleries showing different angles of the product |
| **Price & Discounts** | Pricing details including original price, offer price, and coupon discounts |
| **Stock Status** | Availability status: In Stock / Out of Stock |
| **Variants** | Different colors, sizes, or models of the same product |

---

## 🧠 E-Commerce Features (Functionalities to Test)

| Feature | Description |
|---------|-------------|
| **Search & Filters** | Ability to search products and filter by brand, price, etc. |
| **Product Page** | Displays details, reviews, ratings, and images of a product |
| **Shopping Cart** | Allows adding, editing, or removing items with automatic price updates |
| **Wishlist** | Saves items for future purchase |
| **Checkout** | Involves entering address, selecting delivery options, and payment process |
| **Payment Gateways** | Integration with Credit/Debit cards, UPI, wallets, EMI, etc. |
| **Order Confirmation** | Generates an order ID and confirmation screen |
| **Order History** | Displays past orders and their current status |
| **Return/Refund** | Process to initiate returns, upload necessary proofs, and process refunds |
| **Tracking** | Real-time shipment tracking system |

---

## 💼 E-Commerce Roles (from a Testing Perspective)

| Role | Responsibility |
|------|----------------|
| **Admin** | Manages product listings, seller accounts, and overall backend operations |
| **Seller** | Uploads and manages their own product listings |
| **Customer** | Browses, purchases, and returns products |
| **Delivery Partner** | Manages logistics and shipping of orders |

---

## 🌐 Third-Party Integrations in E-Commerce

- **Payment Gateways**: Razorpay, Paytm, Stripe, etc.
- **Logistics APIs**: Delhivery, ShipRocket, etc.
- **Notification Services**: Twilio (SMS), SendGrid (Email)
- **Customer Support Chat**: Freshdesk, Intercom

---

## 📦 Order Life Cycle

1. **Product Added to Cart**
2. **Checkout & Payment**
3. **Order Confirmation**
4. **Processing & Packaging**
5. **Dispatch via Delivery Partner**
6. **Out for Delivery**
7. **Delivered or Returned**

---

## 🧪 Sample Test Scenarios (Functional Testing)

| Scenario | Test Case Example |
|----------|-------------------|
| **Add to Cart** | Verify that the product quantity updates correctly and the total price recalculates |
| **Product Availability** | Ensure that "Out of Stock" is shown when no inventory is available |
| **Coupon Application** | Check that applying a coupon provides the correct discount |
| **Order Cancellation** | Validate the cancellation process and subsequent refund |
| **Filtering Products** | Ensure filters return only relevant products by brand, price range, etc. |
| **Payment Failure** | Verify that a proper error message appears and users can retry payments |

---

## 📈 Key Metrics to Monitor (For QA & Product Teams)

- **Cart Abandonment Rate**
- **Conversion Rate**
- **Average Order Value (AOV)**
- **Product Return Rate**
- **Page Load Time** (especially on product and search pages)

---

## 🛠️ Non-Functional Testing Areas

| Testing Type         | Focus Area |
|----------------------|------------|
| **Performance Testing** | Assess site scalability (e.g., can it handle 10k+ users during sales?) |
| **Security Testing**    | Ensure secure transactions, data encryption, and safe user data handling |
| **Usability Testing**   | Evaluate UI/UX for intuitiveness across different age groups and demographics |
| **Compatibility Testing** | Test the application across various browsers, devices, and operating systems |

---

## 🔁 Real-Time Examples

- **Amazon**: Exemplifies a multi-vendor B2C model with high scalability and robust features.
- **Myntra**: Known for fashion-focused, mobile-first e-commerce.
- **OLX**: Demonstrates a C2C marketplace for second-hand products.
- **Meesho**: Follows a C2B2C reseller model.
- **MakeMyTrip**: Represents B2C travel e-commerce covering flights, hotels, etc.

---
