# Changelog

Ledger uses semantic versions. While it is in beta, a minor version adds or changes tokens, components or rules,
and a patch fixes them. Every version is a git tag (`v0.1.0`) and an entry in the design site's record.

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
