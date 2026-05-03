<!---
SPDX-FileCopyrightText: © 2018-2025 Alexandros Theodotou <alex@zrythm.org>
SPDX-License-Identifier: FSFAP
-->

# Zrythm — AUR Binary Package

Automatically built binary package of the **latest version** of [Zrythm](https://github.com/zrythm/zrythm) for Arch Linux and derivatives.

The package is updated daily and always matches the latest version available in AUR. No need to compile from source — just install the prebuilt binary.

## Installation

### Via yay (recommended)

```bash
yay -S zrythm-bin
```

### Via paru

```bash
paru -S zrythm-bin
```

### Manually

```bash
git clone https://aur.archlinux.org/zrythm-bin.git
cd zrythm-bin
makepkg -si
```

## Updating

```bash
yay -Su zrythm-bin
```

## How it works

This repository contains a GitHub Actions pipeline that:

1. Checks the latest Zrythm version in AUR every day
2. Builds the package in a clean Arch Linux environment
3. Publishes the ready-to-install `.pkg.tar.zst` to [GitHub Releases](https://github.com/IRRatium/zrythm-aur-bin/releases)
4. Updates the [AUR package zrythm-bin](https://aur.archlinux.org/packages/zrythm-bin)

When installing via yay, the prebuilt binary is downloaded directly — no compilation required.

## About Zrythm

*A highly automated and intuitive digital audio workstation*

![screenshot](https://www.zrythm.org/static/images/screenshots/screenshot-20240208.png)

Zrythm is a DAW designed for both professionals and beginners, featuring support for LV2/CLAP/VST2/VST3/AU plugins, flexible automation and powerful mixing tools.

Learn more at the [official website](https://www.zrythm.org).

## License

Zrythm is licensed under [AGPL-3.0](https://www.gnu.org/licenses/agpl-3.0).
