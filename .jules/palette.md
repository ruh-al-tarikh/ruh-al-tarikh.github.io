## 2026-05-18 - [Accessibility & Semantic Navigation Upgrade]
**Learning:** Standardizing navigation to use semantic `<ul>`/`<li>` and `aria-current="page"` significantly improves accessibility and provides a better experience for screen reader users. Adding a "Skip to main content" link is a critical micro-UX improvement for keyboard navigation.
**Action:** Always ensure navigation is wrapped in semantic list tags and include a skip link that targets the main content area (using `id="main"`).

## 2026-05-20 - [Focus Visibility & Content Standardization]
**Learning:** Consistently applying `:focus-visible` with a high-contrast outline (`#1ee`) significantly improves accessibility for keyboard-only users without impacting the visual experience for mouse users. Standardizing structural elements like `<section>` and the footer text across all pages ensures a predictable and polished UX.
**Action:** Always include `:focus-visible` styles for interactive elements and verify structural consistency across all pages to maintain a professional look and feel.
