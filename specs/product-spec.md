# Product Specification Update: Addition of "Ladies Soaps" Category

**Repository:** [false-eyelash-store](https://github.com/misterfitzy/false-eyelash-store)  
**Specification File:** `specs/product-spec.md`  
**Date:** 2026-02-21  
**Author:** Product Manager (AI)

---

## Overview

This document outlines the update to expand the **false-eyelash-store** e-commerce platform by adding "Ladies Soaps" as a dedicated product category. The goal is to extend the store’s catalog, offering shoppers high-quality soaps targeted at women, and to ensure a best-in-class browsing and purchasing experience. This update builds upon the store’s flexible catalog structure and admin features established for categories like False Eyelashes, False Nails, Hair Dye, Stockings, Lipstick, High Rise Jeans, Accessories, and Ladies Footballs.

---

## 1. Goals

- Expand the online catalog to include "Ladies Soaps" as a core, filterable category.
- Empower users to discover, filter, and shop for soaps according to brand, scent, ingredients, and skin type.
- Enable full admin management and reportability for soaps, ensuring efficient inventory, product information, and order handling.
- Maintain modern e-commerce UX, accessibility, and mobile responsiveness.

---

## 2. Catalog & Navigation Structure

**Add "Ladies Soaps" as a top-level category alongside:**
- False Eyelashes
- False Nails
- Sheer Stockings
- Lipstick
- Hair Dye
- High Rise Jeans
- Ladies Footballs
- Accessories

### ![Mermaid Diagram: Updated Catalog Structure](#)
```mermaid
graph TD
  Catalog --> "False Eyelashes"
  Catalog --> "False Nails"
  Catalog --> "Sheer Stockings"
  Catalog --> "Lipstick"
  Catalog --> "Hair Dye"
  Catalog --> "High Rise Jeans"
  Catalog --> "Ladies Footballs"
  Catalog --> "Accessories"
  Catalog --> "Ladies Soaps"
```

### Navigation

- Primary navigation includes "Ladies Soaps."
- Homepage features soap promotions as banners/tiles.
- Category page supports browsing, filtering, search, and direct product links.

---

## 3. Filters & Product Attributes for Ladies Soaps

- **Brand** (e.g., Dove, Nivea, Body Shop, Custom)
- **Scent/Fragrance** (e.g., Lavender, Rose, Citrus, Unscented)
- **Type** (Bar, Liquid, Exfoliating, Moisturizing, Antibacterial)
- **Skin Type** (Normal, Dry, Oily, Sensitive, Combination)
- **Key Ingredients** (Shea Butter, Aloe, Charcoal, Glycerin, Essential oils, etc.)
- **Vegan/Cruelty-free** (Yes/No)
- **Hypoallergenic** (Yes/No)
- **Size/Volume** (e.g., 50g, 100g, 250ml)
- **Rating**
- **Price Range**
- **In Stock Only**

#### Example: Soap Product Data Model (JSON)
```json
{
  "id": "soap-rosemoist-100g",
  "category": "Ladies Soaps",
  "brand": "RoseMoist",
  "name": "Rose Moisturizing Bar",
  "scent": "Rose",
  "type": "Bar",
  "skin_type": ["Dry", "Normal"],
  "ingredients": ["Rose Extract", "Shea Butter"],
  "vegan": true,
  "cruelty_free": true,
  "hypoallergenic": false,
  "size": "100g",
  "price": 3.99,
  "rating": 4.7,
  "in_stock": true,
  "images": ["/images/soaps/rosemoist-100g-front.jpg"]
}
```

---

## 4. Admin & Management

- **CRUD** for soap products (add/edit/delete/clone).
- Batch import/export (CSV/Excel/JSON).
- Bulk update for attributes (e.g., price, stock, tags).
- Inventory & reorder alerts based on stock thresholds.
- Reporting on sales, inventory, popularity (by brand, scent, etc.).
- Image/media management for high-quality product displays.
- Full support in admin dashboard reporting and product lifecycle management.

---

## 5. User Stories

### Shopper

- As a shopper, I can browse and filter Ladies Soaps by brand, scent, skin type, and type to find suitable products.
- As a shopper, I can view soap details, ingredients, and recommendations for my skin type.
- As a shopper, I can add soaps to my cart and purchase alongside other beauty and fashion items.
- As a shopper, I can view reviews and ratings for soaps.
- As a shopper, I can search for specific soap brands or scents from the main search bar.

### Admin

- As an admin, I can add new soap SKUs with full attribute support.
- As an admin, I can manage stock and receive low inventory alerts for soaps.
- As an admin, I can generate sales and inventory reports filtered by soap category or attribute.
- As an admin, I can bulk update product info and assets easily.

---

## 6. Acceptance Criteria

- "Ladies Soaps" is visible as a category in main navigation, search, and home promotions.
- Users can browse, filter, and search within the soaps category using all supported filters.
- Product detail pages show all relevant soap attributes, images, price, and stock status.
- Soaps can be easily managed (CRUD, batch import/export, reporting) by admins in the dashboard UI.
- All flows are mobile responsive and accessible (e.g., WCAG AA level).
- Mixed-category carts and checkout are supported.
- All catalog, shopping, and admin flows involving soaps meet existing performance and security standards.

---

## 7. UI/UX Recommendations

- Filter panel for soap-specific attributes (scents as color chips, skin type as icons, etc.).
- High-resolution product photography with zoom and alternative views.
- Ingredient pop-overs on product cards.
- “Shop By Skin Type” and “Trending Scents” quick filters.
- Accessible UI components (ARIA, keyboard nav).
- Consistency with existing store UI for cross-category shopping.

---

## 8. Next Steps

1. **Review/approve** this specification.
2. Update wireframes/UI mockups to show soap category and new filter panel.
3. Begin implementation: product model update, catalog UI, admin dashboard.
4. Write and execute test cases (shopper & admin).
5. Curate & import initial soap SKUs/assets.

---

*Committed on: 2026-02-21  
For feedback, further breakdowns, or wireframe examples, please contact the Product Manager.*

---
