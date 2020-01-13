
Debian
====================
This directory contains files used to package weycashd/weycash-qt
for Debian-based Linux systems. If you compile weycashd/weycash-qt yourself, there are some useful files here.

## weycash: URI support ##


weycash-qt.desktop  (Gnome / Open Desktop)
To install:

	sudo desktop-file-install weycash-qt.desktop
	sudo update-desktop-database

If you build yourself, you will either need to modify the paths in
the .desktop file or copy or symlink your weycashqt binary to `/usr/bin`
and the `../../share/pixmaps/weycash128.png` to `/usr/share/pixmaps`

weycash-qt.protocol (KDE)

