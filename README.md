rlibc
=====
[![Build Status](https://travis-ci.org/RustyGecko/rlibc.svg)](https://travis-ci.org/RustyGecko/rlibc)

*This is a fork of Rust's rlibc crate in order to get rlibc for the `thumbv7m-none-eabi` target.*

A bare minimum "libc" for Rust crates that do not want to rely on libc itself.
This crate provides functions which LLVM often lowers intrinsic calls to and
will be required to link correctly.

## Usage

Add this to your `Cargo.toml`:

```toml
[dependencies]

rlibc = "*"
```

And add this to your crate root:

```rust
extern crate rlibc;
```
