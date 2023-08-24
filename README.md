# About
Classic Unix command-line-tool `grep` in Rust 🦀

# Prerequites
You need to have `Rust` and `Cargo` installed on your system just like any Rust project. If it's your first time building on Rust,
you may refer the [docs](https://www.rust-lang.org/tools/install) for getting started.

# Description
This is a mini-version of the `grep` command used in Unix to search for `regex patterns` and `strings` by specifying them as
command line `arguments`, with `[options]` such as `IGNORE_CASE` and many more for a constrained query.

# Usage
The `minigrep` command-line utility can be used by the following line:

```
$ cargo run -- [pattern] [file]
```

Example:
```
$ cargo run -- to poem.txt
```

Output:
```
Are you nobody, too?
How dreary to be somebody!
```

You can specify `env`, like `IGNORE_CASE` for case-insensitive search:
```
$ IGNORE_CASE=1 cargo run -- to poem.txt
```

Output (case-insensitive):
```
Are you nobody, too?
How dreary to be somebody!
To tell your name the livelong day
To an admiring bog!
```

(To run tests, you can use `cargo test` if you feel like extending the tests for your version.)
