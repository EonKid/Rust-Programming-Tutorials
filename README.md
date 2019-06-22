# Rust-Programming-Tutorials
Rust programming language tutorials for beginners

# Installing rustup on Linux or macOS:

$ curl https://sh.rustup.rs -sSf | sh

Success : Rust is installed now. Great!

# Add to sytem PATH:

$ source $HOME/.cargo/env or $ export PATH="$HOME/.cargo/bin:$PATH"

# Get vesion:

$ rustc --version

# Creating Project directory:

$ mkdir ~/projects

$ cd ~/projects

$ mkdir hello_world

$ cd hello_world

# Writing and Running a Rust Program

Filename: main.rs

        fn main() {
            println!("Hello, world!");
        }

$ rustc main.rs

$ ./main

Hello, world!

# Compiling and Running Are Separate Steps

    $ rustc main.rs

    $ ls

    main  main.rs

    $ ./main # or .\main.exe on Windows


# Creating a Project with Cargo

    $ cargo new hello_cargo

    $ cd hello_cargo

TOML (Tom’s Obvious, Minimal Language) format, which is Cargo’s configuration format.

# Building and Running a Cargo Project

$ cargo build

    Compiling hello_cargo v0.1.0 (file:///projects/hello_cargo)
    Finished dev [unoptimized + debuginfo] target(s) in 2.85 secs
    $ ./target/debug/hello_cargo # or .\target\debug\hello_cargo.exe on Windows
    Hello, world!

$ cargo run


    Finished dev [unoptimized + debuginfo] target(s) in 0.0 secs
     Running `target/debug/hello_cargo`

Hello, world!

$ cargo check


    Checking hello_cargo v0.1.0 (file:///projects/hello_cargo)
    Finished dev [unoptimized + debuginfo] target(s) in 0.32 secs


# Building for Release

    cargo build --release

# Cargo as Convention

    $ git clone someurl.com/someproject

    $ cd someproject

    $ cargo build


