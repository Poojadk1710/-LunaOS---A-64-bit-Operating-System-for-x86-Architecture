# LunaOS - A 64-bit Operating System for x86 Architecture

LunaOS is a 64-bit OS designed for the x86_64 architecture, written in C and Assembly. LunaOS offers a simple kernel with basic OS functionalities, aimed at understanding low-level system programming, kernel development, memory management, and bootstrapping an operating system from scratch.

---

## Features

- Monolithic Kernel Architecture
- 64-bit x86_64 architecture support
- Custom bootloader (based on GRUB2)
- Kernel written in C and Assembly
- VGA text mode console output
- Basic paging and memory management
- Interrupt Descriptor Table (IDT) setup
- Programmable Interrupt Controller (PIC) initialization
- Simple keyboard input support
  

---

## Directory Structure

LunaOS/
├── boot/ # GRUB configuration and bootloader files
├── kernel/ # Kernel source files (C and Assembly)
├── include/ # Header files
├── build/ # Output binaries and ISO files
├── linker.ld # Linker script
├── Makefile # Build script
└── README.md # Project documentation

---

## Build Instructions

### Requirements

- GCC cross-compiler targeting `x86_64-elf`
- `make`, `nasm`
- `qemu` (for running the OS)
- `grub-mkrescue`
- `xorriso` or `genisoimage`

### Steps

# Clone the repository
git clone https://github.com/Poojadk1710/-LunaOS---A-64-bit-Operating-System-for-x86-Architecture.git
cd -LunaOS---A-64-bit-Operating-System-for-x86-Architecture

# Build the OS
make

# Run in QEMU
make run

To clean up build files:
make clean

