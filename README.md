<div align="center">

<img src="rashadooz_os_logo.png" alt="RASHADOOZ OS" width="300">

# RASHADOOZ OS

**A tiny, fast, command-line Linux operating system.**

![RAM](https://img.shields.io/badge/RAM-128%20MB-teal)
![ISO](https://img.shields.io/badge/ISO-28%20MB-blue)
![Kernel](https://img.shields.io/badge/Kernel-Linux-yellow)
![Interface](https://img.shields.io/badge/Interface-CLI-gray)

</div>

---

## About

RASHADOOZ OS is a minimal operating system built on the **Linux kernel** with a **Linux command-line interface**. It is designed to boot quickly and run on very old or very small machines, virtual machines and embedded devices.

## Features

- 🐧 Powered by the **Linux kernel**
- 💻 **Command-line only**: no desktop, no bloat
- 🧠 Runs in just **128 MB of RAM**
- 💿 Tiny **28 MB ISO image**
- ⚡ Fast boot
- 🐺 Wolf-themed wallpaper and boot branding

## System Requirements

| Component | Requirement |
|-----------|-------------|
| CPU       | x86 / x86_64 |
| RAM       | **128 MB** minimum |
| Storage   | Not required (runs live from ISO) |
| Boot      | CD/DVD, USB, or virtual machine |

## Download

| File | Size |
|------|------|
| `rashadooz_os.iso` | **28 MB** |

> Get the latest ISO from the [Releases](../../releases) page.

## Quick Start

### Run in QEMU (128 MB RAM)

```bash
qemu-system-x86_64 -m 128 -cdrom rashadooz_os.iso
```

### Run in VirtualBox

1. Create a new **Linux (64-bit)** virtual machine
2. Set memory to **128 MB**
3. Skip virtual hard disk creation
4. Attach `rashadooz_os.iso` as the optical drive and start the VM

### Write to a USB drive

```bash
# Replace /dev/sdX with your USB device. This ERASES it!
sudo dd if=rashadooz_os.iso of=/dev/sdX bs=4M status=progress && sync
```

## Usage

After boot you land in a Linux shell:

```bash
uname -a      # kernel info
free -m       # check memory usage
ls            # list files
help          # list available commands
poweroff      # shut down
```


## Project Structure

```
rashadooz-os/
├── README.md
├── rashadooz-os-wallpaper.jpg
└── rashadooz_os.zip   (compressed os in .zip)
```

## License

The Linux kernel is licensed under GPLv2. Add your own license for RASHADOOZ OS-specific files.

---

<div align="center">Made with 🦅 by <b>RASHADOOZ</b></div>
