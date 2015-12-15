# Tee

[![Build Status](https://travis-ci.org/softprops/tee.svg)](https://travis-ci.org/softprops/tee)

A rustlang adapter for readers which delegate read bytes to a writer, adapted from the standard library's `std::io::Read#tee` which has since been deprecated.

## api docs

rustdoc api documentation can be found [here](https://softprops.github.io/tee)

## examples

The currently unstable/deprecated std library function looks like this

```rust
let tee_reader = reader.tee(writer)
```

In broadcast this looks like

```rust
let tee_reader = tee::Tee::new(reader, writer)
```

Doug Tangren (softprops) 2015
