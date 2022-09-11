# Rust Repository Template 🦀
[![License](https://img.shields.io/badge/license-MIT-green)](./LICENSE)
[![CI](https://github.com/nlp-rs/rust-template/actions/workflows/main.yml/badge.svg)](https://github.com/nlp-rs/rust-template/actions/workflows/main.yml)
[![Security audit](https://github.com/nlp-rs/rust-template/actions/workflows/security-audit.yml/badge.svg)](https://github.com/nlp-rs/rust-template/actions/workflows/security-audit.yml)

Repository template to get quickly started with writing Rust libraries, ready for distributing.

## Features
 - [x] Remote development support with [GitHub Codespaces](https://github.com/features/codespaces)
 - [x] Debugging with the [LLDB Debugger](https://lldb.llvm.org/) tool in Visual Studio Code ([VSCode Marketplace](https://marketplace.visualstudio.com/items?itemName=vadimcn.vscode-lldb))
 - [x] Fuzz testing with LLVM's [libFuzzer](https://llvm.org/docs/LibFuzzer.html) tool and [`cargo fuzz`](https://github.com/rust-fuzz/cargo-fuzz) ([Reference](https://rust-fuzz.github.io/book/introduction.html))
 - [x] Performance benchmarks in Rust with Criterion and Iai (suitable to run in GitHub Actions CI environments)
 - [x] CI/CD support with [GitHub Actions](https://github.com/features/actions), allowing to automate:
   - [x] Running tests and benchmarks
   - [x] Running Rustfmt and Clippy for detecting formatting and linting errors, respectively
   - [x] Daily, midnight scheduled security audits of Rust packages with [`actions-rs/audit-check`](https://github.com/actions-rs/audit-check)
   - [ ] Generating performance benchmark graphs, auto-publishing to GitHub Pages
   - [ ] Documentation of API docs and mdBook using GitHub Pages
   - [ ] Semantic version bumping, `CHANGELOG.md` updates, and new package releases

## Configure
 - GitHub Codespaces: [`devcontainer.json`](./.devcontainer/devcontainer.json) ([Reference](https://containers.dev/implementors/json_reference/))
 - GitHub Action workflows: [`.github/workflows`](./.github/workflows) ([Reference](https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions))
 - Cargo package: [`Cargo.toml`](./Cargo.toml) ([Reference](https://doc.rust-lang.org/cargo/reference/manifest.html))
 - Clippy (Rust linter): [`.clippy.toml`](./.clippy.toml) ([Repository](https://github.com/rust-lang/rust-clippy), [Reference](https://rust-lang.github.io/rust-clippy/))
 - Rustfmt (Rust formatter): [`.rustfmt.toml`](./.rustfmt.toml) ([Repository](https://github.com/rust-lang/rustfmt), [Reference](https://rust-lang.github.io/rustfmt/))

----

# {{library}}
{{library description}}

## Install
```shell
cargo add {{library}}
```

## License
This software is openly licensed and distributed under the [MIT License](./LICENSE).

## Contribution
Unless you explicitly state otherwise, any contribution intentionally submitted for inclusion in the work by you, as defined in the MIT license, shall be licensed as above, without any additional terms or conditions.
