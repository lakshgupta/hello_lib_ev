# hello_lib_ev

An experimental Evryn project to use as a dependency.

## Overview

`hello_lib_ev` is a minimal library written in Evryn. It's intended as a
simple demonstration of packaging reusable code and publishing it for use in
other Evryn projects. The library currently exposes a single function that
returns a greeting string, making it a friendly starting point for learning
how to build and consume Evryn dependencies.

## Usage

Add `hello_lib_ev` as a dependency in your `evryn.toml`:

```toml
[dependencies]
hello_lib_ev = "*"
```

Then import and call the function in your Evryn source:

```ev
import hello_lib_ev;

fun main() -> void {
    hello_lib_ev.hello();
}
```

## Development

- Source files live under `src/` (currently `main.ev`).
- Tests can be added under the `tests/` directory.
- Build using `evryn build` (assuming the tooling is
  installed).

## License

This project is released under the MIT License. See [LICENSE](LICENSE) for
details.
