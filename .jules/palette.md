## 2026-05-18 - [Accessibility & Semantic Navigation Upgrade]
**Learning:** Standardizing navigation to use semantic `<ul>`/`<li>` and `aria-current="page"` significantly improves accessibility and provides a better experience for screen reader users. Adding a "Skip to main content" link is a critical micro-UX improvement for keyboard navigation.
**Action:** Always ensure navigation is wrapped in semantic list tags and include a skip link that targets the main content area (using `id="main"`).

## 2026-05-19 - [Enhanced Keyboard Focus Visibility]
**Learning:** Explicitly styling `:focus-visible` with a high-contrast theme-consistent color (cyan #1ee) significantly improves keyboard navigation accessibility. Relying on default browser focus rings can be insufficient on dark themes.
**Action:** Always include prominent `:focus-visible` styles for all interactive elements to ensure clear visual feedback for keyboard users.
