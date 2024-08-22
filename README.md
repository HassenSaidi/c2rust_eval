# c2rust_eval
Evaluation of the c2rust tool on a large number of open source projects.



This repo contains the results of evaluating [c2rust](https://c2rust.com) on a large number of open source Linux packages. For each package, we want to know:
- is the package a C or a C++ package.
- can the package be compiled with the clang compiler
- does c2rust manage to generate rust files for each c file used in the build.
- does the resulting rust code build using `cargo build`.
- how many `error` and `warning` messages are generated.
- how many `unsafe` are used in the generated code.
- are the errors fixable or is the translation incorrect.
- can we improve the readability of the produced rust code and make it more idiomatic than what c2rust produces.
