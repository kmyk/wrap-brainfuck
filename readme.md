# wrap-brainfuck

A tiny script wraps brainfuck code into C code (and the C code can be executed as a brainfuck code (polyglot), (thank you for [rdebath](https://github.com/rdebath))).

## how to use

``` sh
    $ wrap-brainfuck < a.bf > a.c
    $ gcc a.c # or submit it
```

## interpreter specification

-   EOF is `-1`
-   one cell is 1 byte (`char`).
-   overflow / underflow is possible.
-   the pointer can move indices out of memory, but the reading/writing depends the implementation of C compiler.
