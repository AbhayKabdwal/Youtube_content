# How to install git on linux

## Ubuntu, Debian-based Distributions, and Kali Linux
```bash
# Open Terminal and update package lists
sudo apt update

# Install Git
sudo apt install git

# Verify Installation
git --version
```

## Fedora
```bash
# Open Terminal and update package lists
sudo dnf update

# Install Git
sudo dnf install git

# Verify Installation
git --version
```

## Manjaro and Garuda Linux (Arch-based Distributions)
```bash
# Open Terminal and update package lists
sudo pacman -Syu

# Install Git
sudo pacman -S git

# Verify Installation
git --version
```

## NixOS
```bash
# Open Terminal and update package lists
nix-env -u '*'

# Install Git
nix-env -i git

# Verify Installation
git --version
```