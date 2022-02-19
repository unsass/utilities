# String

The utilities for manage string.

## Usage

```scss
@use "@unsass/utilities/string";
```

## API

### Sass functions

| Mixin     | Description              |
|-----------|--------------------------|
| `replace` | Sets string replacement. |

#### Replace string with `string.replace()`

The following Sass...

```scss
@use "@unsass/utilities/string";

$key: "#{string.replace(test, e)}";
```

...will produce the following CSS...

```scss
$key: "tst";
```
