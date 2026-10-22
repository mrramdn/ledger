---
version: alpha
name: Ledger
description: A dense, dark-first design system for data-heavy product interfaces. Quiet graphite chrome, hairline borders, one violet, and tabular numbers that line up.
colors:
  primary: "#6246EA"
  primary-hover: "#5236D6"
  primary-foreground: "#FFFFFF"
  background: "#F3F4F6"
  foreground: "#12151B"
  card: "#FFFFFF"
  card-foreground: "#12151B"
  popover: "#FFFFFF"
  popover-foreground: "#12151B"
  secondary: "#E9EBEF"
  secondary-foreground: "#12151B"
  muted: "#F3F4F6"
  muted-foreground: "#5B6472"
  accent: "#E1E4EA"
  accent-foreground: "#12151B"
  destructive: "#CF2E2E"
  destructive-foreground: "#FFFFFF"
  success: "#1B7F4E"
  success-foreground: "#FFFFFF"
  warning: "#B45309"
  info: "#0E7490"
  positive: "#1B7F4E"
  negative: "#CF2E2E"
  chart-1: "#2A78D6"
  chart-2: "#EB6834"
  chart-3: "#199E70"
  chart-4: "#C98500"
  chart-5: "#D55181"
  border: "#E1E4EA"
  input: "#848D9C"
  ring: "#6246EA"
typography:
  display:
    fontFamily: JetBrains Mono
    fontSize: 32px
    fontWeight: 500
    lineHeight: 40px
    letterSpacing: -0.01em
  h1:
    fontFamily: IBM Plex Sans
    fontSize: 24px
    fontWeight: 500
    lineHeight: 32px
    letterSpacing: -0.01em
  h2:
    fontFamily: IBM Plex Sans
    fontSize: 20px
    fontWeight: 500
    lineHeight: 28px
    letterSpacing: -0.01em
  h3:
    fontFamily: IBM Plex Sans
    fontSize: 16px
    fontWeight: 500
    lineHeight: 24px
  title:
    fontFamily: IBM Plex Sans
    fontSize: 14px
    fontWeight: 500
    lineHeight: 20px
  body:
    fontFamily: IBM Plex Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 20px
  button:
    fontFamily: IBM Plex Sans
    fontSize: 13px
    fontWeight: 500
    lineHeight: 20px
  small:
    fontFamily: IBM Plex Sans
    fontSize: 13px
    fontWeight: 400
    lineHeight: 20px
  ui:
    fontFamily: IBM Plex Sans
    fontSize: 13px
    fontWeight: 500
    lineHeight: 20px
  caption:
    fontFamily: IBM Plex Sans
    fontSize: 12px
    fontWeight: 400
    lineHeight: 16px
  overline:
    fontFamily: IBM Plex Sans
    fontSize: 12px
    fontWeight: 500
    lineHeight: 16px
    letterSpacing: 0.06em
  mono:
    fontFamily: JetBrains Mono
    fontSize: 13px
    fontWeight: 400
    lineHeight: 20px
rounded:
  xs: 2px
  sm: 4px
  md: 6px
  lg: 8px
  full: 9999px
spacing:
  "1": 4px
  "2": 8px
  "3": 12px
  "4": 16px
  "5": 20px
  "6": 24px
  "8": 32px
  "10": 40px
  "12": 48px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.primary-foreground}"
    typography: "{typography.button}"
    rounded: "{rounded.sm}"
    height: 32px
    padding: 0 12px
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
  button-secondary:
    backgroundColor: "{colors.card}"
    textColor: "{colors.foreground}"
    borderColor: "{colors.input}"
    typography: "{typography.button}"
    rounded: "{rounded.sm}"
    height: 32px
    padding: 0 12px
  button-secondary-hover:
    backgroundColor: "{colors.accent}"
  button-ghost:
    textColor: "{colors.muted-foreground}"
    typography: "{typography.button}"
    rounded: "{rounded.sm}"
    height: 32px
    padding: 0 12px
  button-ghost-hover:
    backgroundColor: "{colors.accent}"
    textColor: "{colors.foreground}"
  button-destructive:
    backgroundColor: "{colors.destructive}"
    textColor: "{colors.destructive-foreground}"
    typography: "{typography.button}"
    rounded: "{rounded.sm}"
    height: 32px
    padding: 0 12px
  icon-button:
    textColor: "{colors.muted-foreground}"
    rounded: "{rounded.sm}"
    size: 32px
  icon-button-hover:
    backgroundColor: "{colors.accent}"
    textColor: "{colors.foreground}"
  chip:
    backgroundColor: "{colors.card}"
    textColor: "{colors.muted-foreground}"
    borderColor: "{colors.border}"
    typography: "{typography.ui}"
    rounded: "{rounded.sm}"
    height: 28px
    padding: 0 10px
  chip-selected:
    textColor: "{colors.foreground}"
    borderColor: "{colors.primary}"
  toggle:
    backgroundColor: "{colors.input}"
    rounded: "{rounded.sm}"
    width: 36px
    height: 20px
  toggle-checked:
    backgroundColor: "{colors.primary}"
  text-field:
    backgroundColor: "{colors.card}"
    textColor: "{colors.foreground}"
    borderColor: "{colors.input}"
    typography: "{typography.small}"
    rounded: "{rounded.sm}"
    height: 32px
    padding: 0 12px
  segmented:
    backgroundColor: "{colors.muted}"
    borderColor: "{colors.border}"
    rounded: "{rounded.sm}"
    height: 32px
    padding: 2px
  segment-selected:
    backgroundColor: "{colors.accent}"
    textColor: "{colors.foreground}"
    rounded: "{rounded.xs}"
    height: 28px
  tab:
    textColor: "{colors.muted-foreground}"
    typography: "{typography.ui}"
    height: 36px
  tab-selected:
    textColor: "{colors.foreground}"
    borderColor: "{colors.primary}"
  badge:
    backgroundColor: "{colors.muted}"
    textColor: "{colors.foreground}"
    borderColor: "{colors.border}"
    typography: "{typography.caption}"
    rounded: "{rounded.sm}"
    height: 20px
    padding: 0 6px
  status-pill:
    textColor: "{colors.foreground}"
    borderColor: "{colors.border}"
    typography: "{typography.caption}"
    rounded: "{rounded.full}"
    height: 20px
    padding: 0 8px
  table-header:
    backgroundColor: "{colors.muted}"
    textColor: "{colors.muted-foreground}"
    typography: "{typography.overline}"
    height: 36px
    padding: 0 8px
  table-row:
    borderColor: "{colors.border}"
    typography: "{typography.small}"
    height: 36px
    padding: 0 8px
  table-row-hover:
    backgroundColor: "{colors.accent}"
  stat-value:
    textColor: "{colors.foreground}"
    typography: "{typography.display}"
  kbd:
    backgroundColor: "{colors.muted}"
    textColor: "{colors.muted-foreground}"
    borderColor: "{colors.border}"
    typography: "{typography.mono}"
    rounded: "{rounded.xs}"
    height: 20px
  tooltip:
    backgroundColor: "{colors.popover}"
    textColor: "{colors.popover-foreground}"
    borderColor: "{colors.border}"
    typography: "{typography.caption}"
    rounded: "{rounded.sm}"
    padding: 4px 8px
  panel-header:
    borderColor: "{colors.border}"
    typography: "{typography.title}"
    height: 40px
    padding: 0 8px 0 16px
  card:
    backgroundColor: "{colors.card}"
    textColor: "{colors.card-foreground}"
    borderColor: "{colors.border}"
    rounded: "{rounded.lg}"
    padding: 16px
---

# Ledger

## Overview

Ledger is a dense, dark-first system for data-heavy product interfaces: dashboards, admin consoles, analytics, logs, billing and back-office tools, developer tools. One rule explains every decision: the chrome stays neutral and quiet so the data can carry color. Panels are graphite (white in light mode) with hairline borders, text comes in two steps, and a single violet marks actions, selection and focus. Status and chart colors appear only on data, and never alone: a delta has a sign, a status has a dot and a word. Everything sits on a 4px grid, every number is set in tabular figures, and the default control is 32px tall.

Dark mode is the reference, light mode is just as complete, and both are driven by the `.dark` class on a parent element, never by `prefers-color-scheme`.

The same tokens exist in three places and must stay in sync:

- `ledger.css` for Tailwind CSS v4. Token names follow shadcn/ui, with a data palette on top.
- This file, for people and coding agents.
- The Figma library "Ledger Design System" (variables, text styles, components).

When building with Ledger, use the semantic tokens and the recipes under Components. If a screen needs something this file does not cover, build it from the same parts: a panel with a 40px header row and 16px padding, 13px interface text, 36px rows, the mono face for identifiers and the numbers that matter, and at most one violet element competing for attention.

## Colors

Use semantic tokens only. The default Tailwind palette is removed in `ledger.css`, so `bg-blue-500` and similar classes produce nothing.

| Token | Light | Dark | Use |
| --- | --- | --- | --- |
| `background` | `#F3F4F6` | `#0B0D12` | Page |
| `foreground` | `#12151B` | `#E9EBEF` | Text and icons |
| `card` | `#FFFFFF` | `#12151B` | Panels, cards, the top bar, fields, chips |
| `card-foreground` | `#12151B` | `#E9EBEF` | Text on cards |
| `popover` | `#FFFFFF` | `#1E232C` | Menus, tooltips, dialogs: the raised layer |
| `popover-foreground` | `#12151B` | `#E9EBEF` | Text on popovers |
| `primary` | `#6246EA` | `#7F56F0` | The main action, the on state of toggle, slider, radio and checkbox, the selected tab line and chip border |
| `primary-hover` | `#5236D6` | `#6E45E0` | Hover fill for primary |
| `primary-foreground` | `#FFFFFF` | `#FFFFFF` | Text on primary |
| `secondary` | `#E9EBEF` | `#1E232C` | Tracks of sliders, progress and spinners |
| `secondary-foreground` | `#12151B` | `#E9EBEF` | Text on secondary |
| `muted` | `#F3F4F6` | `#171B22` | Table headers, code blocks, keyboard keys, the segmented track |
| `muted-foreground` | `#5B6472` | `#848D9C` | Labels, secondary text, resting icons, overlines |
| `accent` | `#E1E4EA` | `#262C37` | Hover surface, pressed icon buttons, the selected segment |
| `accent-foreground` | `#12151B` | `#E9EBEF` | Text on accent |
| `destructive` | `#CF2E2E` | `#D63B40` | Fill of a destructive button |
| `destructive-foreground` | `#FFFFFF` | `#FFFFFF` | Text on destructive |
| `success` | `#1B7F4E` | `#34C27A` | Success dot or fill |
| `success-foreground` | `#FFFFFF` | `#0B0D12` | Text on a success fill |
| `warning` | `#B45309` | `#E8A33D` | Warning dot, bar or text, with a word |
| `info` | `#0E7490` | `#38BDF8` | Informational dot or log level |
| `positive` | `#1B7F4E` | `#34C27A` | A delta that improved, with its sign |
| `negative` | `#CF2E2E` | `#F4726B` | A delta that worsened, error text, error outlines |
| `chart-1` | `#2A78D6` | `#3987E5` | First series and every single-series chart |
| `chart-2` | `#EB6834` | `#E06A2E` | Second series |
| `chart-3` | `#199E70` | `#2BA878` | Third series |
| `chart-4` | `#C98500` | `#B48C0F` | Fourth series |
| `chart-5` | `#D55181` | `#D45C8E` | Fifth series |
| `border` | `#E1E4EA` | `#232931` | Hairlines: panel edges, dividers, table rows |
| `input` | `#848D9C` | `#5B6472` | Outline of fields and secondary buttons, the off track of a toggle |
| `ring` | `#6246EA` | `#7F56F0` | Focus ring |

Dark mode is the `.dark` class on a parent element.

Rules:

- The chrome is gray. Surfaces, borders, labels and body text never carry a hue; `primary` is the only colored part of the chrome, and one view shows it on one thing at a time: the main action, or the current selection.
- Color belongs to data. Series take `chart-1` to `chart-5` in that fixed order and never a status color; a chart with one series uses `chart-1`. Deltas take `positive` or `negative` with a sign (▲ ▼ + −); statuses take a dot in `success`, `warning`, `negative`, `info` or `muted-foreground` next to a word. A status color never stands alone.
- `primary` and `destructive` are fills, not text colors. Links and selected labels are `foreground` with an underline or a primary line; error text is `negative`.
- Two text steps: `foreground` for values and titles, `muted-foreground` for labels, captions and overlines. Disabled parts use 40% opacity instead of a third gray.
- `border` separates, `input` outlines. A hairline is for edges inside the chrome; a control that must be found by its boundary (field, secondary button, switch track) uses `input`, which reaches 3:1.

Measured contrast (WCAG 2, light then dark):

- Text: `foreground` on `background` 16.6 and 16.3; on `card` 18.3 and 15.3; on `secondary` 15.3 and 13.2. `muted-foreground` on `background` 5.4 and 5.8; on `card` 6.0 and 5.5; on `secondary` 5.0 and 4.7. All AA, most AAA.
- Primary: `primary-foreground` on `primary` 5.9 and 4.7; on `primary-hover` 7.3 and 5.8. AA in both modes.
- Status text on `card`: `positive` 5.0 and 8.0; `negative` 5.1 and 6.5; `warning` 5.0 and 8.5; `info` 5.4 and 8.5. `destructive-foreground` on `destructive` 5.1 and 4.6. All AA.
- Boundaries (3:1): `input` on `card` 3.3 and 3.1, on `background` 3.0 and 3.2; `ring` on `background` 5.3 and 4.2; `primary` on `card` 5.9 and 3.9.
- Charts (3:1 for graphics): `chart-1` to `chart-5` on `card` 4.4, 3.2, 3.4, 3.1, 3.9 in light and 5.0, 5.5, 6.1, 5.8, 5.0 in dark. Adjacent pairs were checked for color-vision deficiency in both modes (worst protan ΔE 8.4 light, 9.5 dark).

Three pairs fall below the AA threshold they would need if misused, so the rules above keep them out of those uses:

- `primary` as 13px text on the dark `card` is 3.9:1 (AA asks 4.5:1). Set links and selected labels in `foreground`; if a violet text is unavoidable, `#9D86F5` gives 6.1:1 on the dark card.
- `destructive` as text on the dark `card` is 4.0:1. Error text uses `negative` (`#F4726B`, 6.5:1); the destructive fill keeps its white text at 4.6:1.
- `chart-2` and `chart-4` on the light `background` are 2.9:1 and 2.8:1. Charts sit on `card`, where every series passes; a chart drawn on the page gray needs direct labels.

`border` on `card` is 1.3:1 and 1.2:1 by design: hairlines separate panels and rows without boxing them in, and nothing is identified by a hairline alone.

## Typography

IBM Plex Sans for interface text and JetBrains Mono for identifiers, code, log lines, keyboard keys and KPI values. Both are loaded by the app (`next/font`, `@fontsource` or a link tag). Weights 400, 500 and 600; 600 is for the wordmark only. `ledger.css` sets `font-variant-numeric: tabular-nums` on `html`, so every number lines up without a class.

| Utility | Size / line | Weight | Tracking | Use |
| --- | --- | --- | --- | --- |
| `type-display` | 32 / 40 | 500 | -0.01em | KPI values and the wordmark, in the mono face |
| `type-h1` | 24 / 32 | 500 | -0.01em | Page title |
| `type-h2` | 20 / 28 | 500 | -0.01em | Section title |
| `type-h3` | 16 / 24 | 500 | 0 | Subsection, dialog title |
| `type-title` | 14 / 20 | 500 | 0 | Panel and card titles |
| `type-body` | 14 / 20 | 400 | 0 | Body copy, descriptions |
| `type-ui` | 13 / 20 | 500 | 0 | Buttons, chips, tabs, field labels, segment labels |
| `type-small` | 13 / 20 | 400 | 0 | Table cells, list labels, option labels, field text |
| `type-caption` | 12 / 16 | 400 | 0 | Hints, timestamps, footers |
| `type-overline` | 12 / 16 | 500 | 0.06em | Table headers and section labels, uppercase |
| `type-mono` | 13 / 20 | 400 | 0 | IDs, amounts, timestamps, code, log lines, keyboard keys |

Buttons use the `button` role: 13 / 20, weight 500, the same as `type-ui`.

Rules:

- Use the `type-*` utilities instead of composing size, weight and tracking by hand. They are named `type-*` so that `tailwind-merge` does not confuse them with text colors.
- Nothing is set below 12px, and 12px is only for captions and overlines.
- Headings are small and medium weight. Dense interfaces do not shout: a 24px title is the largest text on a page besides a KPI value.
- Uppercase only in `type-overline`, at 12px or more, tracked 0.06em. Sentence case everywhere else.
- Numbers that are compared or scanned (amounts, counts, timestamps, IDs) are `type-mono`, right-aligned in columns. Prose numbers stay in Plex Sans.
- Field text is 13px because Ledger is desktop first. On a phone-first product, raise inputs to 16px so mobile browsers do not zoom on focus.

## Layout

- Spacing uses the 4px grid. Common steps: 4 (between icon and label), 8 (inside a control, between chips), 12 (compact panel padding), 16 (panel padding, grid gaps), 24 and 32 (between sections).
- Heights: controls 28 (small), 32 (default) and 36 (large); table and list rows 36 (32 compact); panel header 40; badges, pills and keyboard keys 20; icons 16.
- The page is `bg-background`. Content lives in panels (`bg-card` with a hairline border); only a page title or a filter row sits loose on the page.
- A dashboard is a grid with `gap-4`: one column on phones, more from 640px. KPI stats sit in one row, wide panels (charts, tables, logs) span columns, and every panel takes the height of its content: no fixed heights, no heights tied to the window, and no panel that scrolls vertically. A long table shows a page of rows with pagination.
- A panel has a 40px header row (title left, quiet icon buttons right) over a body with 16px padding. Tables and logs sit in their own bordered container inside the body and scroll sideways only.
- An app shell puts a 224px sidebar of ghost buttons (icon and label, the current page with `aria-current="page"` and the `accent` fill) left of the content from 1024px; below that the nav becomes a row above it.
- The top bar is a 40px `bg-card` strip with a bottom hairline: the wordmark on the left, context (environment, version, time) in `type-mono` and the theme switch on the right. Filters are a row of chips below it.
- Text aligns left; numbers align right. A key-value row puts the label in `muted-foreground` on the left and the mono value on the right.

## Elevation & Depth

The system is flat. Depth is three graphite steps and hairlines.

- Dark: page `#0B0D12`, panel `#12151B`, raised `#1E232C`. Light: page `#F3F4F6`, panel white, raised white with a hairline and a shadow.
- Panels, cards, fields and buttons have a 1px border and no shadow.
- `shadow-lg` is the only shadow, for surfaces that float: menus, tooltips, dialogs. Always pair it with the `border`.
- Selection uses tint, not depth: a selected row or chip gets `bg-primary/10`, a hovered row `bg-accent/40`.
- Nothing is embossed or glassy. A keyboard key shows its 2px bottom border, not a bevel.

## Shapes

Small radii, consistent everywhere.

- Controls are 4px (`rounded-sm`): buttons, chips, fields, badges, the switch track, checkboxes.
- Panels inside a card are 6px (`rounded-md`): tables, lists, code blocks, the segmented track.
- Cards and panels are 8px (`rounded-lg`).
- Tracks and inner parts are 2px (`rounded-xs`): slider and progress tracks, the segment, keyboard keys, the switch thumb.
- Only two things are round: the radio button and the status pill (`rounded-full`), so a status reads as a status at a glance.

`--radius` is `0.375rem`, so shadcn/ui components come out close: `rounded-md` is 6px, `rounded-lg` and `rounded-xl` are 8px. For exact 4px controls use `rounded-sm`.

Icons are Lucide at 16px (`size-4`) with a 1.75 stroke in `currentColor`. Icon-only buttons need an `aria-label`.

## Components

Copy these recipes. The live versions, with the same classes and the same placeholder content, are in `preview/index.html`, one card per recipe. `preview/demo.html` is an example screen, a billing and operations dashboard, built only from these recipes and layout utilities.

### Button

32px, 4px radius, 13px medium text. One primary button per view; a destructive button only for actions that delete or cannot be undone.

```html
<button type="button" class="inline-flex h-8 shrink-0 items-center justify-center gap-1.5 rounded-sm px-3 type-ui whitespace-nowrap transition-colors disabled:pointer-events-none disabled:opacity-40 bg-primary text-primary-foreground hover:bg-primary-hover">Save</button>
```

- Secondary: replace the color classes with `border border-input bg-card text-foreground hover:bg-accent`.
- Ghost: `text-muted-foreground hover:bg-accent hover:text-foreground`.
- Destructive: `bg-destructive text-destructive-foreground hover:bg-destructive/90`.
- The gallery labels them by job: Save (primary), Continue (secondary), Cancel (ghost), Delete (destructive).
- An icon goes before the label at 16px with the 6px gap the class already sets.

### Button sizes

Three heights with the same 13px text, and two states. Small is for table rows, toolbars and card footers; large for a form's one submit button.

```html
<button type="button" class="inline-flex h-8 shrink-0 items-center justify-center gap-1.5 rounded-sm px-3 type-ui whitespace-nowrap transition-colors disabled:pointer-events-none disabled:opacity-40 border border-input bg-card text-foreground hover:bg-accent h-7 px-2.5">Small</button>
<button type="button" class="inline-flex h-8 shrink-0 items-center justify-center gap-1.5 rounded-sm px-3 type-ui whitespace-nowrap transition-colors disabled:pointer-events-none disabled:opacity-40 border border-input bg-card text-foreground hover:bg-accent">Default</button>
<button type="button" class="inline-flex h-8 shrink-0 items-center justify-center gap-1.5 rounded-sm px-3 type-ui whitespace-nowrap transition-colors disabled:pointer-events-none disabled:opacity-40 border border-input bg-card text-foreground hover:bg-accent h-9 px-4">Large</button>
<button type="button" disabled class="inline-flex h-8 shrink-0 items-center justify-center gap-1.5 rounded-sm px-3 type-ui whitespace-nowrap transition-colors disabled:pointer-events-none disabled:opacity-40 bg-primary text-primary-foreground hover:bg-primary-hover"><span class="size-3.5 animate-spin rounded-full border-2 border-white/30 border-t-white" aria-hidden="true"></span>Saving</button>
```

- Small (28px): `h-7 px-2.5`. Large (36px): `h-9 px-4`. Nothing is smaller than 28px.
- Disabled is the native `disabled` attribute at 40% opacity. A busy button is `disabled` with a 14px spinner in place of the icon and a verb in the -ing form (Saving, Sending).

### Icon button

32px square hit area around a 16px icon. A toggle icon button carries `aria-pressed`.

```html
<button type="button" aria-label="Copy" class="inline-flex size-8 shrink-0 items-center justify-center rounded-sm text-muted-foreground transition-colors hover:bg-accent hover:text-foreground aria-pressed:bg-accent aria-pressed:text-foreground disabled:pointer-events-none disabled:opacity-40"><!-- 16px Lucide icon --></button>
```

Small (28px) in table rows and pagination: `size-7`. A pressed toggle icon button has the `accent` fill; a disabled one is at 40% opacity.

### Chip

28px filter chip with an optional mono count. Exactly one chip in a group has `aria-pressed="true"`; the selected chip gets the primary border and a 10% tint.

```html
<button type="button" aria-pressed="true" class="inline-flex h-7 shrink-0 items-center gap-1.5 rounded-sm border border-border bg-card px-2.5 type-ui text-muted-foreground transition-colors hover:text-foreground aria-pressed:border-primary aria-pressed:bg-primary/10 aria-pressed:text-foreground">All<span class="type-mono text-xs">128</span></button>
```

A chip that opens a menu ends with a 14px chevron-down icon and, when a value is set, shows it in mono (`Status Active`); it toggles its own `aria-pressed` instead of joining a group.

### Toggle

36 by 20px switch with the control radius, not a pill. Flip `aria-checked` on click; label it with visible text in a 36px row. A disabled switch gets `disabled`, and its label `opacity-40`.

```html
<div class="flex h-9 w-full items-center justify-between gap-4"><span class="type-small">Notifications</span><button type="button" role="switch" aria-checked="true" aria-label="Notifications" class="group relative h-5 w-9 shrink-0 rounded-sm bg-input transition-colors aria-checked:bg-primary disabled:opacity-40"><span class="absolute top-0.5 left-0.5 size-4 rounded-xs bg-white transition-transform group-aria-checked:translate-x-4"></span></button></div>
```

### Slider

A native range input with the `ledger-slider` utility: a 4px track and a 16px square thumb. The label and the mono readout share a row above. Chrome and Safari need `--slider-fill` to paint the filled part, so update it, and the `output`, on every `input` event.

```html
<div class="w-full"><div class="flex items-baseline justify-between"><label for="value" class="type-ui">Value</label><output for="value" class="type-mono text-muted-foreground" data-unit="%">50%</output></div><input id="value" type="range" min="0" max="100" value="50" class="ledger-slider mt-2" /><p class="mt-2 type-caption text-muted-foreground">Supporting text that explains the setting.</p></div>
```

```js
el.style.setProperty('--slider-fill', `${((el.value - el.min) / (el.max - el.min)) * 100}%`);
output.textContent = `${el.value}${output.dataset.unit}`;
```

### Single selection (radio)

Native radios in a `fieldset` with a `legend`, one per 32px row. The checked state is a 5px primary ring around a card-colored center. A disabled option has `disabled` on the input and `text-muted-foreground` on its label.

```html
<fieldset class="w-full"><legend class="type-ui">Choose one</legend><div class="mt-2 flex flex-col"><label class="flex h-8 items-center gap-2.5 type-small"><input type="radio" name="choice" value="a" class="size-4 shrink-0 appearance-none rounded-full border border-input bg-card transition-[border-width,border-color] checked:border-5 checked:border-primary disabled:opacity-40" />Option A</label><label class="flex h-8 items-center gap-2.5 type-small"><input type="radio" name="choice" value="b" checked class="size-4 shrink-0 appearance-none rounded-full border border-input bg-card transition-[border-width,border-color] checked:border-5 checked:border-primary disabled:opacity-40" />Option B <span class="text-muted-foreground">Default</span></label></div></fieldset>
```

### Checkbox

A native checkbox with the `ledger-checkbox` utility: 16px, 4px radius, a primary fill with a white check when checked and a dash when `indeterminate` (set the property from script). A "Select all" box sits above its options, which are indented by 26px (`pl-6.5`), shows the dash when only some are checked, and its hint counts them (`2 of 3`).

```html
<label class="flex h-8 items-center gap-2.5 type-small"><input type="checkbox" checked class="ledger-checkbox" />Option A</label>
```

### Text field

32px field with a 13px label above and an optional hint or unit. Numeric fields are `type-mono text-right`.

```html
<label class="block w-full"><span class="type-ui">Email</span><input type="email" placeholder="name@example.com" class="h-8 w-full rounded-sm border border-input bg-card px-3 type-small text-foreground placeholder:text-muted-foreground disabled:opacity-40 mt-1.5" /><span class="mt-1.5 block type-caption text-muted-foreground">Supporting text for the field.</span></label>
<label class="block w-full"><span class="type-ui">Value</span><span class="relative mt-1.5 block"><input type="text" inputmode="decimal" value="12.5" class="h-8 w-full rounded-sm border border-input bg-card px-3 type-small text-foreground placeholder:text-muted-foreground disabled:opacity-40 pr-8 type-mono text-right" /><span class="pointer-events-none absolute inset-y-0 right-3 flex items-center type-small text-muted-foreground">%</span></span></label>
```

An error adds `aria-invalid="true"` and `aria-describedby`, swaps `border-input` for `border-negative`, and puts a `type-caption text-negative` message below that says how to fix the value:

```html
<label class="block w-full"><span class="type-ui">Email</span><input type="email" value="name@example" aria-invalid="true" aria-describedby="email-error" class="h-8 w-full rounded-sm border border-input bg-card px-3 type-small text-foreground placeholder:text-muted-foreground disabled:opacity-40 mt-1.5 border-negative" /><span id="email-error" class="mt-1.5 block type-caption text-negative">Enter an email such as name@example.com.</span></label>
```

A disabled field has `disabled` and its label `text-muted-foreground`. A search field puts a 16px search icon at `left-2.5` and pads the input with `pl-8`.

### Segmented control

A 32px track in `muted` with a hairline; segments are 28px buttons with `aria-pressed`, exactly one pressed, filled with `accent`.

```html
<div role="group" aria-label="Period" class="inline-flex h-8 items-center gap-0.5 rounded-sm border border-border bg-muted p-0.5"><button type="button" aria-pressed="false" class="h-7 rounded-xs px-2.5 type-ui text-muted-foreground transition-colors hover:text-foreground aria-pressed:bg-accent aria-pressed:text-foreground">Day</button><button type="button" aria-pressed="true" class="h-7 rounded-xs px-2.5 type-ui text-muted-foreground transition-colors hover:text-foreground aria-pressed:bg-accent aria-pressed:text-foreground">Week</button><button type="button" aria-pressed="false" class="h-7 rounded-xs px-2.5 type-ui text-muted-foreground transition-colors hover:text-foreground aria-pressed:bg-accent aria-pressed:text-foreground">Month</button></div>
```

Use it for a view switch of two to five short options (Day / Week / Month, a date range, density). Longer sets are Tabs.

### Tabs

36px tabs on a hairline; the selected tab is `foreground` with a 2px primary line. The arrow keys move between tabs and show the matching `tabpanel`.

```html
<div role="tablist" aria-label="Sections" class="flex w-full gap-2 overflow-x-auto border-b border-border"><button type="button" role="tab" id="tab-items" aria-selected="true" aria-controls="panel-items" class="inline-flex h-9 shrink-0 items-center gap-1.5 border-b-2 border-transparent px-1 type-ui text-muted-foreground transition-colors hover:text-foreground aria-selected:border-primary aria-selected:text-foreground">Items<span class="inline-flex h-5 items-center rounded-sm border border-border bg-muted px-1.5 text-xs leading-4 font-medium">128</span></button></div>
<div role="tabpanel" id="panel-items" aria-labelledby="tab-items" class="pt-2"><!-- content --></div>
```

### Badge

20px label for counts, versions and environments. Neutral by default; a mono badge for versions and IDs.

```html
<span class="inline-flex h-5 items-center rounded-sm border border-border bg-muted px-1.5 text-xs leading-4 font-medium">128</span>
```

- Version or ID: add `font-mono`.
- Quiet: add `text-muted-foreground`. Highlighted (one per view): swap `border-border bg-muted` for `border-primary bg-primary/10` and keep the word in `foreground`, the way a selected chip is marked, for a single word only, such as New. The word reads 15.7:1 and 14.1:1 on the tint, and the primary border is 5.9:1 and 3.9:1 against the card; violet text would be 3.7:1 on the dark badge.

### Status pill

The one round control: a 20px pill with a status dot and the word, in `foreground`. The dot is `success` (Active, Paid), `warning` (Pending, Due), `negative` (Failed, Overdue), `muted-foreground` (Draft) or `info` (Scheduled); the word always comes with it.

```html
<span class="inline-flex h-5 items-center gap-1.5 rounded-full border border-border px-2 text-xs leading-4 font-medium whitespace-nowrap"><span class="size-1.5 rounded-full bg-success" aria-hidden="true"></span>Active</span>
```

### Progress

A 4px bar under a label row with a mono value. The fill is `primary`; a bar that reports a problem is `warning` or `negative`, and then the value is in the same color and gets a word (`92% used`, `100% reached`).

```html
<div class="w-full"><div class="flex items-baseline justify-between"><span class="type-ui">Progress</span><span class="type-mono text-muted-foreground">64%</span></div><div role="progressbar" aria-label="Progress" aria-valuenow="64" aria-valuemin="0" aria-valuemax="100" class="mt-2 h-1 w-full overflow-hidden rounded-xs bg-secondary"><div class="h-full w-[64%] rounded-xs bg-primary"></div></div></div>
```

### List

Key-value rows of 36px in a 6px bordered panel: the label in `muted-foreground` left, the mono value right.

```html
<ul class="w-full divide-y divide-border rounded-md border border-border"><li class="flex h-9 items-center justify-between gap-4 px-3"><span class="type-small text-muted-foreground">Account</span><span class="type-mono">Personal</span></li></ul>
```

### Spinner

16px, two-tone ring. Put the count of what is loading next to it when it is known.

```html
<span role="status" aria-label="Loading" class="size-4 animate-spin rounded-full border-2 border-secondary border-t-primary"></span>
```

### Card

The panel every dashboard is made of: 8px radius, hairline, a 40px header row with the title and quiet icon buttons, a body with 16px padding, and an optional 40px footer.

```html
<article class="flex w-full flex-col rounded-lg border border-border bg-card"><header class="flex h-10 items-center justify-between border-b border-border pr-2 pl-4"><h3 class="type-title">Card title</h3><!-- icon buttons --></header><div class="flex flex-col gap-1 p-4"><span class="type-overline text-muted-foreground">Metric</span><span class="type-display">12.5%</span><span class="type-caption text-muted-foreground">Supporting text that explains the item in a line or two.</span></div><footer class="flex h-10 items-center justify-between border-t border-border pr-2 pl-4"><span class="type-caption text-muted-foreground">Updated 14 Oct 2026</span><!-- small ghost button --></footer></article>
```

### Data table

36px rows in a 6px bordered container, a `muted` header with overline labels, a checkbox column, right-aligned mono numbers and a status pill. A sortable header is a button inside a `th` with `aria-sort`; the `ledger-sort` utility draws the arrow from that attribute. A selected row carries `data-selected`.

```html
<div class="w-full overflow-x-auto rounded-md border border-border"><table class="w-full border-collapse type-small"><thead class="bg-muted"><tr><th scope="col" class="h-9 px-2 text-left whitespace-nowrap type-overline text-muted-foreground shadow-[inset_0_-1px_0_0_var(--border)] w-9"><input type="checkbox" class="ledger-checkbox" aria-label="Select all rows" /></th><th scope="col" aria-sort="none" class="h-9 px-2 text-left whitespace-nowrap type-overline text-muted-foreground shadow-[inset_0_-1px_0_0_var(--border)]"><button type="button" class="ledger-sort inline-flex items-center rounded-xs type-overline transition-colors hover:text-foreground">Name</button></th><th scope="col" class="h-9 px-2 text-left whitespace-nowrap type-overline text-muted-foreground shadow-[inset_0_-1px_0_0_var(--border)]">Status</th><th scope="col" aria-sort="none" class="h-9 px-2 text-left whitespace-nowrap type-overline text-muted-foreground shadow-[inset_0_-1px_0_0_var(--border)]"><button type="button" class="ledger-sort inline-flex items-center rounded-xs type-overline transition-colors hover:text-foreground">Updated</button></th><th scope="col" aria-sort="none" class="h-9 px-2 text-left whitespace-nowrap type-overline text-muted-foreground shadow-[inset_0_-1px_0_0_var(--border)] text-right"><button type="button" class="ledger-sort inline-flex items-center rounded-xs type-overline transition-colors hover:text-foreground">Value</button></th></tr></thead><tbody><tr class="h-9 border-b border-border last:border-b-0 transition-colors hover:bg-accent/40 data-selected:bg-primary/10"><td class="px-2 whitespace-nowrap"><input type="checkbox" class="ledger-checkbox" aria-label="Select Item A" /></td><td class="px-2 whitespace-nowrap" data-sort="Item A">Item A</td><td class="px-2 whitespace-nowrap"><span class="inline-flex h-5 items-center gap-1.5 rounded-full border border-border px-2 text-xs leading-4 font-medium whitespace-nowrap"><span class="size-1.5 rounded-full bg-success" aria-hidden="true"></span>Active</span></td><td class="px-2 whitespace-nowrap type-mono text-muted-foreground" data-sort="2026-10-14">14 Oct 2026</td><td class="px-2 whitespace-nowrap type-mono text-right" data-sort="1234">1,234</td></tr></tbody></table></div>
```

- Clicking a sort button sets its `th` to `ascending` or `descending`, resets the others to `none`, and reorders the rows by the cells' `data-sort` values (dates as ISO strings, numbers without separators).
- The header checkbox selects every row and is `indeterminate` when only some are selected.
- The table takes the height of its rows and never scrolls vertically: show a page of rows and put Pagination under it. The container scrolls sideways only when the columns do not fit (below 640px).
- Compact tables use `h-8` rows. Dates and amounts are mono; amounts in one currency stay right-aligned in one column.

### Stat

A KPI: an overline label, the value in `type-display`, a signed delta in `positive` or `negative`, an inline SVG sparkline in `chart-1`, and secondary rows below a hairline. The sparkline is a `path` in a 240×48 box with `preserveAspectRatio="none"` and `vector-effect="non-scaling-stroke"`, so it stretches to the panel and keeps a 1.5px line.

```html
<div class="flex w-full flex-col"><div class="flex items-center justify-between"><span class="type-overline text-muted-foreground">Metric</span><span class="type-caption text-muted-foreground">Last 24 h</span></div><div class="mt-1 flex items-baseline gap-2"><span class="type-display">1,234</span><span class="inline-flex items-center gap-1 type-ui text-positive"><svg width="8" height="8" viewBox="0 0 8 8" aria-hidden="true"><path d="M4 1 7.5 7h-7z" fill="currentColor"/></svg>2.4%</span></div><svg class="mt-3 h-12 w-full text-chart-1" viewBox="0 0 240 48" preserveAspectRatio="none" aria-hidden="true"><path d="M0.0 46.0 L17.1 40.5 L34.3 43.6 L51.4 34.2 L68.6 37.2 L85.7 26.6 L102.9 21.1 L120.0 27.3 L137.1 18.1 L154.3 14.5 L171.4 18.6 L188.6 8.8 L205.7 4.3 L222.9 9.8 L240.0 2.0 L240 48 L0 48 Z" fill="currentColor" fill-opacity="0.1"/><path d="M0.0 46.0 L17.1 40.5 L34.3 43.6 L51.4 34.2 L68.6 37.2 L85.7 26.6 L102.9 21.1 L120.0 27.3 L137.1 18.1 L154.3 14.5 L171.4 18.6 L188.6 8.8 L205.7 4.3 L222.9 9.8 L240.0 2.0" fill="none" stroke="currentColor" stroke-width="1.5" vector-effect="non-scaling-stroke"/></svg><div class="mt-3 flex items-baseline justify-between border-t border-border pt-3"><span class="type-small text-muted-foreground">Rate</span><span class="inline-flex items-baseline gap-2"><span class="type-mono">12.5%</span><span class="inline-flex items-center gap-1 type-ui text-positive"><svg width="8" height="8" viewBox="0 0 8 8" aria-hidden="true"><path d="M4 1 7.5 7h-7z" fill="currentColor"/></svg>0.4 pt</span></span></div></div>
```

The delta's color says whether the change is good, the triangle says which way it went: a duration that grew is a red ▲, a cost that fell a green ▼. The sparkline carries no status color.

### Toolbar

A `role="toolbar"` row above a list or table: a search field that grows, filter chips (with a chevron when they open a menu) and an action button, wrapping on narrow screens.

```html
<div role="toolbar" aria-label="Items" class="flex w-full flex-wrap items-center gap-2"><label class="relative min-w-40 flex-1"><span class="sr-only">Search</span><span class="pointer-events-none absolute inset-y-0 left-2.5 flex items-center text-muted-foreground"><!-- 16px search icon --></span><input type="search" placeholder="Search" class="h-8 w-full rounded-sm border border-input bg-card px-3 type-small text-foreground placeholder:text-muted-foreground disabled:opacity-40 pl-8" /></label><div role="group" aria-label="Filters" class="flex gap-2"><!-- chips: Status, Date --></div><!-- secondary button: Export --></div>
```

### Keyboard key

A 20px key in the mono face with a 2px bottom border. Keys of one shortcut sit 4px apart; "then" between two chords is a caption.

```html
<kbd class="inline-flex h-5 min-w-5 items-center justify-center rounded-xs border border-b-2 border-border bg-muted px-1 font-mono text-xs leading-4 text-muted-foreground">⌘</kbd>
```

### Code

A log block: a 6px `muted` panel with one mono line per entry: a muted timestamp, the level as a word in `info`, `warning` or `negative`, and the message. Lines do not wrap; the block scrolls sideways.

```html
<div class="w-full overflow-x-auto rounded-md border border-border bg-muted p-3 type-mono"><div class="flex flex-col gap-1"><span class="flex gap-3 whitespace-nowrap"><span class="shrink-0 text-muted-foreground">12:04:31</span><span class="w-10 shrink-0 text-info">info</span><span>Task started</span></span><span class="flex gap-3 whitespace-nowrap"><span class="shrink-0 text-muted-foreground">12:04:33</span><span class="w-10 shrink-0 text-warning">warn</span><span>Retry 1 of 3</span></span></div></div>
```

A source column (`w-16 shrink-0 text-muted-foreground`) may sit between the level and the message. Inline code in prose: `<code class="rounded-xs bg-muted px-1 py-0.5 type-mono">pnpm build</code>`.

### Pagination

A `nav` with the range in mono on the left and 28px page buttons on the right; the current page has `aria-current="page"` and the `accent` fill. Previous and next are small icon buttons, disabled at the ends.

```html
<nav aria-label="Pagination" class="flex w-full flex-wrap items-center justify-between gap-3"><span class="type-small text-muted-foreground"><span class="type-mono text-foreground">1–50</span> of <span class="type-mono text-foreground">1,234</span></span><div class="flex items-center gap-0.5"><button type="button" aria-label="Previous page" disabled class="inline-flex size-7 shrink-0 items-center justify-center rounded-sm text-muted-foreground transition-colors hover:bg-accent hover:text-foreground aria-pressed:bg-accent aria-pressed:text-foreground disabled:pointer-events-none disabled:opacity-40"><!-- chevron-left --></button><button type="button" aria-current="page" class="h-7 min-w-7 rounded-sm px-1.5 type-mono text-muted-foreground transition-colors hover:bg-accent hover:text-foreground aria-[current=page]:bg-accent aria-[current=page]:text-foreground">1</button><button type="button" aria-label="Next page" class="inline-flex size-7 shrink-0 items-center justify-center rounded-sm text-muted-foreground transition-colors hover:bg-accent hover:text-foreground aria-pressed:bg-accent aria-pressed:text-foreground disabled:pointer-events-none disabled:opacity-40"><!-- chevron-right --></button></div></nav>
```

### Tooltip

CSS only: a `group` wrapper shows the `role="tooltip"` element on hover and on focus within. The tooltip is the raised layer (`popover`) with the hairline and the one shadow, 12px text, one line where possible. The trigger points at it with `aria-describedby`; `data-open` on the wrapper keeps one open in documentation.

```html
<span class="group relative inline-flex"><button type="button" aria-describedby="tip-label" class="inline-flex h-8 shrink-0 items-center justify-center gap-1.5 rounded-sm px-3 type-ui whitespace-nowrap transition-colors disabled:pointer-events-none disabled:opacity-40 border border-input bg-card text-foreground hover:bg-accent h-7 px-2.5">Label</button><span role="tooltip" id="tip-label" class="pointer-events-none absolute bottom-full left-1/2 z-10 mb-2 w-max max-w-56 -translate-x-1/2 rounded-sm border border-border bg-popover px-2 py-1 type-caption text-popover-foreground opacity-0 shadow-lg transition-opacity group-hover:opacity-100 group-focus-within:opacity-100 group-data-open:opacity-100">Tooltip text, one short line</span></span>
```

### Focus

Every interactive element gets the global focus ring from `ledger.css`: a 2px `ring` outline with a 1px offset, visible on graphite and on white. Do not remove it, and do not replace it with a color change alone.

## Do's and Don'ts

- Do keep the chrome gray: surfaces, hairlines, labels and body text have no hue, so color on data means something.
- Do pair every status or delta color with a sign, an icon or a word, and give series their colors in the fixed order `chart-1` to `chart-5`.
- Do set compared numbers in `type-mono`, right-aligned, and let the tabular figures line them up.
- Do keep one violet element competing for attention per view: the main action, or the current selection.
- Do give icon-only buttons an `aria-label`, sortable headers `aria-sort`, switches `role="switch"`, and every field a visible label.
- Don't set text in `primary` or `destructive`; links are `foreground` with an underline, error text is `negative`.
- Don't go below 12px text or 28px controls, and don't drop the 4px grid for a one-off size.
- Don't add shadows to panels, cards, fields or buttons; only menus and tooltips float.
- Don't use pills or large radii; controls are 4px, panels 6px, cards 8px. Only the radio and the status pill are round.
- Don't use the default Tailwind palette, hard-coded hex values, gradients or tinted panels.
- Don't draw a chart in a status color, and don't draw one on the page gray without labels.
