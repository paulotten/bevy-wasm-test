# Prerequisites

[Install Rust](https://www.rust-lang.org/tools/install)

    rustup target add wasm32-unknown-unknown

    cargo install wasm-pack

# Compiling

    wasm-pack build --target web --release

If you run into https://github.com/bevyengine/bevy/issues/3099 then do

    cargo update -p tracing-wasm --precise 0.2.0

# Running locally

    wasm-pack build --target web --release

Open http://127.0.0.1:8000/pkg/ in a web browser.
