Workman keyboard layouts
========================

Workman keyboard layout originally proposed by OJ Bucao at https://workmanlayout.org.

When learning cold-turkey, try printing the included keyboard image as a desk reference.

# Workman Keyboard Layout for X11 (Optimized for Vim)

This guide will help you install the Workman keyboard layout for X11 systems using a simple command. This layout is optimized for Vim users and improves ergonomic efficiency.

## Installation

You can install the layout by downloading the `.Xmodmap` file directly into your home directory:

```bash
wget -O ~/.Xmodmap https://raw.githubusercontent.com/twichai/Workman-for-vim/master/xmodmap/xmodmap.workman
```

Then, activate the new keyboard layout with the following command:

```bash
xmodmap ~/.Xmodmap
```

## Make It Persistent

To make sure the layout is applied every time you log in, add the following line to your `.xinitrc` or `.xsession` file:

```bash
xmodmap ~/.Xmodmap
```

## Notes

* This configuration is intended for X11 systems (e.g., most Linux desktops).
* Make sure you back up your existing `.Xmodmap` if you have one.

## Uninstallation

If you want to revert to your previous layout, simply delete the `.Xmodmap` file or restore your backup, then run:

```bash
setxkbmap us
```

---
