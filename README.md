# cargo-debug

A subcommand for cargo that launches the specified debugger on the output of a provided subcommand.

## Usage

Install with `cargo install cargo-debug`

- `cargo debug test` to run the test binary in a debugger
- `cargo debug --debugger=lldb build` to run the output binary in lldb
- `cargo debug test -- --all` to run the `cargo test` with the `--all` argument
- `cargo debug test -- -- --ignored` to run the test binary in the debugger with the `--ignored` argument
- `cargo debug --command-file=test.cmd build` to run the build binary in a debugger with the specified command file
- `cargo debug --filter=X --no-run test` to build cargo test, filter for the output binary starting with X, and output the debug command without running

## Status

[![GitHub tag](https://img.shields.io/github/tag/ryankurte/cargo-debug.svg)](https://github.com/ryankurte/cargo-debug)
[![Build Status](https://travis-ci.com/ryankurte/cargo-debug.svg?branch=master)](https://travis-ci.com/ryankurte/cargo-debug)
[![Crates.io](https://img.shields.io/crates/v/cargo-debug.svg)](https://crates.io/crates/cargo-debug)
[![Docs.rs](https://docs.rs/cargo-debug/badge.svg)](https://docs.rs/cargo-debug)

[Open Issues](https://github.com/ryankurte/cargo-debug/issues)

