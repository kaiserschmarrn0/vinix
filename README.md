# vOS

An effort to write a modern, fast, and interesting operating system in V.

Join the [Discord chat](https://discord.gg/vlang) (`#v-os` channel).

#### Goals

- Keep it simple and easy to understand.
- Write it in V as much as possible.
- Target modern 64-bit architectures and CPU features.

#### Why?

- Explore V capabilities in bare metal programming.
- Break the compiler as much as possible.
- Build a minimal and useful platform for software [especially written in V :^)], allowing for better control, isolation, and smaller attack surface in VMs.
- Having fun.

### Build Instructions

#### Prerequisites

The following packages need to be installed on the system in order to build vOS: `make`, `git`, `nasm`, `gcc/clang`, `python3`, `pip3`, `parted`, `pkg-config`, `libuuid`, `libfuse`, and `qemu` to test it.

#### Build commands

To build the distro which includes the cross toolchain necessary
to build kernel and ports, run:

```bash
make distro
```

The OS can then be built with `make` and ran within qemu with `make run`.
