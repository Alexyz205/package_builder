# Development Tools Installer

This repository contains installation scripts for essential development tools:

- Neovim (v0.10.4) - A hyper-extensible text editor
- Tmux (v3.5) - A terminal multiplexer
- Ranger (v1.9.4) - A file manager with VI key bindings

## Requirements

These scripts require one of the following package managers:
- apt-get (Debian/Ubuntu)
- Homebrew (macOS)

## Supported Architectures

- x86_64 (64-bit Intel/AMD)
- aarch64 (ARM64)

## Usage

### Standard Installation

To install directly to your system:

```bash
# Install Neovim
./install_nvim

# Install Tmux
./install_tmux

# Install Ranger
./install_ranger
```

### Create Portable Packages

To create portable .tar.gz packages:

```bash
# Create Neovim package
./install_nvim --targz

# Create Tmux package
./install_tmux --targz

# Create Ranger package
./install_ranger --targz
```

The packaged archives will be created in the parent directory with names like:
- `nvim_release_0.10.4_x86_64.tar.gz`
- `tmux_release_3.5_x86_64.tar.gz`
- `ranger_release_1.9.4_x86_64.tar.gz`

## Features

- Automatic dependency installation
- Cross-platform support (Linux and macOS)
- Architecture detection
- Option to create portable packages
- Uses specific tagged releases for consistent builds

## Notes

- The scripts require sudo access for system-wide installation
- Each tool is built from source using the specified version tags
- The build process may take some time depending on your system
