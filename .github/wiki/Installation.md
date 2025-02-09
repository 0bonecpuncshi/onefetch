This wiki page will guide you through getting onefetch working on your system.

[![Packaging status](https://repology.org/badge/vertical-allrepos/onefetch.svg)](https://repology.org/project/onefetch/versions)

# Table of Contents

* [Universal Install](#universal-install)
    * [Cargo](#cargo)
    * [Snap](#snap)
    * [Build from source](#build-from-source)
* [OS/Distro Packages](#osdistro-packages)
    * [Alpine Linux](#alpine-linux)
    * [Arch](#arch)
    * [Fedora](#fedora)
    * [FreeBSD](#freebsd)
    * [Funtoo](#funtoo)
    * [macOS](#macos)
        * [Homebrew](#homebrew)
        * [MacPorts](#macports)
    * [NetBSD](#netbsd)
    * [NixOS](#nixos)
    * [openSUSE](#openSUSE-Leap-or-Tumbleweed)
    * [Ubuntu](#ubuntu-ppa)
    * [Void Linux](#void-linux)
    * [Windows](#windows)
        * [Winget](#Winget)
        * [Scoop](#scoop)
        * [Chocolatey](#chocolatey)

# Universal

If your architecture is supported by the pre-built binaries, you can download them from the [releases page](https://github.com/o2sh/onefetch/releases).

## Cargo

First, install `rustup` to get the `rust` compiler installed on your system (using the recommended `curl https://sh.rustup.rs -sSf | sh -s` installation method) and then

```
cargo install onefetch
```

This method will build the binary from source.

To update, run

```
cargo install onefetch --force
```

## Snap

For a system with Snap installed, run

```
snap install onefetch
```

The stable version will be installed for you automatically.

## Build from source

First, install `rustup` to get the `rust` compiler installed on your system (using the recommended `curl https://sh.rustup.rs -sSf | sh -s` installation method) and then

```
git clone https://github.com/o2sh/onefetch
cd onefetch
make install
```

# OS/Distro Packages

## Alpine Linux

1. Update repositories
    - `apk update`
2. Install the package
    - `apk add onefetch`


## Arch

Onefetch is available in the official repos.

- Install the package
    - `pacman -S onefetch`

## Fedora

Install it from the COPR

```
sudo dnf copr enable varlad/onefetch
sudo dnf install onefetch
```

## FreeBSD

Install it from the official repositories

- `pkg install onefetch`

## Funtoo

Funtoo has an autogenerated onefetch package in the official kits:

- `emerge app-misc/onefetch`

## MacOS

### HomeBrew

Install `onefetch` with Homebrew

```
brew install onefetch
```

To update, run

```
brew upgrade onefetch
```

### MacPorts

Install `onefetch` with MacPorts

```
sudo port selfupdate
sudo port install onefetch
```

To update run,

```
sudo port upgrade onefetch
```

## NetBSD

Install it from the official repositories.

- `pkg_add onefetch`


## NixOS

Install it from the official repositories

- `nix-env -i onefetch`


## openSUSE Leap or Tumbleweed

Install it from the official repositories.

- `zypper install onefetch`


## Ubuntu (ppa)

```
sudo add-apt-repository ppa:o2sh/onefetch
sudo apt-get update
sudo apt-get install onefetch
```

If your Ubuntu version isn't supported, use [snap](#snap).

## Void Linux

Install it from the official repositories

- `sudo xbps-install -S onefetch`


## Windows

### Winget

You can install onefetch using [winget](https://docs.microsoft.com/en-us/windows/package-manager/winget/)

```
winget install onefetch
```

### Scoop

For [Scoop](https://scoop.sh/) users, onefetch is available from the "Extras" bucket

```
scoop bucket add extras
scoop install onefetch
```

### Chocolatey

If you prefer to use [Chocolatey](https://chocolatey.org/) to manage software, it can be installed like so

```
choco install onefetch
```