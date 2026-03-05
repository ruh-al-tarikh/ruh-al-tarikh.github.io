## 2026-05-18 - [Accessibility & Semantic Navigation Upgrade]
**Learning:** Standardizing navigation to use semantic `<ul>`/`<li>` and `aria-current="page"` significantly improves accessibility and provides a better experience for screen reader users. Adding a "Skip to main content" link is a critical micro-UX improvement for keyboard navigation.
**Action:** Always ensure navigation is wrapped in semantic list tags and include a skip link that targets the main content area (using `id="main"`).

## 2026-05-19 - [Visual Consistency and Focus States]
**Learning:** Maintaining consistent structural patterns (like wrapping content in `<section>` and standardizing footer text) across all pages creates a more professional and predictable user experience. Implementing `:focus-visible` styles ensures that accessibility improvements are only visible to keyboard users, keeping the UI clean for mouse users while supporting those who need it.
**Action:** Standardize common components (footer, header) and use `:focus-visible` for high-contrast focus indicators site-wide.

## 2026-05-20 - [Standard Site-wide UX Enhancements]
**Learning:** Implementing `scroll-behavior: smooth` (respecting `prefers-reduced-motion`) and a custom `::selection` color are low-effort, high-impact micro-UX improvements that provide a polished, branded feel. For mobile navigation, using `inline-block` with generous padding for links ensures that active indicators (like `border-bottom`) are correctly sized to the text while maintaining large, accessible touch targets.
**Action:** Always include smooth scrolling and branded selection colors in new projects. For mobile menus, prioritize touch target size and visual correctness of active states.
