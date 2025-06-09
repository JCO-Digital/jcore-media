# JCORE Media

JCORE Media is a collection of SCSS mixins designed to simplify responsive design by handling CSS breakpoints in your stylesheets. It provides a set of breakpoint variables and mixins for targeting different screen sizes, making it easy to write maintainable and scalable responsive styles.

## Features

- Predefined breakpoint map for common device widths (xs, sm, md, lg, xl, xxl)
- `breakpoint` mixin for targeting a minimum width
- `breakpoint-only` mixin for targeting a specific breakpoint range
- Built with modern SCSS and compatible with most build tools

## Installation

```sh
pnpm add @jcodigital/jcore-media
# or
npm install @jcodigital/jcore-media
# or
yarn add @jcodigital/jcore-media
```

## Usage

Import the SCSS file and use the mixins in your styles:

```scss
@use "@jcodigital/jcore-media/src/media.scss" as media;

.my-class {
  color: red;

  @include media.breakpoint(md) {
    color: blue;
  }

  @include media.breakpoint-only(lg) {
    color: green;
  }
}
```

## Breakpoints

The following breakpoints are available:

| Name | Width   |
|------|---------|
| xs   | 0       |
| sm   | 360px   |
| md   | 768px   |
| lg   | 992px   |
| xl   | 1200px  |
| xxl  | 1536px  |

## License

GPL-3.0-or-later

