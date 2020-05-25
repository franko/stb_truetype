stb truetype
============

truetype single-file public domain (or MIT licensed) library for C/C++, with a meson build.

This repository contains a copy of the stb_truetype code provided in:

https://github.com/nothings/stb/

but keep only the truetype file and provides meson based setup to install it as a standard library.
When installed a pkg-config file for the library will be provided.

All the credit goes to the original author of the stb libraries.

usage
-----

```sh
meson setup build
ninja -C build
ninja -C install
```

This repository was created to be used with the [Little library helper](https://github.com/franko/lhelper).
Using lhelper the install can be done, within an environment, using the command:

```sh
lhelper install stb_truetype
```

Once installed the software can be automatically discovered by other libraries using pkg-config.

To use with pkg-config:

```sh
pkg-config --cflags stb_truetype
pkg-config --libs stb_truetype
```

