These toolchains were built using crosstool-ng commit #358945ff2219e37d280532522d2c62309614d162 in a Debian 11 container.

Both the crosstool-ng config files and sources used to build them are included in the repo.

The toolchains are fully statically linked,
and should therefore work on any aarch64 or x86_64 Linux or MacOS box with a reasonably recent kernel.

Currently, the build system is not smart enough to choose the correct toolchain.
Instead, it's up to you to modify the 2 top-level symlinks appropriately.
Currently, they point to Linux on aarch64, because that's the main developer's setup.
