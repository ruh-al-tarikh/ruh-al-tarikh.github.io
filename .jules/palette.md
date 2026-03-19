## 2026-02-21 - [Standardized Focus Indicators]
**Learning:** Consistently using `:focus-visible` with a high-contrast brand color (`#1ee`) and `outline-offset` provides a clear, non-intrusive indicator for keyboard users that integrates with the site's dark theme.
**Action:** Implement `:focus-visible { outline: 2px solid #1ee; outline-offset: 2px; }` in the global stylesheet to ensure all interactive elements are accessible.

## 2026-03-09 - [Link Accessibility in Dark Mode]
**Learning:** Relying purely on color (#0af vs #1ee) to identify links in a dark-themed UI can be difficult for users with low vision or color blindness. Defaulting to underlines for content-area links significantly improves discoverability and compliance with WCAG 1.4.1.
**Action:** Always underline links within the primary content area ('main section') to ensure they are accessible via more than just color.

## 2026-05-18 - [Accessibility & Semantic Navigation Upgrade]
**Learning:** Standardizing navigation to use semantic `<ul>`/`<li>` and `aria-current="page"` significantly improves accessibility and provides a better experience for screen reader users. Adding a "Skip to main content" link is a critical micro-UX improvement for keyboard navigation.
**Action:** Always ensure navigation is wrapped in semantic list tags and include a skip link that targets the main content area (using `id="main"`).

## 2026-05-20 - [High-Contrast Skip Links & Mobile Hit Targets]
**Learning:** For dark-themed sites with brand-colored accents (like `#0af`), using the brand color as a background for skip links requires switching to a dark text color (e.g., `#000`) to pass WCAG AAA contrast. Additionally, increasing mobile navigation hit targets to at least 44-48px (using `display: block` and padding) significantly improves usability without requiring layout changes.
**Action:** Always verify contrast ratios for skip links against their active state backgrounds and ensure mobile navigation links have a minimum hit area of 44px.

## 2026-05-22 - [Global Link Accessibility]
**Learning:** Default browser blue links (#0000ee) often fail WCAG contrast on dark backgrounds. Using brand-aligned colors (like #0af) for global link styles ensures consistency and readability across all content, not just navigation. Transition effects (e.g., color shift to #1ee) provide essential interactive feedback.
**Action:** Define global link styles with appropriate contrast ratios and hover transitions to ensure accessibility and a cohesive user experience.

## 2026-05-24 - [Micro-UX Accessibility and Interaction]
**Learning:** Improving accessibility often involves visual cues beyond just color. Underlining links in prose (WCAG 1.4.1) and ensuring consistent heading hierarchies across the site significantly enhances the user experience for everyone. Adding subtle hover transitions (like a small lift) provides immediate, delightful feedback that makes the interface feel more responsive.
**Action:** Ensure links in body text are underlined by default and use subtle CSS transforms for interactive feedback on navigation elements.

## 2026-05-26 - [Subtle Entrance Animations & Branded Scrollbars]
**Learning:** Subtle entrance animations (fade-in + slight slide) provide a polished, premium feel for content loading. Branded scrollbars further unify the UI design language. Both must be implemented carefully: animations should respect `prefers-reduced-motion`, and scrollbars should maintain enough contrast to remain functional.
**Action:** Use `animation` with a `prefers-reduced-motion: reduce` fallback and `::-webkit-scrollbar` for cohesive branding on webkit browsers.
## 2026-05-25 - [Section Entrance Animations & Path Portability]
**Learning:** Adding subtle entrance animations (e.g., a 0.6s fade-in) can make a static site feel more dynamic and modern. However, these must always respect `prefers-reduced-motion` to remain accessible. Additionally, for GitHub Pages projects, using relative paths for assets (like `../assets/css/style.css`) is more robust than absolute paths (`/assets/css/style.css`), especially when the site is hosted on a sub-path.
**Action:** Use relative paths for cross-page asset linking and always wrap animations in `prefers-reduced-motion` media queries.

## 2026-06-12 - [Focus Management & Custom Scrollbars]
**Learning:** Adding `tabindex="-1"` to the `<main>` element is essential for making "Skip to Content" links work reliably across all browsers and screen readers. Combining this with `main:focus { outline: none; }` allows the focus to move correctly without creating an accidental visual border around the entire page content. Additionally, custom branded scrollbars (using `::-webkit-scrollbar`) provide a final layer of "UI polish" that makes dark-themed sites feel cohesive and intentional.
**Action:** Always pair skip-links with `tabindex="-1"` on the target and implement themed scrollbars to maintain brand consistency in dark mode.

## 2026-06-15 - [Accessible & Stable Scrollbars]
**Learning:** Standard scrollbars often have poor contrast on dark themes, and their appearance can cause "layout jumps." Using `scrollbar-gutter: stable` prevents these shifts, while standard CSS properties like `scrollbar-width` and `scrollbar-color` ensure a consistent, accessible experience across all modern browsers.
**Action:** Always include `scrollbar-gutter: stable` on the `html` element and use high-contrast thumb colors (e.g., #777 on dark backgrounds) for better accessibility.

## 2026-06-20 - [Semantic Hierarchy & Brand Consistency]
**Learning:** Using a single `<h1>` per page for the primary content title and converting the site brand in the header to a `<p class="site-title">` with a link to the homepage creates a clear, logical document hierarchy for screen readers and search engines while maintaining a consistent visual identity. Adding `aria-labelledby` to sections further enhances landmark navigation.
**Action:** Promote primary content headings to `<h1>`, use named landmarks for sections, and ensure the site header brand is a home link with consistent styling across all pages.

## 2026-06-25 - [Modern Typography & Synchronized Interactions]
**Learning:** Modern CSS properties like `text-wrap: balance` (for headings) and `text-wrap: pretty` (for body text) provide high-impact typographic polish with minimal effort. Additionally, using `:focus-within` on containers (like `<section>`) ensures keyboard users receive the same interactive "delight" (like lift effects) as mouse users.
**Action:** Default to modern text-wrap properties for improved readability and use `:focus-within` to unify the experience between mouse and keyboard users.
