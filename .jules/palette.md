## 2026-05-18 - [Accessibility & Semantic Navigation Upgrade]
**Learning:** Standardizing navigation to use semantic `<ul>`/`<li>` and `aria-current="page"` significantly improves accessibility and provides a better experience for screen reader users. Adding a "Skip to main content" link is a critical micro-UX improvement for keyboard navigation.
**Action:** Always ensure navigation is wrapped in semantic list tags and include a skip link that targets the main content area (using `id="main"`).

## 2026-05-19 - [Visual Consistency and Focus States]
**Learning:** Maintaining consistent structural patterns (like wrapping content in `<section>` and standardizing footer text) across all pages creates a more professional and predictable user experience. Implementing `:focus-visible` styles ensures that accessibility improvements are only visible to keyboard users, keeping the UI clean for mouse users while supporting those who need it.
**Action:** Standardize common components (footer, header) and use `:focus-visible` for high-contrast focus indicators site-wide.

## 2026-05-20 - [Mobile Navigation Touch Targets]
**Learning:** For vertical mobile navigation, using `display: block` on anchor tags is superior to `display: inline-block` because it ensures the entire width of the navigation container is clickable. While `inline-block` might look better for centered text with underlines/borders, it significantly reduces the hit area (WCAG 2.5.5), leading to a poorer user experience.
**Action:** Prioritize `display: block` with generous padding (e.g., `0.6rem 1rem`) for mobile navigation links to maximize accessibility and ease of use.
