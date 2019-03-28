Monocerus Engine
================

**Monocerus** is a lightweight, multi-platform, multi-architecture emulator
framework for smart contracts of blockchain platforms, and beyond.

Monocerus offers some key features:

- Emulate smart contract's byte-code, that requires no source code.
- Muli-platform: native build for Windows & \*nix (with Mac OSX, Linux,
  \*BSD & Solaris confirmed).
- Clean/simple/lightweight/intuitive blockchain-neutral API.
- Implemented in pure C language, with (future) support for bindings of other languages.
- Allow fine-grained instrumentation, with user-customized callbacks.
- Thread-safe by design.
- Open source with permissive license

Further information is available at http://www.groundx.io/monocerus


Code release
------------

To be publish in early **April 2019** - stay tuned!


Compilation
-----------

See [COMPILE](docs/COMPILE.md) for how to compile Monocerus.


mndebug
-------

Run in non-interactive mode, and default function selector:

```
$ ./mndebug -t -f ../samples/sample_evm.bin
```

To trace with a function seletor:

```
$ ./mndebug -t -f ../samples/out/sample.bin-runtime -s 8f33ea2d
```

Interactive mode:

```
$ ./mndebug -f ../samples/reentrancy-victim.bin -i -s d0e30db0

> selector d0e30db0
> callvalue deadbeef
> r

> selector 3ccfd60b
> callvalue 0
> r
```

Contact
-------

Contact us via mailing list, email or twitter for any questions.
