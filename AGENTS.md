# Agent Guide: dotfiles

This repository is used for managing dotfiles testing and development environments via Vagrant.

## Infrastructure
- **Vagrant VMs**:
  - `dotfiles-test`: Ubuntu 18.04 (Bento box)
  - `dotfiles-dev`: Ubuntu 24.04 (Bento box)
- **Provider**: VirtualBox

## Workspace Structure
- `assets/`: Platform-specific binary assets (Linux/Windows).
- `.local/bin/`: Local tool binaries (e.g., `clang-format`, `clangd`).

## Developer Commands
- **VM Management**:
  - `vagrant up [vm_name]`: Start the specified VM.
  - `vagrant ssh [vm_name]`: SSH into the specified VM.
  - `vagrant halt [vm_name]`: Stop the specified VM.
  - `vagrant destroy [vm_name]`: Destroy the specified VM.
