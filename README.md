# aarch64-elf-pkgbuilds

This is PKGBUILD scripts to build aarch64 cross-toolchain for baremetal.

This PKGBUILDs based on mips64-elf-* (AUR).

## How to install

### Install order

Please install packages in following order:

1. aarch64-elf-binutils
2. aarch64-elf-gcc-stage1
3. aarch64-elf-newlib
4. aarch64-elf-gcc

### How to make packages

```
$ cd aarch64-elf-binutils
$ makepkg -s
$ sudo pacman -U aarch64-elf-binutils*.tar.xz

...the rest is the same as above.
```



## Memo

I did not check that the toolchain can compile code and execute it on baremetal environment.
