## 2026-05-18 - [Accessibility & Semantic Navigation Upgrade]
**Learning:** Standardizing navigation to use semantic `<ul>`/`<li>` and `aria-current="page"` significantly improves accessibility and provides a better experience for screen reader users. Adding a "Skip to main content" link is a critical micro-UX improvement for keyboard navigation.
**Action:** Always ensure navigation is wrapped in semantic list tags and include a skip link that targets the main content area (using `id="main"`).

## 2026-02-21 - [Standardized Focus Indicators]
**Learning:** Consistently using `:focus-visible` with a high-contrast brand color (`#1ee`) and `outline-offset` provides a clear, non-intrusive indicator for keyboard users that integrates with the site's dark theme.
**Action:** Implement `:focus-visible { outline: 2px solid #1ee; outline-offset: 2px; }` in the global stylesheet to ensure all interactive elements are accessible.

## 2026-05-20 - [High-Contrast Skip Links & Mobile Hit Targets]
**Learning:** For dark-themed sites with brand-colored accents (like `#0af`), using the brand color as a background for skip links requires switching to a dark text color (e.g., `#000`) to pass WCAG AAA contrast. Additionally, increasing mobile navigation hit targets to at least 44-48px (using `display: block` and padding) significantly improves usability without requiring layout changes.
**Action:** Always verify contrast ratios for skip links against their active state backgrounds and ensure mobile navigation links have a minimum hit area of 44px.

## 2026-05-22 - [Global Link Accessibility]
**Learning:** Default browser blue links (#0000ee) often fail WCAG contrast on dark backgrounds. Using brand-aligned colors (like #0af) for global link styles ensures consistency and readability across all content, not just navigation. Transition effects (e.g., color shift to #1ee) provide essential interactive feedback.
**Action:** Define global link styles with appropriate contrast ratios and hover transitions to ensure accessibility and a cohesive user experience.
