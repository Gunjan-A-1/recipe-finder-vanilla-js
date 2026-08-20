# 🍳 Recipe Finder — Culinary & Recipe Discovery App

An editorial-style, single-page recipe finder app built with pure **HTML5, CSS3, and Vanilla JavaScript** (Zero Frameworks/Libraries). Powered by [TheMealDB API](https://www.themealdb.com/api.php).

---

## ✨ Features

- **🔍 4-Stage Smart Search:**
  1. Live Title Search via TheMealDB API.
  2. Local Typo-Tolerant / Fuzzy Search (handles misspellings like *"chiken tika"*).
  3. Reverse Ingredient Lookup (if a user types an ingredient instead of a dish name).
  4. Web Fallback with 1-click Google, YouTube, and AllRecipes links.
- **🥕 "What's in my kitchen" (Ingredient Search):** Search using multiple ingredients (e.g., `chicken, garlic, tomato`). Finds the mathematical intersection (all ingredients) or ranks by highest match count.
- **⭐ Deterministic Recipe of the Day:** Picks the exact same recipe for all users across the globe each day using a deterministic date-hash algorithm (`djb2`), changing automatically at midnight.
- **⚖️ Interactive Servings Scaler:** Scale ingredients by **½×, 1×, 2×, or 3×**. Accurately computes mixed numbers, fractions (`1 1/2 cups`), ranges (`2-3 cloves`), and metric values.
- **🛒 Smart Shopping List:**
  - Add ingredients directly with current scaling factor applied.
  - Automatically merges duplicate ingredients case-insensitively without overwriting measurements.
  - Checklist state with strike-through and 1-click clipboard export.
- **❤️ Persistent Favorites:** Save favorite recipes locally with `localStorage`.
- **⚡ Offline-Indexed Catalog:** Background caches the database into `localStorage` on initial load for instant autocomplete suggestions without network latency.
- **🖨️ Clean Print Mode:** Custom print stylesheet to print clean recipe cards directly.
- **🎨 Editorial Aesthetic:** Warm cream/terracotta/olive palette with serif typography (*Playfair Display*) and pure SVG outline icons (no emojis, no external icon packs).

---

## 🛠️ Tech Stack

- **HTML5** — Semantic markup, accessibility features.
- **CSS3** — Custom design tokens, CSS Grid, Flexbox, smooth transitions, print stylesheet.
- **Vanilla JavaScript (ES6+)** — `fetch` with `async/await`, `localStorage`, Set/Map operations, Levenshtein distance algorithm, debouncing.
- **API** — [TheMealDB Free API](https://www.themealdb.com/api.php)

---

## 🚀 How to Run Locally

1. Clone this repository:
   ```bash
   git clone https://github.com/YOUR-USERNAME/recipe-finder-vanilla-js.git
