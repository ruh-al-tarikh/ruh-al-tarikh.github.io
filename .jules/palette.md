## 2026-05-18 - [Accessibility & Semantic Navigation Upgrade]
**Learning:** Standardizing navigation to use semantic `<ul>`/`<li>` and `aria-current="page"` significantly improves accessibility and provides a better experience for screen reader users. Adding a "Skip to main content" link is a critical micro-UX improvement for keyboard navigation.
**Action:** Always ensure navigation is wrapped in semantic list tags and include a skip link that targets the main content area (using `id="main"`).

## 2026-05-19 - [Keyboard Accessibility & Asset Portability]
**Learning:** Implementing explicit `:focus-visible` styles with sufficient contrast and offset is essential for keyboard navigation clarity. Additionally, using relative asset paths in subpages ensures the UI remains intact across different hosting environments (e.g., local file browsing vs. production root).
**Action:** Always add `:focus-visible` outlines to interactive elements and use relative paths for assets in sub-directories to maintain site portability.
