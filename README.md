# Ansible playbook setup for CTF-s

## Introduction
This playbook is intended to be used on a fresh Linux installation. This playbook mostly focuses on binary exploitation and reverse engineering tools, but also includes some other tools that are useful in CTF-s.

> **Note:** This playbook is intended to be used on a fresh Linux installation. It may not work as intended on a system that already has some of the tools installed.

> **Another Note:** Also, this playbook was created because at the time of writing, i just broke my Linux installation 💀

## Description
Tested on Kali Linux WSL on 30th of June 2024 and Ubuntu 22.04 LTS on 11th of July 2024. This playbook installs the following tools:
- [python3](https://www.python.org/)
- [pip](https://pypi.org/project/pip/)
- [pycryptodome](https://pycryptodome.readthedocs.io/en/latest/)
- [pwntools](https://github.com/Gallopsled/pwntools)
- [GDB](https://www.gnu.org/software/gdb/)
- [GDB-Peda](https://github.com/longld/peda)
- [GDB-Pwndbg](https://github.com/pwndbg/pwndbg)
- [GDB-GEF](https://github.com/hugsy/gef)
- [gcc-multilib](https://packages.ubuntu.com/focal/gcc-multilib)
- [gdb-multiarch](https://packages.ubuntu.com/focal/gdb-multiarch)
- [angr](https://github.com/angr/angr)
- [netcat](https://netcat.sourceforge.io/)
- [ropper](https://github.com/sashs/Ropper)
- [one_gadget](https://github.com/david942j/one_gadget)
- [qemu](https://www.qemu.org/)
- [docker](https://www.docker.com/)
- [nmap](https://nmap.org/)
- [sqlmap](https://sqlmap.org/)
- [john](https://www.openwall.com/john/)
- [steghide](http://steghide.sourceforge.net/)
- [binwalk](https://github.com/ReFirmLabs/binwalk)
- [hashcat](https://hashcat.net/hashcat/)
- [dirbuster](https://tools.kali.org/web-applications/dirb)
- [ffuf](https://github.com/ffuf/ffuf)
- [nodejs](https://nodejs.org/)
- [npm](https://www.npmjs.com/)
- [tmux](https://github.com/tmux/tmux)
- [patchelf](https://nixos.org/patchelf.html)
- [pwninit](https://github.com/io12/pwninit)
- [cargo](https://doc.rust-lang.org/cargo/)
- [elfutils](https://sourceware.org/elfutils/)

## Requirements
- [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)
- Basically any Linux that uses apt package manager
- You

## How to use
```
sudo apt install ansible
ansible-playbook -i localhost playbook.yml -vvvv
```