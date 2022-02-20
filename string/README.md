# String

The utilities for manage string.

## Usage

```scss
@use "@unsass/utilities/string";
```

## API

### Sass functions

| Function  | Description                           |
|-----------|---------------------------------------|
| `replace` | Return value with replacement option. |

#### Replace string with `string.replace()`

The following Sass will produce:

```scss
@use "@unsass/utilities/string";

$key: "#{string.replace(test, e)}";
// tst
```
