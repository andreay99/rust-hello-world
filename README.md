# Rust Hello World

Assignment: set up a Rust toolchain, compile "Hello World", and publish it to GitHub.

## Environment

| Tool | Version |
| --- | --- |
| rustc | 1.98.0 |
| cargo | 1.98.0 |
| VS Code | with the `rust-analyzer` extension |

Rust was installed with [rustup](https://www.rust-lang.org/tools/install):

```sh
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

## Two ways to compile

### 1. With `rustc` directly

[`hello.rs`](hello.rs) is the standalone program from
[Rust by Example](https://doc.rust-lang.org/rust-by-example/hello.html):

```sh
rustc hello.rs
./hello
# Hello World!
```

### 2. With Cargo

[`src/main.rs`](src/main.rs) is the binary crate created by `cargo new`:

```sh
cargo run
# Hello, world!
```

`cargo build` alone puts the executable at `target/debug/rust-hello-world`.

## Opening this in VS Code

```sh
code .
```

VS Code will suggest the `rust-analyzer` extension, which is recommended in
[`.vscode/extensions.json`](.vscode/extensions.json). It provides completion,
inline type hints, and Run/Debug buttons above `fn main()`.
