## 2026-05-18 - [Accessibility & Semantic Navigation Upgrade]
**Learning:** Standardizing navigation to use semantic `<ul>`/`<li>` and `aria-current="page"` significantly improves accessibility and provides a better experience for screen reader users. Adding a "Skip to main content" link is a critical micro-UX improvement for keyboard navigation.
**Action:** Always ensure navigation is wrapped in semantic list tags and include a skip link that targets the main content area (using `id="main"`).

## 2026-02-21 - [Standardized Focus Indicators]
**Learning:** Consistently using `:focus-visible` with a high-contrast brand color (`#1ee`) and `outline-offset` provides a clear, non-intrusive indicator for keyboard users that integrates with the site's dark theme.
**Action:** Implement `:focus-visible { outline: 2px solid #1ee; outline-offset: 2px; }` in the global stylesheet to ensure all interactive elements are accessible.
