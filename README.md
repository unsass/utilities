# Utilities

[![Version](https://flat.badgen.net/npm/v/@unsass/utilities)](https://www.npmjs.com/package/@unsass/utilities)
[![Download](https://flat.badgen.net/npm/dt/@unsass/utilities)](https://www.npmjs.com/package/@unsass/utilities)

## Install

```shell
npm install @unsass/utilities
```

## Usage

```scss
@use "@unsass/utilities";
```

## API

### Sass mixins

| Mixin            | Description                    |
|------------------|--------------------------------|
| `ellipsis`       | Sets the ellipsis rules.       |
| `font-smoothing` | Sets the font smoothing rules. |

#### Ellipsis rule with `utilities.ellipsis()`

The following Sass...

```scss
@use "@unsass/utilities";

.foo {
    @include utilities.ellipsis;
}
```

...will produce the following CSS...

```css
.foo {
    -moz-osx-font-smoothing: grayscale;
    -webkit-font-smoothing: antialiased;
}
```

#### Ellipsis rule with `utilities.font-smoothing()`

The following Sass...

```scss
@use "@unsass/utilities";

.foo {
    @include utilities.font-smoothing;
}
```

...will produce the following CSS...

```css
.foo {
    text-overflow: ellipsis;
    white-space: nowrap;
    overflow: hidden;
}
```

### Sass functions

| Function                                     | Description                           |
|----------------------------------------------|---------------------------------------|
| `string-replace($string, $search, $replace)` | Return value without the unit.        |
| `strip-unit($value)`                         | Return value with replacement option. |


## Components

| Component            | Description                     | Sass `@use` prefix   |
|----------------------|---------------------------------|----------------------|
| [`string`](./string) | Utilities functions for string. | `utilities.string-*` |
| [`strip`](./strip)   | Utilities functions for strip.  | `utilities.strip-*`  |
