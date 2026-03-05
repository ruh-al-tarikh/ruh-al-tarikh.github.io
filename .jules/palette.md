## 2026-05-18 - [Accessibility & Semantic Navigation Upgrade]
**Learning:** Standardizing navigation to use semantic `<ul>`/`<li>` and `aria-current="page"` significantly improves accessibility and provides a better experience for screen reader users. Adding a "Skip to main content" link is a critical micro-UX improvement for keyboard navigation.
**Action:** Always ensure navigation is wrapped in semantic list tags and include a skip link that targets the main content area (using `id="main"`).

## 2026-05-19 - [Visual Consistency and Focus States]
**Learning:** Maintaining consistent structural patterns (like wrapping content in `<section>` and standardizing footer text) across all pages creates a more professional and predictable user experience. Implementing `:focus-visible` styles ensures that accessibility improvements are only visible to keyboard users, keeping the UI clean for mouse users while supporting those who need it.
**Action:** Standardize common components (footer, header) and use `:focus-visible` for high-contrast focus indicators site-wide.

## 2026-05-20 - [Mobile Navigation Touch Targets]
**Learning:** For vertical mobile navigation, using `display: block` on anchor tags is superior to `display: inline-block` because it ensures the entire width of the navigation container is clickable. While `inline-block` might look better for centered text with underlines/borders, it significantly reduces the hit area (WCAG 2.5.5), leading to a poorer user experience.
**Action:** Prioritize `display: block` with generous padding (e.g., `0.6rem 1rem`) for mobile navigation links to maximize accessibility and ease of use.

## 2026-05-21 - [Brand-Aligned Selection and Smooth Motion]
**Learning:** Micro-interactions like a custom `::selection` color that matches the brand identity (e.g., using #1ee Cyan) provide a subtle touch of delight that makes the site feel more cohesive. Additionally, implementing `scroll-behavior: smooth` (while respecting `prefers-reduced-motion`) significantly improves the perceived quality of navigation, especially when jumping to internal anchors like the "Skip to main content" link.
**Action:** Always wrap `scroll-behavior: smooth` in a `prefers-reduced-motion: no-preference` media query and use brand-aligned colors for selection styles to enhance site personality.

## 2026-05-22 - [Standardized Accessibility and Metadata Polish]
**Learning:** Small polishes like adding `aria-label` to navigation landmarks, consistent page titles, and setting a `theme-color` meta tag for mobile browsers collectively elevate the site's perceived quality and accessibility. Improving color contrast for secondary text (like the footer) from #888 to #aaa ensures WCAG AA compliance and better readability on dark backgrounds.
**Action:** Include a "polish pass" for every feature, ensuring landmark labels are present, metadata is optimized for mobile, and color contrast meets accessibility standards.
