# Design Examples

These are written design specifications, not rendered screenshots. Use them as starting points and adapt them to the actual project.

## Example 1: Glassmorphism SaaS Dashboard
**Best for:** analytics tools, AI workspaces, modern SaaS products.

- Page background: deep slate or a restrained gradient.
- Panels: translucent surfaces with subtle borders and blur where supported.
- Typography: clear, high-contrast headings and readable body text.
- Layout: sidebar, top bar, summary cards, main chart, activity list.
- Components: navigation, KPI cards, chart panel, filters, empty/loading states.
- Accessibility: keep text contrast strong; do not use blur as a substitute for clear surfaces.
- Performance: avoid excessive backdrop filters on large areas.

## Example 2: Minimalist Product Landing Page
**Best for:** SaaS products, developer tools, focused product marketing.

- Layout: compact navigation, strong hero headline, one primary CTA, product preview, benefits, proof, pricing, FAQ, footer.
- Colors: neutral background, dark text, one primary brand color.
- Typography: strong heading hierarchy and comfortable line lengths.
- Components: buttons, feature grid, testimonials or proof, pricing cards.
- Motion: restrained entrance transitions; respect reduced-motion preferences.
- Accessibility: semantic headings, clear links, visible focus states.

## Example 3: Bento Grid Feature Section
**Best for:** product features, AI tool collections, portfolios.

- Layout: responsive grid with cards of varied spans.
- Cards: consistent radius, padding, border, and internal hierarchy.
- Content: each card communicates one feature or outcome.
- Responsive: collapse to fewer columns on narrow screens.
- Accessibility: do not rely on card position or color alone to convey meaning.

## Example 4: Dark Developer Dashboard
**Best for:** developer platforms, monitoring, APIs, technical tools.

- Layout: sidebar, command/search area, KPI row, charts or logs, recent activity.
- Colors: dark neutral surfaces, readable foreground, distinct status tokens.
- Typography: use monospace only for code, IDs, and data where appropriate.
- Components: tables, filters, code blocks, status badges, pagination.
- Accessibility: ensure muted text and status indicators remain distinguishable.

## Example 5: E-commerce Product Detail
**Best for:** online stores and marketplaces.

- Layout: product media, title, price, options, availability, CTA, delivery details, description, reviews.
- Components: image gallery, variant selector, quantity control, cart action, accordions.
- Responsive: stack media and purchase details appropriately on mobile.
- Accessibility: label every option, announce cart updates, provide meaningful image alternatives.

## Example 6: Authentication Page
**Best for:** sign-in, sign-up, password recovery.

- Layout: focused form with clear heading, brief explanation, fields, primary action, recovery links.
- Components: labeled inputs, password visibility control if appropriate, inline validation, loading and error states.
- Accessibility: labels, keyboard access, error messages associated with fields.
- Security: never expose secrets in UI examples or logs.

## Example 7: Admin Data Table
**Best for:** management consoles and operations tools.

- Layout: page title, filters, search, table, pagination, bulk actions where needed.
- States: loading, no results, empty data, errors, selected rows.
- Responsive: use an appropriate mobile alternative instead of forcing an unreadable wide table.
- Accessibility: meaningful headers, keyboard interaction, clear selection states.

## Example 8: Mobile-First Booking Flow
**Best for:** appointments, travel, events, reservations.

- Layout: short progressive steps with clear progress and back navigation.
- Components: date/time picker, selection summary, form fields, confirmation state.
- Accessibility: keyboard support, understandable date/time labels, error recovery.
- UX: preserve user input when moving between steps where feasible.

## Example 9: Editorial / Magazine Layout
**Best for:** blogs, news, long-form content.

- Layout: prominent lead story, readable article column, clear category navigation, related content.
- Typography: readable line length and line height; strong but consistent heading hierarchy.
- Components: article cards, author/date metadata, tags, pagination.
- Accessibility: semantic landmarks and descriptive link text.

## Example 10: Responsive Portfolio
**Best for:** individual developers, designers, agencies.

- Layout: intro, selected work, project details, capabilities, about, contact.
- Components: project cards, technology labels, CTA, optional motion.
- Responsive: stack sections cleanly and avoid tiny tap targets.
- UX: prioritize real work and useful context over decorative effects.

## Example template for adding a new example
### Name
- Best for:
- Layout:
- Colors:
- Typography:
- Components:
- Interaction:
- Responsive behavior:
- Accessibility:
- Trade-offs:
