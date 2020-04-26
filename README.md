
# grub-bgrt theme

A theme for GRUB2 which uses your system's UEFI logo (aka BGRT).

## Installation

```sh
    sudo ./install.sh	# Fetches your BGRT, adjusts the theme to suit and installs it.
    echo GRUB_THEME=/boot/grub/themes/grub-bgrt/theme.txt | sudo tee -a /etc/default/grub
    sudo update-grub
```

## Font

To change the font in the theme, try something like:

```sh
	grub-mkfont -o dejavu_12.pf2 -a -s 12 /usr/share/fonts/truetype/dejavu/DejaVuSans.ttf
```

(-a adds antialiasing, -s 12 sets the size to 12). Don't forget to update the `theme.txt.in` as well.

## Plymouth Theme

You may also want to pair this with origin author [plymouth theme](https://github.com/darac/plymouth-bgrt).

## License

All the files in this project are distributed under the [GNU General Public License](./LICENSE).

## Author

Paul Saunders

## Modificator
Izumi Kagurazaka

## Forked from

https://github.com/fghibellini/arch-silence
