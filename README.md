# Lenovo Ideapad battery conservation mode on GNU/Linux
[![made-with-bash](https://img.shields.io/badge/Made%20with-Bash-1f425f.svg)](https://www.gnu.org/software/bash/)
[![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)

![ideapad-cm-screencast.gif](ideapad-cm-screencast.gif "ideapad-cm Screencast")

A script to enable/disable battery conservation mode in Lenovo Ideapad laptops. :computer: :battery: :guardsman:

## Installation (Arch Linux)

If you use Arch Linux, then you can use the bundled PKGBUILD file to build and
install this script.

```bash
git clone https://github.com/tildehacker/ideapad-conservation-mode.git
cd "ideapad-conservation-mode"
makepkg
sudo pacman -U *.tar.xz
```

## Installation
Clone this repository to a directory of your choice and add it to your PATH environment variable.

### Clone
```bash
git clone https://github.com/tildehacker/ideapad-conservation-mode.git
```

### Add it to PATH
Adjust `.bashrc` according to your current shell.
```bash
echo "export PATH=\$PATH:$( pwd )" >> ~/.bashrc
```

## Usage
```bash
Usage:
	ideapad-cm enable|disable|status [acpi_call|ideapad_laptop]
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
This project is licensed under the GPL-3.0 License - see the [LICENSE](LICENSE)
file for details.
