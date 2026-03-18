# Aplair Project 🚀

High-performance, cinematic real estate video editing platform.

## 🏗️ Project Structure

The project is organized into a clean, modular architecture:

- **Root Directory**:
    - `index.html`: Main landing page with all interactive components (Booking Modal, Pricing, FAQ, etc.).
    - `refund-policy.html`: Optimized legal page for refund information.
    - `terms-of-service.html`: Optimized legal page for terms and conditions.
    - `sw.js`: Service Worker for PWA features and Advanced Caching (v2.2).
    - `sitemap.xml` & `robots.txt`: SEO configurations.
    - `favicon.png`: Brand identity asset.

- **Assets Folder (`/assets/`)**:
    - `css/`: 
        - `style.css`: Master stylesheet with variables and all component styles.
        - `style.min.css`: Minified production version (v2.2).
    - `js/`:
        - `script.js`: Core application logic (Form handling, Google Sheets integration, UI interactions).
        - `script.min.js`: Optimized production version (v2.2).
    - `images/`: High-quality brand logos and UI assets.

## ⚡ Performance Optimizations

We have implemented several professional-grade optimizations to ensure a 99+ score on Google PageSpeed:

1.  **Zero Layout Shift (CLS Fixes)**:
    - **Header Inline Script**: Determines user language/direction *before* body rendering to prevent "jumping" from LTR to RTL.
    - **Stable Dimensions**: Hero buttons and critical elements have fixed `min-width` and `min-height` to reserve space during loading.
2.  **Advanced Caching (Service Worker)**:
    - Implemented a `sw.js` with a **Cache-First** strategy.
    - Assets are stored locally in the browser, bypassing server TTL limits and providing instant secondary loads.
3.  **Core Web Vitals & Fonts**:
    - **Preconnect**: Established early connections to Google Fonts and external SVG sources.
    - **Font Preloading**: Critical font weights are preloaded to eliminate FOUT (Flash of Unstyled Text).
    - **Minification**: All CSS/JS are delivered in minified formats with cache-busting versioning (`v=2.2`).

## 🌍 Internationalization (i18n)

- **Unified Logic**: Both main and legal pages share the same language persistence system via `localStorage`.
- **Dynamic Content**: Text is swapped using `data-en`/`data-ar` attributes for standard elements and `data-lang-content` for large blocks.

## 🛠️ Maintenance & Deployment

- **Version Control**: When updating CSS or JS, increment the `?v=X.X` query string in all HTML files and `sw.js` to clear browser caches.
- **Minification**: Use a build script or manual compressor to keep `.min` files in sync with source code.
- **Hosting**: Optimized for GitHub Pages or any static CDN.

---
*Maintained by the Aplair Team | © 2026*
