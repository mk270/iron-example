Example iron app
================

To use:

1. Ensure toolchain is up-to-date
2. Build
3. Run and test

Keeping up-to-date
------------------

You will need to be up-to-date with Rust and [Cargo](http://crates.io). 
These tools change daily, and normally a very recent version of both is 
required. 

Building
--------

    cargo build

Run and test
------------

    cargo run

This command will start an HTTP server on http://localhost:3000/ and not
terminate. Separately, you should do something like

    curl http://localhost:3000/

and this should display the string "Hello, world!"
