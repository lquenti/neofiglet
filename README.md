# neofiglet

[![docs](https://docs.rs/neofiglet/badge.svg)](https://docs.rs/neofiglet)
[![crates.io](https://img.shields.io/crates/v/neofiglet.svg)](https://crates.io/crates/neofiglet)

The [FIGlet](http://www.figlet.org/) library all the cool kids use!

# Note (Pretty important)

This is currently in a full rewrite since this is easier than hack good kerning into this version. (See [#3](https://github.com/lquenti/neofiglet/issues/3))

Therefore, the API __will__ completely break within the next few weeks as I will release a `1.0.0`.

I mean, this is not a problem as this version is feature-complete, just that if you can wait a few weeks... good stuff will come.

# Example

```rust
use neofiglet::FIGfont;

fn main() {
    let standard_font = FIGfont::standard().unwrap();
    let figure = standard_font.convert("Hello Rust");
    assert!(figure.is_some());
    println!("{}", figure.unwrap());
}
```

![figlet-sample](./figlet-sample.png)

# License

neofiglet is based on [figlet-rs](https://crates.io/crates/figlet-rs), which sadly is not maintained anymore.

rs-figlet is distributed under the terms of the Apache License (Version 2.0).

See [LICENSE](LICENSE) and [COPYRIGHT](COPYRIGHT) for details.
