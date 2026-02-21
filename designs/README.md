# Ergonomic Lady Egg (Beauty Sponge) – High-Level Design Spec

---

## Suggested Color Palette & Style

| Token           | Hex      | Usage                              |
|-----------------|----------|-------------------------------------|
| Fancy Pink      | #FF91AF  | Brand/primary, accent, buttons      |
| Soft Peach      | #FFDFD3  | Secondary bg, highlights            |
| Lavender Dream  | #D6B4FC  | Alternate accent, variant options   |
| Clean White     | #FFFFFF  | Main background, containers         |
| Gentle Gray     | #F5F5F7  | Panels, input bg, border highlight  |
| Charcoal Black  | #29243A  | Title, strong text, nav, contrast   |
| Minty Green     | #ADEFC7  | Success/informational highlights    |

**Style:** Playful, soft curves, luxury-feel. Clean sans-serif fonts (Montserrat, Roboto, or similar). Illustrative icons for ergonomic features.

---

## Layout Description (Wireframes)

### 1. Home Page
```
-----------------------------
[Navbar] -- Logo | Shop | Bundles | About | Cart
-----------------------------
[Hero Section: Large image of Lady Egg in hand with long nails]
Headline: “Blend Beautifully, Protect Your Nails”
CTA: [Shop Lady Egg] [Learn More]
-----------------------------
[Product Highlights - 3 Columns]
- Nail Friendly Grip   - Ultra Soft Foam      - Stylish Stand
-----------------------------
[Collections Grid: Lady Egg Colors w/ quick add]
-----------------------------
[Testimonials Slider]
-----------------------------
[Footer]
-----------------------------
```

### 2. Product Detail Page – Lady Egg
```
-----------------------------
[Navbar]
-----------------------------
[Product Gallery | Product Info]
[ Main image (hand w/ long nails), alt angles, color selector  ][ Title, price, color, Nail Friendly badge ]
[ Add to Cart ] [Bundle with Accessories]
[ Description: Ergonomic Features | Material | Care ]
[ Tabs: Details | Reviews | Bundles ]
-----------------------------
[Suggested Products Grid]
-----------------------------
[Footer]
-----------------------------
```

### 3. Category Page – Beauty Tools
```
-----------------------------
[Navbar]
-----------------------------
[Filter Sidebar]
- Brand
- Material
- Ergonomic Features (Nail Friendly)
- Color
[List/Grid of Lady Eggs and other tools]
-----------------------------
[Footer]
-----------------------------
```

### 4. Admin Product Addition/Edit Page
```
-----------------------------
[Sidebar: Catalog | Orders | Users |]
-----------------------------
[Form:]
- Product Name
- Slug
- Type: Beauty Sponge
- Colors (multi)
- Image uploads
- Price
- Tags: Nail Friendly, Ergonomic, Vegan
- Description
- Bundles
- Stock management
- Save/Publish
-----------------------------
```

---

## UI Elements to Include
- Buttons: Primary (Fancy Pink), Secondary (Soft Peach), Icon (Lavender)
- Toggles/Switches: For filtering (Ergonomic/Nail Friendly)
- Badges: “Nail Friendly”, “Vegan”, “Eco”
- Color selectors: Palette swatches
- Product Carousel/Slider
- Tabs (Details/Reviews/Bundles)
- Input forms: Admin, Reviews
- Modal overlays for bundle selection
- Quick add to cart feature in collection grid
- Accessibility: High-contrast text, focus outlines, alt text

---

## Component Breakdown
- **Navbar:** Logo, shop links, cart (mobile & desktop)
- **Hero Section:** Large callout, lifestyle image, CTAs
- **Product Card:** Image, price, badges, color selector, quick add
- **Product Gallery:** Main & alternate views, zoom
- **Feature Grid:** Icons w/ short text for ergonomic features
- **Review/Slider:** Customer quotes with star rating
- **Admin UI:** Form fields, tag selectors, stock interface
- **Footer:** Links, contact, social media
- **Filter Sidebar:** Checkbox/toggle filters for ergonomic/nail friendly

---

## Mermaid Layout Diagram
```mermaid
graph TD
  Home --|Hero| HeroSection
  Home --|Highlights| ProductHighlights
  Home --|Collections| CollectionGrid
  Home --|Slider| Testimonials
  ProductPage --|Gallery| ProductGallery
  ProductPage --|Details| ProductInfoDetails
  ProductPage --|Tabs| ProductTabs
  Admin --|Form| AdminProductForm
  Admin --|Sidebar| AdminNav
```

---

## External Visuals
- [Figma Prototype Board (work-in-progress)](https://www.figma.com/file/0XYZabcd1234example)

---

## Supporting Design Tokens
- See `designs/colors.json` for palette in code form

---

### Ready for Product Manager review. For feedback, comment on this commit!
