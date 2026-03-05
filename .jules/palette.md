## 2026-05-18 - [Accessibility & Semantic Navigation Upgrade]
**Learning:** Standardizing navigation to use semantic `<ul>`/`<li>` and `aria-current="page"` significantly improves accessibility and provides a better experience for screen reader users. Adding a "Skip to main content" link is a critical micro-UX improvement for keyboard navigation.
**Action:** Always ensure navigation is wrapped in semantic list tags and include a skip link that targets the main content area (using `id="main"`).

## 2026-02-22 - [Keyboard Accessibility & Global Focus States]
**Learning:** In minimalist, dark-themed sites, default focus indicators can be hard to see or inconsistent. Implementing a global `:focus-visible` rule with high-contrast colors (like cyan #1ee) and an offset significantly improves the keyboard navigation experience without affecting mouse users.
**Action:** Always implement high-contrast `:focus-visible` styles for all interactive elements to ensure WCAG compliance and clear navigation feedback.
