# sfdisk-sort

This repository contains 2 programs - one is Go-based [`sfdisk-sort-go`](https://github.com/artnoi43/sfdisk-sort-go/), and the other is [`sfdisk-sort-rs`](https://github.com/artnoi43/sfdisk-sort-rs/) written in Rust.

The Go version is a one-file script, requiring 0 external dependency other than the Go programming language's standard library. The goal behind this is to make it very portable.

The Rust version has conservative source file layout, and requires `cargo` to get dependencies and compile.

## Getting the programs

The repositories for both `sfdisk-sort-go` and `sfdisk-sort-rs` are included here as submodules.

To init files from these repos _for the first time_, use:


```
$ git submodule update --init --recursive;
```

To pull changes from these repos, use:

```
$ # Git >= 1.8.2
$ git submodule update --recursive --remote;
$
$ # or you can use
$ git submodule update --recursive;
$
$ # or
$ git pull --recurse-submodules;
```

For more info on pulling git submodules, see this question from [StackOverflow](https://stackoverflow.com/questions/1030169/pull-latest-changes-for-all-git-submodules)
