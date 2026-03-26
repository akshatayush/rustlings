# [Rustlings](https://rustlings.rust-lang.org/) 🦀

Rustlings is a collection of exercises that teaches you the fundamentals of reading and writing [Rust](https://rust-lang.org/) code. It's an alternative to [Rust by Example](https://doc.rust-lang.org/rust-by-example/) that works with your own environment. This is my work-through of the Rustlings course, that I used to supplement the [Official Rust Book](https://doc.rust-lang.org/book/) for a more hands-on approach to learning. Because as pleasurable it is to read this extremely well written book, reading hundreds of pages of dense documentation is not my jam.

## Quick start

*Ensure the Rust tool-chain is installed. [duh](https://rust-lang.org/tools/install/)...*

```bash
rustup toolchain install stable   # Install rust tool-chain
cargo install rustlings           # Cargo is installed with the tool-chain
```

<a name="tip-anchor"></a>
> [!TIP]
> Adding [`CARGO_HOME`](https://doc.rust-lang.org/cargo/guide/cargo-home.html) to your `PATH` environment variable will allow you to use programs installed via cargo as commands on your CLI.

```bash
export $PATH="$HOME/.cargo/bin:$PATH"
```

*Finally[^1]...*
```bash
rustlings init  # Creates a directory named rustlings
cd rustlings    # Move into new directory
rustlings       # Start the watch daemon
```

## How it works

- Running the `rustlings` command will open a watch daemon that'll watch the current unsolved exercise for compiler errors and warnings.
- Open the current exercise in a text editor of your choice and complete the `TODO`'s to remove any compiler errors and panics.
- The daemon watches the file for any newly saved changes and recompiles the program automatically.
- The exercise is complete when the program compiles without any errors or warnings.

## Exercise to Book Chapter mapping

| Exercise               | Book Chapter        |
| ---------------------- | ------------------- |
| variables              | §3.1                |
| functions              | §3.3                |
| if                     | §3.5                |
| primitive_types        | §3.2, §4.3          |
| vecs                   | §8.1                |
| move_semantics         | §4.1-2              |
| structs                | §5.1, §5.3          |
| enums                  | §6, §18.3           |
| strings                | §8.2                |
| modules                | §7                  |
| hashmaps               | §8.3                |
| options                | §10.1               |
| error_handling         | §9                  |
| generics               | §10                 |
| traits                 | §10.2               |
| lifetimes              | §10.3               |
| tests                  | §11.1               |
| iterators              | §13.2-4             |
| smart_pointers         | §15, §16.3          |
| threads                | §16.1-3             |
| macros                 | §20.5               |
| clippy                 | Appendix D          |
| conversions            | n/a                 |

[^1]: If it wasn't *finally* for you :(, try following the [tip](#tip-anchor)
