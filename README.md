# Linux Networking Shell Basics

[![Shell checks](https://img.shields.io/github/actions/workflow/status/itkrivoshei/linux-networking-shell-basics/shell.yml?branch=master&style=flat-square&label=shell%20checks)](https://github.com/itkrivoshei/linux-networking-shell-basics/actions/workflows/shell.yml)
[![License: GPL-3.0](https://img.shields.io/badge/license-GPL--3.0-blue?style=flat-square)](LICENSE)
[![Shell](https://img.shields.io/badge/shell-Bash-lightgrey?style=flat-square)](https://www.gnu.org/software/bash/)

Archived UNIX/Linux networking, system administration, and shell scripting exercises from the 42 School / School 21 curriculum.

## Stack

- Bash
- UNIX/Linux command-line tools
- Basic networking utilities: `ifconfig`, `netstat`, `arp`, `nslookup`, `host`, `whois`, `traceroute`

## Scope

```txt
network/    Networking command exercises
system/     System administration command exercises
scripting/  Small Bash scripts and an interactive exercise menu
```

The repository is kept as historical learning material. Some commands reflect the original bootcamp environment and may be macOS/BSD-specific or outdated on modern Linux systems.

## Install

No package installation is required.

Clone the repository:

```bash
git clone https://github.com/itkrivoshei/linux-networking-shell-basics.git
cd linux-networking-shell-basics
```

## Run

Most files are small command exercises and can be inspected directly:

```bash
cat network/01
cat system/01
cat scripting/01
```

Run the interactive menu:

```bash
cd scripting
./03
```

Run an individual script:

```bash
cd scripting
./01
```

`scripting/02` can delete local users. It is blocked by default and should not be run on a real system without review. To run it intentionally:

```bash
cd scripting
ALLOW_USER_DELETE=1 ./02
```

## Verify

Check Bash syntax locally:

```bash
bash -n scripting/01 scripting/02 scripting/03
```

The repository also includes a GitHub Actions workflow that runs Bash syntax checks for files under `network/`, `system/`, and `scripting/`.

## License

Licensed under the [GPL-3.0 License](LICENSE).
