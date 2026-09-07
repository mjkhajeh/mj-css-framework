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
<section class="mj df ai-c jc-sb g-16 pinline-20 pblock-12">
  <h1 class="mj mblock-0">Dashboard</h1>
  <button class="mj br-8 pinline-12 pblock-8">Open</button>
</section>
```

Most utilities are scoped to an element carrying `mj`. For example, `mj df` sets `display: flex`, while `mj g-16` sets `gap: 16px`. The `screen-reader-text` helper targets a descendant of an `mj` element.

## Utility groups

| Group | Examples | Purpose |
| --- | --- | --- |
| Display | `df`, `dg`, `dn` | Flex, grid, and hidden display modes |
| Alignment | `ai-c`, `jc-c`, `jc-sb` | Flex and grid alignment |
| Centering | `center` | Sets `place-items: center` |
| Grid | `g-t-c-1` … `g-t-c-4` | One-to-four equal grid columns |
| Gaps | `g-0` … `g-20`, `g-r-*`, `g-c-*` | Gap, row-gap, and column-gap |
| Margins | `mt-*`, `mb-*`, `m-block-*`, `m-inline-*` | Directional and logical margins |
| Padding | `pt-*`, `pb-*`, `p-block-*`, `p-inline-*` | Directional and logical padding |
| Border radius | `br-2` … `br-32`, `br-pill`, `br-circle` | Rounded corners and shapes |
| Colors | `color-white`, `color-black`, `color-h-white`, `color-h-black` | Text colors and hover colors |
| Size | `w-*`, `h-*` | Width and height utilities |
| Position | `pos-*`, `t-*`, `b-*`, `s-*`, `e-*`, `ii-*`, `ib-*`, `i-*` | Positioning and inset values |
| Z-index | `z-a`, `z-0` … `z-3`, `z--1` … `z--3` | Stacking order utilities |
| Opacity | `o-0`, `o-10`, `o-50`, `o-100` | Opacity presets |
| Transitions | `tr-all` | A short all-property transition |
| Borders | `border-t`, `border-h-t` | Transparent borders and hover borders |
| Font sizes | `fs-10` … `fs-48` | Rem-based font-size presets |
| Font weights | `fw-100` … `fw-900` | Numeric font-weight presets |
| Line height | `lh-1` | Line-height presets |
| Backgrounds | `back-t`, `back-w`, `back-b` | Transparent, white, and black backgrounds |
| Overflow | `over-a`, `over-h` | Auto and hidden overflow behavior |
| Text alignment | `texta-s`, `texta-c`, `texta-e` | Start, center, and end text alignment |
| Line clamps | `line-clamp`, `line-clamp-1` … `line-clamp-3` | Multi-line truncation helpers |
| White space | `white-space-nowrap` | Prevents text wrapping |
| Box shadow | `bs-n` | Removes the box shadow |
| Aspect ratio | `ar-1` | Sets a square aspect ratio |
| Box sizing | `bsize-bb` | Uses `border-box` sizing |
| Interaction | `p-event-n`, `disabled` | Disables pointer and touch interaction |
| Accessibility | `screen-reader-text` | Visually hides content while keeping it available to screen readers |

Most numeric utilities use the value in the class name as pixels. For example, `mj mt-16` produces `margin-top: 16px`, and `mj w-48` produces `width: 48px`. Logical properties such as `mblock-*` and `pinline-*` help the same markup work across writing directions.

## Browser support

The stylesheet uses modern CSS features including logical properties, dynamic viewport units, and `inset`. Choose a browser support target appropriate for your application if you extend or transpile the source.

## License

This project is licensed under the MIT License. See the LICENSE file or [MIT License](https://opensource.org/licenses/MIT) for details.
