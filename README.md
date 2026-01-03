# Firefox custom settings

Set global firefox preferences through one package.

## Installation
Ensure that you got firefox installed to make this effective!!

Add librefox repo, the following lines, to /etc/pacman.conf

```
[librefox_arch]
SigLevel = Optional DatabaseOptional
Server = https://github.com/librefox05/$repo/raw/refs/heads/main/$arch
```

then run

```
sudo pacman -Syy firefox-custom-settings
```

