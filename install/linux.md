---
title: Linux
nav_order: 2
layout: page
description: ""
parent: Install
---
# Install on Linux

## Flatpak
Can be installed on any Linux distribution. Find Vorta on [Flathub](https://flathub.org/apps/details/com.borgbase.Vorta). To install:
```
$ flatpak install flathub com.borgbase.Vorta
```

Settings can be transferred by copying `~/.local/share/Vorta/settings.db` to `~/.var/app/com.borgbase.Vorta/data/Vorta/`.

Maintained by [@Hofer-Julian](https://github.com/Hofer-Julian).


## Install from Source
The most generic way is to install it as Python package using [PIP](https://pip.readthedocs.io/en/stable/installing/). First [install](https://borgbackup.readthedocs.io/en/stable/installation.html) Borg using the package of your distribution or via PyPI. The latter needs some additional [source packages](https://borgbackup.readthedocs.io/en/stable/installation.html#dependencies). Then install Vorta from PyPI. Your local Python version must be >= 3.6.
```
$ pip3 install vorta
```

### Add Entry to Application Launcher
You can add a `.desktop` entry to get a link to Vorta in your application launcher, usually `~/.local/share/applications/vorta.desktop`. Use the template available [here](https://github.com/borgbase/vorta/blob/master/src/vorta/assets/metadata/com.borgbase.Vorta.desktop) and adjust the `Exec` and [`Icon`](https://github.com/borgbase/vorta/blob/master/src/vorta/assets/icons/scalable/com.borgbase.Vorta.svg) paths if necessary. 


## Distribution Packages

### Arch Linux
Use the [AUR package](https://aur.archlinux.org/packages/vorta/).
```
$ yay -S vorta
```

Maintained by [@bjo81](https://github.com/bjo81).


### RPM-based packages

Can be used on for Fedora, EPEL (and friends), OpenSuse, Mageia and CentOS >= 7. For more details see the [custom repo](https://copr.fedorainfracloud.org/coprs/luminoso/vorta/).
```
$ sudo dnf copr enable luminoso/vorta
$ sudo dnf install vorta
```

Maintained by [@luminoso](https://github.com/luminoso)


### Solus Linux
Use the official [package](https://dev.getsol.us/source/vorta/). Command for install:
```
$ sudo eopkg it vorta
```
Maintained by [@kyrios123](https://github.com/kyrios123).


### Ubuntu Linux
Use the official [PPA](https://launchpad.net/~samuel-w1/+archive/ubuntu/vorta/). Supports 20.04 and greater. Command for install:
```
$ sudo add-apt-repository ppa:samuel-w1/vorta
$ sudo apt-get update
$ sudo apt-get install vorta
```
Maintained by [@samuel-w](https://github.com/samuel-w).


**Looking to maintain a package?** [Open](https://github.com/borgbase/vorta/issues/new) an issue or pull request and it will be added here.



