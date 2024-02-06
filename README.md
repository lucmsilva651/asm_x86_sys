# asm_x86_sys

This repo contains the code for a simple Operating System that shows the message "Hello World!" when booted.

Following the ["Building an OS"](https://www.youtube.com/watch?v=9t-SPC7Tczc&list=PLFjM7v6KGMpiH2G-kT781ByCNC_0pKpPN) tutorial.

## Compiling and testing

### Pre-requisites
Any Linux distribution or macOS (via Homebrew). If you use Windows, you can try [WSL (Linux on Windows)](https://learn.microsoft.com/en-us/windows/wsl/install).

### Installing tools
Run the commands below to install Make, NASM (the Assembly compiler) and the QEMU Virtual Machine system.
```sh
sudo apt install make nasm qemu qemu-system-x86
```

### Compiling and testing
Run the commands below to compile the ASM file inside /src and run the OS:
```sh
make && qemu-system-i386 -fda build/main_floppy.img
```

Credits: nanobyte - [GitHub](https://github.com/nanobyte-dev), [YouTube](https://www.youtube.com/@nanobyte-dev)
