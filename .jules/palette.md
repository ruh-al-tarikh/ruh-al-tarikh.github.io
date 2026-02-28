## 2026-05-18 - [Accessibility & Semantic Navigation Upgrade]
**Learning:** Standardizing navigation to use semantic `<ul>`/`<li>` and `aria-current="page"` significantly improves accessibility and provides a better experience for screen reader users. Adding a "Skip to main content" link is a critical micro-UX improvement for keyboard navigation.
**Action:** Always ensure navigation is wrapped in semantic list tags and include a skip link that targets the main content area (using `id="main"`).

## 2026-05-19 - [Visual Consistency and Focus States]
**Learning:** Maintaining consistent structural patterns (like wrapping content in `<section>` and standardizing footer text) across all pages creates a more professional and predictable user experience. Implementing `:focus-visible` styles ensures that accessibility improvements are only visible to keyboard users, keeping the UI clean for mouse users while supporting those who need it.
**Action:** Standardize common components (footer, header) and use `:focus-visible` for high-contrast focus indicators site-wide.

## 2026-05-20 - [Mobile Navigation & Asset Path Fixes]
**Learning:** Using `display: block` for navigation links in a vertical (mobile) layout causes the `aria-current="page"` indicator (bottom border) to span the full width, which can be visually confusing. Switching to `display: inline-block` ensures the indicator remains proportional to the text. Additionally, using absolute paths for assets (like `/assets/css/style.css`) in subpages breaks when the site is not served from the root domain; relative paths (e.g., `../assets/css/style.css`) are more robust.
**Action:** Use `display: inline-block` for vertical navigation links to keep indicators appropriately sized, and always use relative paths for internal assets to ensure cross-environment compatibility.
