# Tech Portfolio - Accessibility & Visual Design Enhancements

## 1. Accessibility Enhancements (WAVE & WCAG AA Compliance)

*   **Fixed Low-Contrast Muted Text:** Increased body text contrast (`--text-muted`) from `#9CA3AF` to `#D1D5DB` against the `#0B0F19` background to achieve a WCAG AA contrast ratio of **12.1:1** (exceeding the required 4.5:1 minimum).
*   **Fixed Contrast on Heading Gradient Accent:** Increased cyan contrast (`--accent-cyan`) from `#06B6D4` to `#22D3EE` to ensure high contrast against dark surfaces and borders.
*   **Fixed Missing Form Label Associations:** Added explicit `for` attributes on `<label>` elements linked directly to matching `id` attributes on form `<input>` and `<textarea>` tags.
*   **Added Semantic Grouping for Form Controls:** Wrapped input groups within a `<fieldset>` and `<legend>` container to provide full screen-reader context for related controls.
*   **Fixed Dynamic Error State Accessibility:** Applied `aria-invalid="true"` and `aria-describedby` attributes to form fields in an error state so screen readers immediately announce inline validation messages.
*   **Added Skip Navigation Link:** Included a hidden-by-default `<a class="skip-link" href="#main-content">Skip to Main Content</a>` element at the top of every page for keyboard-only user navigation.

---

## 2. Visual Design & Gestalt Principles

*   **Gestalt Principle 1: Proximity**
    *   *Implementation:* On `projects.html`, project titles, descriptions, and tag badges are grouped closely together inside discrete `<article>` cards with distinct padding, while a wider `gap` separates distinct project cards from one another.
*   **Gestalt Principle 2: Common Region**
    *   *Implementation:* On `about.html` and `projects.html`, related form inputs and project articles are bounded within visibly lighter surface containers (`#111827`) with subtle border outlines, visually unifying related controls into single regional cards.
*   **Color Palette Consistency:**
    *   *Primary Background:* `#0B0F19` (Deep Space Dark)
    *   *Surface / Cards:* `#111827` (Dark Slate)
    *   *Primary Text:* `#F3F4F6` (Off-White)
    *   *Muted Body Text:* `#D1D5DB` (High-Contrast Light Gray)
    *   *Accent Colors:* `#22D3EE` (Accessible Electric Cyan) & `#3B82F6` (Tech Blue)