# Changelog

Ledger uses semantic versions. While it is in beta, a minor version adds or changes tokens, components or rules,
and a patch fixes them. Every version is a git tag (`v0.1.0`) and an entry in the design site's record.

## 0.2.2 (2026-10-24)

- The highlighted badge keeps its word in `foreground` and marks itself with a primary border and a 10% primary
  tint, the way a selected chip is marked. Its violet word read 3.7:1 on the dark badge, under the 4.5:1 a 12px
  word needs, and broke the rule that `primary` is a fill, not a text color; the word now reads 15.7:1 in light
  and 14.1:1 in dark. The Badge recipe and the gallery's Badge card change; the demo has no highlighted badge.
- The gallery's title, Ledger, is its `h1`, for screen readers; it looks the same.
- The Code recipe's log block takes `tabindex="0"`, `role="region"` and an `aria-label`, so a keyboard can scroll
  it sideways; the demo's activity log does the same, named "Activity log". Both show the focus ring when focused
  and otherwise look the same.
- Figma: not changed in this release; the Badge component's highlighted tone still shows the violet word.

## 0.2.1 (2026-10-14)

- The gallery groups its 24 components under six category headings (Data, Input, Text, Navigation, Status,
  Layout) instead of a row of filter chips under the header. Card names are now `h3` under the section's `h2`.
- The Figma galleries lose the chip row.

## 0.2.0 (2026-10-14)

A blank component sheet and an example screen.

- The gallery is a component sheet with placeholder content instead of a billing dashboard: Save, Continue,
  Cancel and Delete; Email with name@example.com; Option A to D; Active, Pending, Failed, Draft and Scheduled; a
  table of Item A to E under Name, Status, Updated and Value. It has 24 cards (12 with reset) that show variants,
  sizes, disabled, error, and selected and unselected states, laid out as a masonry of cards at their natural
  height, with no scroll area inside a card.
- One new recipe, Button sizes (small, default and large, disabled and busy), so `DESIGN.md` has 24 recipes; every
  recipe's markup uses the gallery's placeholder content. The Data table, Code, Text field, Checkbox, Single
  selection, Toggle and Progress recipes describe their states; the data table no longer scrolls vertically.
- `preview/demo.html`: the billing and operations console of a small software company, built only from the
  recipes: a sidebar, a toolbar with search and a date range, four KPI stats with sparklines, a stacked revenue
  chart in the data palette, an invoice table with tabs, plan chips, sorting, selection and pagination, a
  collections panel, an activity log, and dunning settings. Dark first; `preview/input.css` scans it too.
- Figma: placeholder content in the components, the Cover and both galleries; the Table row gains an Updated
  column, Code an optional source, Progress a negative tone (111 variants in 24 sets) and 11 new icons (27);
  the galleries were rebuilt as the same sheet; a new Example page has `Example/Light` and `Example/Dark`, the
  dashboard rebuilt from instances, with the chart drawn from shapes bound to the variables.
- Fixes: the gallery and the demo take the height of their content and never the window's; log columns keep
  their width on narrow screens.

## 0.1.0 (2026-10-14)

First beta.

- Tokens in light and dark mode, in `ledger.css` (Tailwind CSS v4, shadcn/ui token names plus a data palette:
  `chart-1` to `chart-5`, `positive`, `negative`, `info`) and in the front matter of `DESIGN.md`. Dark mode is
  the reference.
- `DESIGN.md` with the rules, the measured contrast of both modes (every text and control pair at WCAG AA, the
  chart palette checked for color-vision deficiency) and 23 recipes.
- A component gallery in `preview/` laid out as an operations and billing dashboard, with 23 live components,
  category filters, copy on every panel and reset on the 12 that keep state.
- The Figma library "Ledger Design System": 94 variables in four collections (38 primitives, 31 color tokens in
  light and dark, 23 sizes, 2 font families), 14 text styles bound to the font variables, one effect style,
  24 components with 110 variants, 16 Lucide icons, a foundations page, and a light and a dark gallery built
  from instances.
