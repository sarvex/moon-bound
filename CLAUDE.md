# MoonBound Development Guide

## Build and Run Commands
- `cargo build` - Build the project
- `cargo run` - Run the project
- `cargo build --release` - Build for release
- `cargo clippy` - Run linter
- `cargo test` - Run all tests
- `cargo test test_name` - Run a single test
- `cargo test -- --nocapture` - Run tests with output visible

## End-to-end Testing
- `cd end2end && npx playwright test` - Run E2E tests

## Code Style Guidelines
- **Imports**: Group external crates first, then internal modules
- **Formatting**: 4-space indentation, 100-column width
- **Types**: Leverage Rust's type system fully with explicit types where helpful
- **Naming**: PascalCase for types/components, snake_case for functions/variables
- **Error Handling**: Use Result for recoverable errors, expect/unwrap sparingly
- **Documentation**: Document public APIs with /// comments
- **Components**: Use the #[component] attribute for Leptos components
- **State Management**: Use signals for reactive state (create_signal, create_rw_signal)

## Project Structure
- `src/` - Application code
- `style/` - SCSS styling
- `assets/` - Static assets
- `end2end/` - Playwright E2E tests