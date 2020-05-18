# mnchrm-grb

A monochromatic
[GRUB](https://www.gnu.org/software/grub/) 
theme that displays white icons on a black background.

![screenshot](screenshot.png?raw=true)

Includes logos for over a dozen popular operating systems, including:

- Arch Linux
- CentOS
- Debian
- elementaryOS
- Fedora
- FreeBSD
- Gentoo Linux
- Linux Mint
- macOS
- Manjaro Linux
- Microsoft Windows
- OpenBSD
- openSUSE
- Solus
- Ubuntu
- Void Linux

... in addition to some generic icons.

## Manual Installation

Copy the `mnchrm` folder to any directory accessible by GRUB at boot, i.e., `/boot/grub/themes/`:

    # cp -r mnchrm /boot/grub/themes/

Then set the `GRUB_THEME` value in `/etc/default/grub` to the location of `theme.txt`:

    GRUB_THEME="/boot/grub/themes/mnchrm/theme.txt"

Finally, update the configuration file. With `grub-mkconfig`:

    # grub-mkconfig -o /boot/grub/grub.cfg

Consult your distribution's documentation for more details.
