# GBA Makefile Template

This repository provides a solid template Makefile for GBA development with
devkitARM, supporting C, C++, and Assembly.

## Usage

- Modify the options inside `Makefile` to suit your needs, and run `make`.
- To get verbose output, run `make V=1` or `make VERBOSE=1`.
- To run a clean build, run `make -B`

build.mk contains all of the build code, and you usually don't need to touch it
at all.

## Features

- Soundbank creation with mmutil
- Graphics processing with grit
- Binary conversion with bin2s
- Use of relative and symlinked file paths (../etc/hi.c)
- Creating a multiboot build by adding `_mb` suffix to project name
- `*.iwram.ext`, `*.arm.ext`, and `*.thumb.ext` filenames override ARM/THUMB code
- Building with LTO
- Specifying title, game code, etc. for gbafix
- Running ROM in mGBA (by default) via `make run`

## License

Repository is licensed under the [CC0 1.0 Universal License][CC0].

[CC0]: https://creativecommons.org/publicdomain/zero/1.0/
