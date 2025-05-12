# 🛍️ E-Commerce Domain Knowledge - Product Comparison & Display Page

## 🔍 Product Comparison Functionality

### ✅ Available Comparison Criteria:
- Price-wise
- Model-wise
- Ratings-wise
- Description-wise
- Weight-wise
- Dimensions-wise
- Clock Speed-wise

---

## 🚀 Navigating to Product Comparison Page

### 🛣️ Ways to Navigate:
1. **From Search Results**  
   - Add products to comparison → Click "Product Comparison" link.
2. **From Success Message**  
   - After adding product, click on the success toast message.
3. **From Category Page**  
   - Available in both **List View** and **Grid View**.
4. **From Product Display Page**
5. **From List/Grid Views in Subcategory Pages**

---

## ➕ Places Where "Compare This Product" Option is Available:

| Page Type                      | View Type      | Compare Option Available |
|-------------------------------|----------------|---------------------------|
| Product Display Page          | -              | ✅                        |
| Search Results Page           | List & Grid    | ✅                        |
| Category Page (e.g. Mac)      | List & Grid    | ✅                        |
| Subcategory Page (e.g. iMac)  | List & Grid    | ✅                        |

---

## 🧠 Tool Used for Mapping: Mind Map X Mind Tool

### 🧭 Basic Shortcuts:
- `Tab` → Create a **Child Node**
- `Enter` → Create a **Sibling Node**
- Easy drag-and-drop reordering of nodes

---

## 📦 Product Display Page Overview

### 🖼️ Sections Present:
1. **Product Thumbnails**
   - Multiple thumbnails
   - Opens in **Lightbox** with navigation
2. **Main Displayed Image**
   - Highlighted thumbnail image
3. **Product Name**
   - E.g., iMac
4. **Brand**
   - E.g., Apple
5. **Product Code**
   - Unique identifier for each product
6. **Availability Status**
   - Statuses can be:
     - ✅ `In Stock`
     - ❌ `Out of Stock`
     - ⚠️ _Potential_ → `Limited Stock` (To be confirmed with client)

---

## 🧪 Additional Test Scenarios

- Check lightbox scrolling for thumbnails
- Confirm correct image displayed when thumbnail is clicked
- Ensure product availability statuses behave correctly
  - Edge case: Add “Limited Stock” if applicable

---

> 📌 **Note:** Documenting UI sections and comparison options helps in better test case planning and identifying feature coverage during QA processes.

