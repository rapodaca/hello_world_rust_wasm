# Hello World with Rust and WebAssembly

This projects demonstrates two-way string passing between JavaScript and a WebAssembly instance compiled from Rust. Only the standard library is used. wasm-bindgen is not needed. Details about the approach can be found in *[Rust and WebAssembly from Scratch: Hello World with Strings](https://depth-first.com/articles/2020/07/07/rust-and-webassembly-from-scratch-hello-world-with-strings/)*.

The intent is to document with working code string message passing to help evaluate the need for more advanced tooling.

To build:

```bash
cargo build --target wasm32-unknown-unknown --release
```

Run a webserver, open the index.html page through it, and open a developer console. You should see the message: "greeting – "Hello, Satoshi!""