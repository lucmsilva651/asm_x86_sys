# asm_x86_sys

This repo contains the code for a simple Operating System that shows the message "Hello World!" when booted.

Following the ["Building an OS"](https://www.youtube.com/watch?v=9t-SPC7Tczc&list=PLFjM7v6KGMpiH2G-kT781ByCNC_0pKpPN) tutorial.

## Compiling and testing

### Pre-requisites
Any Linux distribution or Mac OS (install via Homebrew). If you use Windows, you can try [WSL](https://learn.microsoft.com/en-us/windows/wsl/install).

### Installing tools
Run the commands below to install Make, NASM (assembly compiler) and QEMU VM system.
> sudo apt install make nasm qemu && sudo apt install qemu-system-x86

### Compiling and testing
Run the commands below to compile the ASM file inside /src and run the OS:
> make && qemu-system-i386 -fda build/main_floppy.img

Credits: nanobyte - [GitHub](https://github.com/nanobyte-dev), [YouTube](https://www.youtube.com/@nanobyte-dev)
