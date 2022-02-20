# String

The utilities for manage string.

## Usage

```scss
@use "@unsass/utilities/strip";
```

## API

### Sass functions

| Function | Description                    |
|----------|--------------------------------|
| `unit`   | Return value without the unit. |

#### Strip unit value with `strip.unit()`

The following Sass will produce:

```scss
@use "@sass-collective/strip-unit";

$value: strip.unit(100px);
// 100
```
