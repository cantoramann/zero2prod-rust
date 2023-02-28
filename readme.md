# Zero to Production in Rust

## Inner Development Loop

### Faster Linking

- For faster linking, I am using `lzd` for Mac.

### cargo-watch

- `cargo watch -x check -x test -x run` for faster compilation during development.

### Continuous Integration

#### Tests

- `cargo test` for running tests.

#### Code Coverage

- `cargo tarpaulin --ignore-tests` for running code coverage.

#### Linting

- `cargo clippy -- -D warnings` for linting.

#### Formatting

- `cargo fmt -- --check` for formatting.

#### Security Vulnerabilities

- `cargo install cargo-audit` for installing `cargo-audit`.
- `cargo audit` for scanning the dependency tree for security vulnerabilities.

## Cargo Expand

`cargo expand` for expanding macros.

- `cargo install cargo-expand` for installing `cargo-expand`.
- `rustup toolchain install nightly --allow-downgrade` for installing nightly toolchain.
- `cargo +nightly expand` for expanding macros. This command uses the nightly build only for the `expand` command.
