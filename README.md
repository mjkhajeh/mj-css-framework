# MJ CSS Framework

A lightweight, Sass-powered CSS utility library. Utilities are composed with the `mj` namespace, making it possible to describe common layout, spacing, sizing, positioning, and visual properties directly in an element's class list.

## Files

- `styles.scss` — readable Sass source and the place to add or change utilities.
- `styles.min.css` — compressed CSS build for use in a browser.

## Usage

Include the compiled stylesheet in your page:

```html
<link rel="stylesheet" href="styles.min.css">
```

Apply utilities by combining the `mj` namespace with one or more utility names:

```html
<section class="mj df ai-c jc-sb g-16 p-inline-20 p-block-12">
  <h1 class="mj m-block-0">Dashboard</h1>
  <button class="mj br-8 p-inline-12 p-block-8">Open</button>
</section>
```

Most utilities are scoped to an element carrying `mj`. For example, `mj df` sets `display: flex`, while `mj g-16` sets `gap: 16px`.

## Utility reference

Every utility is scoped to an element carrying the `mj` class, so `df` is used as `class="mj df"`.

| Group | Utilities | Purpose |
| --- | --- | --- |
| Display | `df`, `dn`, `dg` | Flex, grid, and hidden display modes |
| Alignment | `ai-c`, `jc-c`, `jc-sb`, `center` | Flex and grid alignment |
| Flex | `flex-w`, `flex-w-n`, `flex-dir-c`, `flex-dir-r`, `flex-a`, `flex-1` | Flex wrapping, direction, and sizing utilities |
| Grid columns | `g-t-c-1`, `g-t-c-2`, `g-t-c-3`, `g-t-c-4` | One-to-four equal grid columns |
| Cells | `cell-1` | Places an item in the first grid row and column |
| Gaps | `g-0`, `g-2`, `g-4`, `g-6`, `g-8`, `g-10`, `g-12`, `g-16`, `g-20` | Gap, row-gap, and column-gap |
| Row gap | `g-r-0`, `g-r-2`, `g-r-4`, `g-r-6`, `g-r-8`, `g-r-10`, `g-r-12`, `g-r-16`, `g-r-20` | Row spacing for flex and grid layouts |
| Column gap | `g-c-0`, `g-c-2`, `g-c-4`, `g-c-6`, `g-c-8`, `g-c-10`, `g-c-12`, `g-c-16`, `g-c-20` | Column spacing for flex and grid layouts |
| Margin | `m-a`, `m-0`, `m-2`, `m-4`, `m-6`, `m-8`, `m-10`, `m-12`, `m-16`, `m-20`, `m-24` | Directional and logical margins |
| Margin top | `mt-a`, `mt-0`, `mt-4`, `mt-8`, `mt-12`, `mt-16`, `mt-20` | Controls the top margin |
| Margin bottom | `mb-a`, `mb-0`, `mb-4`, `mb-8`, `mb-12`, `mb-16`, `mb-20` | Controls the bottom margin |
| Margin block | `m-block-a`, `m-block-0`, `m-block-4`, `m-block-8`, `m-block-12`, `m-block-16`, `m-block-20` | Controls the block-axis margins |
| Margin inline | `m-inline-a`, `m-inline-0`, `m-inline-4`, `m-inline-8`, `m-inline-12`, `m-inline-16`, `m-inline-20` | Controls the inline-axis margins |
| Padding | `p-0`, `p-2`, `p-4`, `p-6`, `p-8`, `p-10`, `p-12`, `p-16`, `p-20`, `p-24` | Directional and logical padding |
| Padding top | `pt-a`, `pt-0`, `pt-4`, `pt-8`, `pt-12`, `pt-16`, `pt-20` | Controls the top padding |
| Padding bottom | `pb-a`, `pb-0`, `pb-4`, `pb-8`, `pb-12`, `pb-16`, `pb-20` | Controls the bottom padding |
| Padding block | `p-block-a`, `p-block-0`, `p-block-4`, `p-block-8`, `p-block-12`, `p-block-16`, `p-block-20` | Controls the block-axis padding |
| Padding inline | `p-inline-a`, `p-inline-0`, `p-inline-4`, `p-inline-8`, `p-inline-12`, `p-inline-16`, `p-inline-20` | Controls the inline-axis padding |
| Border radius | `br-2`, `br-4`, `br-8`, `br-12`, `br-16`, `br-20`, `br-24`, `br-32`, `br-pill`, `br-circle` | Rounded corners and shapes |
| Text color | `color-fff`, `color-white`, `color-h-white`, `color-000`, `color-black`, `color-h-black` | Text colors and hover colors |
| Width | `w-a`, `w-fit`, `w-full`, `w-100`, `w-100dvw`, `w-95dvw`, `w-90dvw`, `w-16`, `w-20`, `w-24`, `w-32`, `w-36`, `w-48`, `w-64` | Width utilities |
| Height | `h-a`, `h-full`, `h-100`, `h-100dvw`, `h-95dvw`, `h-90dvw`, `h-16`, `h-20`, `h-24`, `h-32`, `h-36`, `h-48`, `h-64` | Height utilities |
| Position | `pos-r`, `pos-a`, `pos-f`, `pos-s` | Positioning values |
| Top | `t-a`, `t-0`, `t-2`, `t-4`, `t-6`, `t-8`, `t-12`, `t-16`, `t-20` | Top position values |
| Bottom | `b-a`, `b-0`, `b-2`, `b-4`, `b-6`, `b-8`, `b-12`, `b-16`, `b-20` | Bottom position values |
| Inline-start | `s-a`, `s-0`, `s-2`, `s-4`, `s-6`, `s-8`, `s-12`, `s-16`, `s-20` | Inline start position values |
| Inline-end | `e-a`, `e-0`, `e-2`, `e-4`, `e-6`, `e-8`, `e-12`, `e-16`, `e-20` | Inline end position values |
| Inline inset | `ii-a`, `ii-0`, `ii-2`, `ii-4`, `ii-6`, `ii-8`, `ii-12`, `ii-16`, `ii-20` | Inset inline position values |
| Block inset | `ib-a`, `ib-0` | Inset block position values |
| Inset | `i-a`, `i-0`, `i-2`, `i-4` | Inset position values |
| Z-index | `z-a`, `z-0`, `z-1`, `z-2`, `z-3`, `z--1`, `z--2`, `z--3` | Stacking order utilities |
| Opacity | `o-0`, `o-10`, `o-50`, `o-1`, `o-100` | Opacity presets |
| Transition | `tr-all` | A short all-property transition |
| Border | `border-t`, `border-transparent`, `border-h-t`, `border-h-transparent` | Borders utilities |
| Font size | `fs-10`, `fs-12`, `fs-14`, `fs-16`, `fs-18`, `fs-20`, `fs-24`, `fs-32`, `fs-48` | Rem-based font-size presets |
| Font weight | `fw-100`, `fw-200`, `fw-300`, `fw-400`, `fw-500`, `fw-600`, `fw-700`, `fw-800`, `fw-900` | Numeric font-weight presets |
| Line height | `lh-1` | Line-height presets |
| Background | `back-t`, `b-transparent`, `back-w`, `b-white`, `back-b`, `b-black` | Transparent, white, and black backgrounds |
| Overflow | `over-a`, `over-h` | Auto and hidden overflow behavior |
| Text alignment | `texta-s`, `texta-c`, `texta-e` | Start, center, and end text alignment |
| Line clamp | `line-clamp`, `line-clamp-1`, `line-clamp-2`, `line-clamp-3` | Multi-line truncation helpers |
| White space | `white-space-nowrap` | Prevents text wrapping |
| Box shadow | `bs-n` | Removes the box shadow |
| Aspect ratio | `ar-1` | Sets a square aspect ratio |
| Box sizing | `bsize-bb` | Uses `border-box` sizing |
| Interaction | `p-event-n`, `disabled` | Disables pointer and touch interaction |
| Accessibility | `screen-reader-text` | Visually hides content while keeping it available to screen readers |

### Flex, cell, and hover utilities

| Utility | Description |
| --- | --- |
| `flex-w` | Sets `flex-wrap: wrap`, allowing flex items to move onto multiple lines. |
| `flex-w-n` | Sets `flex-wrap: nowrap`, keeping flex items on a single line. |
| `flex-dir-c` | Sets `flex-direction: column`. |
| `flex-dir-r` | Sets `flex-direction: row`. |
| `flex-a` | Sets `flex: auto`. |
| `flex-1` | Sets `flex: 1`, allowing an item to grow and share available space. |
| `cell-1` | Places a grid item in grid row 1 and grid column 1. |
| `color-h-white` | Applies white text color when the `mj` element is hovered. |
| `color-h-black` | Applies black text color when the `mj` element is hovered. |
| `border-h-t` | Applies a transparent border color when the `mj` element is hovered. |
| `border-h-transparent` | Applies a transparent border color when the `mj` element is hovered. |

Numeric utilities use the value in the class name as pixels unless otherwise noted. For example, `mj mt-16` produces `margin-top: 16px`, and `mj w-48` produces `width: 48px`. The `a` value means `auto`; it is primarily useful for margin and positioning utilities. Logical properties such as `m-block-*` and `p-inline-*` work across writing directions.

## Browser support

The stylesheet uses modern CSS features including logical properties, dynamic viewport units, and `inset`. Choose a browser support target appropriate for your application if you extend or transpile the source.

## License

This project is licensed under the MIT License. See the LICENSE file or [MIT License](https://opensource.org/licenses/MIT) for details.
