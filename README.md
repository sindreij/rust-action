# Rust Github Action

'Silverbullet' for a quickstart Rust CI based upon [Github Actions](https://developer.github.com/actions/)

*What's inside the "box":*

* Rust
* Rustfmt
* Clippy
* Cargo Release

# Usage

```
workflow "Quickstart" {
  on = "push"
  resolves = ["Quickstart"]
}

action "Quickstart" {
  uses = "icepuma/rust-action@master"
  args = "cargo fmt -- --check && cargo clippy -- -Dwarnings && cargo test"
}
```
