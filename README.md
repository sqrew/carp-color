# carp-color

A graphics-oriented color library for the [Carp language](https://github.com/carp-lang/Carp).

## Features

- **RGB & RGBA Support:** Precise `Double` based color representation.
- **HSL Color Space:** Full support for HSL with robust RGB <-> HSL conversions.
- **Manipulation:** Helpers for `lighten`, `darken`, `saturate`, `desaturate`, and `lerp`.
- **Hex Strings:** Parse from and format to standard hex codes (e.g., `#ff0000`).
- **Byte Helpers:** Easy conversion to/from 0-255 byte ranges for interoperability with SDL, OpenGL, etc.

## Installation

Add this to your project by loading `color.carp`.

```clojure
(load "path/to/carp-color/color.carp")
(use Color)
```

## Running Tests

```bash
carp -x test/color_test.carp
```

## License

MIT
