# neofiglet

The [FIGlet](http://www.figlet.org/) library all the cool kids use!

# Example

```rust
use neofiglet::FIGfont;

fn main() {
    let standard_font = FIGfont::standand().unwrap();
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
