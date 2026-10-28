<div align="center">

<img src="rashadooz_os_logo.png" alt="RASHADOOZ OS" width="300">

# RASHADOOZ OS

**A tiny, fast, command-line Linux operating system.**

![RAM](https://img.shields.io/badge/RAM-128%20MB-teal)
![ISO](https://img.shields.io/badge/ISO-28%20MB-blue)
![Kernel](https://img.shields.io/badge/Kernel-Linux-yellow)
![Interface](https://img.shields.io/badge/Interface-CLI-green)

</div>

---

## About

RASHADOOZ OS is a minimal operating system built on the **Linux kernel** with a **Linux command-line interface**. It is designed to boot quickly and run on very old or very small machines, virtual machines and embedded devices.

## Features

- 💻 **Command-line only**: no desktop, no bloat
- 🧠 Runs in just **64 MB of RAM**
- 💿 Tiny **less than 1 MB iamge iso**
- ⚡ Fast boot 

## System Requirements

| Component | Requirement |
|-----------|-------------|
| CPU       | x86 / x86_32 |
| RAM       | **64 MB** minimum |
| Storage   | Not required (runs live from ISO) |
| Boot      | CD/DVD, USB, or virtual machine |

## Download

| File | Size |
|------|------|
| `rashadooz_os.iso` | **556 KB** |

> Get the latest ISO from the [Releases](../../releases) page.

## Quick Start

### Run in QEMU (64 MB RAM)

```bash
qemu-system-i386 -cdrom rashadooz.iso
```

### Run in VirtualBox

1. Create a new **(32-bit)** virtual machine
2. Set memory to **64 MB**
3. Skip virtual hard disk creation
4. Attach `rashadooz.iso` as the optical drive and start the VM

### Write to a USB drive

```bash
# Replace /dev/sdX with your USB device. This ERASES it!
sudo dd if=rashadooz.iso of=/dev/sdX bs=4M status=progress && sync
```

## Usage

After boot you land in a Linux shell:

```bash
help          # show this list of commands
version       # print the operating system version
info          # show details system information 
ls            # list files and directories
snake         # play snake game with (W A S D and Q)
Tetris        # play Tetris game with (W A S D and Q)
clear         # clear the screen 
```


## Project Structure

```
rashadooz-os/
├── README.md
├── rashadooz-os-wallpaper.jpg
└── rashadooz.iso   (the os iamge iso)
```


<div align="center">Made with 🦅 by <b>RASHADOOZ</b></div>
