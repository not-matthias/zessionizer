# Contributing to Zessionizer

Thank you for your interest in contributing to Zessionizer!

## Code of Conduct

This project adheres to a Code of Conduct that all contributors are expected to follow. Please read [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) before contributing.

## How Can I Contribute?

### Reporting Bugs

Before creating bug reports, please check existing issues to avoid duplicates. When creating a bug report, include:

- **Clear title and description**
- **Steps to reproduce** the behavior
- **Expected behavior** vs actual behavior
- **Environment details**: Zellij version, OS, terminal emulator
- **Relevant logs** from `~/.local/share/zellij/zessionizer/zessionizer-otlp.json`

### Suggesting Features

Feature requests are welcome! Please:

- **Check existing issues** to avoid duplicates
- **Describe the feature** and its use case clearly
- **Explain why** this feature would be useful
- **Provide examples** of how it would work

### Pull Requests

1. **Fork the repository** and create your branch from `main`
2. **Follow the coding style** (run `make clippy`)
3. **Write clear commit messages** following [Conventional Commits](https://www.conventionalcommits.org/):
   - `feat:` for new features
   - `fix:` for bug fixes
   - `docs:` for documentation changes
   - `refactor:` for code refactoring
   - `chore:` for maintenance tasks
4. **Update CHANGELOG.md** under "Unreleased" section if needed
5. **Ensure the build passes**: `make build` and `make clippy`
6. **Open a Pull Request** with a clear description

## Development Setup

### Prerequisites

- Rust 1.70 or later
- Zellij 0.40.0 or later
- WASM target: `rustup target add wasm32-wasip1`

### Building

```bash
# Clone your fork
git clone https://github.com/YOUR_USERNAME/zessionizer.git
cd zessionizer

# Build the plugin
make build

# Run clippy linting
make clippy

# Check available make commands
make help
```

### Testing Locally

```bash
# Install to local Zellij plugins directory
make install

# Then restart Zellij or reload the plugin
```

## Coding Guidelines

- Use `make clippy` before committing
- Add documentation comments (`///`) for public APIs
- Keep functions focused and reasonably sized
- Follow existing code patterns

## Questions?

Open an issue for questions or check existing issues and discussions.

Thank you for contributing! 🎉
