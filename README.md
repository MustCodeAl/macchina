![Macchina preview image](screenshots/banner.png)

[![Crates.io](https://img.shields.io/crates/v/macchina?style=for-the-badge&label=VERSION&color=0D3B66)](https://crates.io/crates/macchina)
[![Crates.io](https://img.shields.io/crates/d/macchina?style=for-the-badge&label=DOWNLOADS&color=0D3B66)](https://crates.io/crates/macchina)
![reposize](https://img.shields.io/github/repo-size/grtcdr/macchina?color=0D3B66&logo=github&style=for-the-badge)
![loc](https://img.shields.io/tokei/lines/github/grtcdr/macchina?color=0D3B66&label=Lines%20of%20Code&logo=rust&style=for-the-badge)

# Table of Contents
- [About](#about)
- [Benchmarks](#bench)
- [Features](#features)
- [Dependencies](#deps)
- [Usage](#usage)
- [Installation](#install)
- [Platform Support](#platform-support)
- [Contributors](#contributors)
---

# About Macchina <a name="about"></a>

_Macchina_ lets you view basic system information, like your hostname, kernel, uptime, memory usage, and much more.
It provides you with convenient features and customization options but doesn't lose sight of its two main priorities, minimalism and performance.

![Macchina preview image](screenshots/preview.png)

---

# Benchmarks <a name="bench"></a>
_Macchina_ is pretty fast, see for yourself!

- Execution time is measured using [hyperfine](https://github.com/sharkdp/hyperfine)
- Hiding elements with `--hide` significantly improves speed

## 🐧 Linux
| Command | Mean [ms] | Min [ms] | Max [ms] | Relative |
|:---|---:|---:|---:|---:|
| `macchina` | 24.7 ± 0.6 | 23.7 | 26.3 | 1.00 |
| `neofetch` | 373.4 ± 3.8 | 367.3 | 385.9 | 15.10 ± 0.39 |

__Summary__: `macchina` runs __15.10 ± 0.39__ times __faster__ than `neofetch`

## 👩🏽‍💻 macOS

| Command | Mean [ms] | Min [ms] | Max [ms] | Relative |
|:---|---:|---:|---:|---:|
| `macchina` | 5.0 ± 0.2 | 4.7 | 5.9 | 1.00 |
| `neofetch` | 484.5 ± 4.3 | 477.2 | 492.3 | 97.10 ± 3.84 |

__Summary__: `macchina` runs __97.10 ± 3.84__ times __faster__ than `neofetch`

## 🚩 NetBSD

| Command | Mean [ms] | Min [ms] | Max [ms] | Relative |
|:---|---:|---:|---:|---:|
| `macchina` | 245.1 ± 1.0 | 244.1 | 247.6 | 1.00 |
| `neofetch` | 1264.8 ± 5.7 | 1258.0 | 1276.9 | 5.16 ± 0.03 |

__Summary__: `macchina` runs __5.16 ± 0.03__ times __faster__ than `neofetch`

---

# Features <a name="features"></a>
### Themes
![Theme preview](screenshots/themes.png)

The [themes wiki page](https://github.com/grtcdr/macchina/wiki/Themes) contains a list of all the built-in themes that you can use.

### Bars
![Preview of bar argument](screenshots/bars.png)

### What it fetches
- Host
  - Username
  - Hostname
- Product
- Kernel
- Distribution
- Desktop Environment
- Window Manager
- Package Count <sup>[[1]](https://github.com/grtcdr/macchina/wiki/Platform-Support)</sup>
- Shell
- Terminal
- Processor
  - Model
  - Thread count
- Uptime
- Memory Usage
- Battery
  - Percentage
  - Status
- Palette

---

# Usage <a name="usage"></a>
_Macchina_ comes packed with __arguments__ that let you customize its behavior and styling.

The [usage wiki page](https://github.com/grtcdr/macchina/wiki/Usage) can tell you all about them and how they work.

---

# Dependencies <a name="deps"></a>
## 🐧 Linux:
- `wmctrl`
- __Gentoo Only:__ `portage-utils`
## 🚩 NetBSD:
- `wmctrl`
- `ripgrep`

The [dependencies wiki page](https://github.com/grtcdr/macchina/wiki/Dependencies) explains why these dependencies exist.

---

# Installation <a name="install"></a>
_Macchina_ is available on:

- [crates.io](https://crates.io/crates/macchina)
- [AUR](https://aur.archlinux.org/packages/macchina/)
- [pkgsrc](https://pkgsrc.se/sysutils/macchina)

Read the [installation guide](https://github.com/grtcdr/macchina/wiki/Installation) to see the multiple ways you can install it on your machine, or download the [prebuilt binaries](https://github.com/grtcdr/macchina/releases)!

---

# Platform Support <a name="platform-support"></a>

|  Platform |      Support       |
| :-:       |        :-:         |
| GNU/Linux |        Yes         |
| NetBSD    |        Yes         |
| macOS     |        Yes         |
| Windows   |        Partial     |

# 🌍 Contributors <a name="contributors"></a>

[![Crates.io](https://contrib.rocks/image?repo=grtcdr/macchina)](https://github.com/grtcdr/macchina/graphs/contributors)

_Macchina_, like many other open-source projects, would not be where it is right now without the help of its contributors, thank you all so much!

- Support for __NetBSD__ would not be possible without the help and testing of NetBSD/pkgsrc package maintainer [pin](https://pkgsrc.se/bbmaint.php?maint=pin@NetBSD.org)
- Support for __macOS__ and __Windows__ would not be possible without the help, testing and major contributions of [123marvin123](https://github.com/123marvin123)