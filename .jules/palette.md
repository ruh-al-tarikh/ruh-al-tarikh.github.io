## 2026-05-18 - [Accessibility & Semantic Navigation Upgrade]
**Learning:** Standardizing navigation to use semantic `<ul>`/`<li>` and `aria-current="page"` significantly improves accessibility and provides a better experience for screen reader users. Adding a "Skip to main content" link is a critical micro-UX improvement for keyboard navigation.
**Action:** Always ensure navigation is wrapped in semantic list tags and include a skip link that targets the main content area (using `id="main"`).

## 2026-05-19 - [Visual Consistency & Focus Indicators]
**Learning:** Maintaining visual consistency across pages by standardizing the content structure (e.g., using `<section>` wrappers) and the footer text ensures a professional and predictable user experience. Implementing `:focus-visible` styles provides essential accessibility for keyboard users without adding visual noise for mouse users.
**Action:** Consistently apply the `<main id="main"><section>...</section></main>` pattern and use the standardized footer format. Ensure `:focus-visible` is always present in the global stylesheet.
