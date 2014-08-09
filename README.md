Example iron app
================

Overview
--------

[Iron](http://ironframework.io/) is a fast-developing HTTP framework
for Rust.  This repository contains a trivial self-contained example
of its use in an executable, suitable for cloning for your own
experiments.

The source code is in `src/main.rs`; its dependency on Iron is declared
through a stanza in the `Cargo.toml` file.

Usage
-----

1. Ensure toolchain is up-to-date
2. Build
3. Run and test


Keeping up-to-date
------------------

A lot of compilation errors are a direct result of not being up-to-date
with the latest versions of various tools.

You will need to be up-to-date with Rust and [Cargo](http://crates.io). 
These tools change daily, and normally a very recent version of both is 
required. Cargo is now bundled with Rust, and both may be updated with
the `rustup.sh' command. If you are not too security-conscious, you may
achieve this on a UNIX-like system with:

    curl www.rust-lang.org/rustup.sh | sudo sh

This will download and install the latest Rust and Cargo binaries into
/usr/local/bin.

Building
--------

    cargo build

The actual executable will be created in `target/iron-example`; you can run
this file directly.

Run and test
------------

    cargo run

This command will start an HTTP server on http://localhost:3000/ and not
terminate. Separately, you should do something like

    curl http://localhost:3000/

and this should display the string "Hello, world!"
