# Utilities

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
