# c2rust_eval

This repo contains the results of evaluating [c2rust](https://c2rust.com) on a large number of open source Linux packages. For each package, we want to know:
- is the package a C or a C++ package.
- can the package be compiled with the clang compiler.
- does c2rust manage to generate rust files for each c file used in the build.
- does the resulting rust code build using `cargo build`.
- how many `error` and `warning` messages are generated when `cargo build`.
- how many `unsafe` statements are present in the generated rust code.
- are the errors fixable or is the translation incorrect.

## Results.md
This file contains the evaluation results of c2rust.

## Stats.md
Contains stats on the success rate of c2rust.

## Idioms.md
Contains the list of C functions that can be translated to idiomatic Rust and which one are challenging.
