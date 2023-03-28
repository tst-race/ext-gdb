# GDB for RACE

This repo provides scripts to custom-build the
[GDB tool](https://www.sourceware.org/gdb/) for RACE.

## License

The GDB tool is licensed under the GPL license.

Only the build scripts in this repo are licensed under Apache 2.0.

## Dependencies

GDB has no dependencies on any custom-built libraries.

## How To Build

The [ext-builder](https://github.com/tst-race/ext-builder) image is used to
build GDB.

```
git clone https://github.com/tst-race/ext-builder.git
git clone https://github.com/tst-race/ext-gdb.git
./ext-builder/build.py \
    --target linux-x86_64 \
    ./ext-gdb
```

## Platforms

GDB is built for the following platforms:

* `linux-x86_64`
* `linux-arm64-v8a`

## How It Is Used

GDB is used included in the development RACE images for debugging.
