Run natively:

`cargo run --features native`

Run on the web:

`cargo build --target wasm32-unknown-unknown --features web`
`wasm-bindgen --out-dir target --target web target/wasm32-unknown-unknown/debug/test_workspace.wasm`
`basic-http-server`

Open `http://localhost:4000/`