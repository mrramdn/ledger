# Ledger

A dense, dark-first design system for data-heavy product interfaces: dashboards, admin consoles, analytics, logs, billing and back-office tools. The chrome stays neutral and quiet (graphite or white panels, hairline borders, one violet for actions and focus) so the data can carry color; everything sits on a 4px grid and every number is set in tabular figures. The same tokens exist as a Tailwind CSS v4 theme, a `DESIGN.md` that people and coding agents follow, and a Figma library.

"Ledger" is a working name.

## Files

| File | What it is |
| --- | --- |
| `ledger.css` | Tailwind CSS v4 theme: color tokens (light and dark, with a data palette `chart-1`…`chart-5`, `positive`, `negative`, `info`), radii, the one shadow, type utilities, slider, checkbox and sort-header utilities. Token names follow shadcn/ui. |
| `DESIGN.md` | The rules and the 23 component recipes, in the [design.md](https://github.com/google-labs-code/design.md) format, with the measured contrast of both modes. |
| `preview/index.html` | Component gallery built with the theme, laid out as an operations and billing dashboard. Has a dark mode switch, category filters, and copy and reset buttons per panel. |
| `CHANGELOG.md` | What changed in each version. |

Figma: [Ledger Design System](https://www.figma.com/design/81WUGAI2i0QQoUpjy271bm) (pages Cover, Foundations and Components).

## Use it in a project

1. Load IBM Plex Sans (400, 500, 600) and JetBrains Mono (400, 500, 600), for example with `next/font/google` or `@fontsource/ibm-plex-sans` and `@fontsource/jetbrains-mono`.
2. Copy `ledger.css` next to your main stylesheet and import it after Tailwind:

   ```css
   @import "tailwindcss";
   @import "./ledger.css";
   ```

3. Copy `DESIGN.md` to the project root so coding agents follow the same rules.
4. Dark mode is the `.dark` class on `<html>`. Ledger is designed dark first, so start there and check light mode second.

The theme removes the default Tailwind color palette on purpose. Use the semantic tokens (`bg-card`, `text-muted-foreground`, `bg-primary`, `text-chart-1` and so on) and the `type-*` utilities.

## Preview

```sh
pnpm install
pnpm build   # writes preview/preview.css from the classes in preview/index.html
pnpm dev     # same, watching for changes
```

Then open `preview/index.html` in a browser. Copy needs a secure context, so serve the folder (`python3 -m http.server -d preview`) if the clipboard button does nothing over `file://`.

`npx @google/design.md lint DESIGN.md` checks the token file.

## Versions

The version is in `package.json`, `CHANGELOG.md` says what changed, and every release is a git tag. To release:

1. Change the files and run `pnpm build`, so `preview/preview.css` matches the gallery.
2. Raise `version` in `package.json` and add an entry to `CHANGELOG.md`.
3. Commit, tag `v<version>` (`git tag -a v0.2.0 -m "Ledger 0.2.0"`) and push with `git push --follow-tags`.
4. On the design site, sync this folder and add the version to Ledger's record. The site's tests fail while the
   record states a different version from the synced files.

## Where the look comes from

The look is original. It follows the conventions of dense data tools (graphite layers, hairline borders, tabular numbers, a monospace face for identifiers and logs) without copying any one product. The color pairs were measured for WCAG contrast and the chart palette was checked for color-vision deficiency separation in both modes; the numbers are in `DESIGN.md`.
