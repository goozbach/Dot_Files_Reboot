# Dot File Management -- REBOOT
I have always wanted a simple way of managing my bash file settings (`.bashrc`, `.bash_profile` and the like). I had built a system much like this one, but it didn't work very well. So this is a ground-up rewrite

This repository is a reboot of the (original Dot_Files)[https://github.com/goozbach/dot_files] repository. Created to simplify the delivery and manageability for multiple systems.

There will be multiple branches, one for each system's default files. The "Master" branch will house just the README.markdown and makefile. To get a copy of the default files provied from a certian platform check out that platform's branch.

In the future, the old repository will be sanitized and added as an additional branch called "goozbach_custom"

## Instructions
### Creating source files
Any file which matches the shell glob `_*` will be linked into `$HOME` as a symlink with the first `_`  replaced with a `.`

For example:

    _bashrc

becomes

    ${HOME}/.bashrc

### Installing source files
It's as simple as running:

    make

From this top-level directory.

## Requirements
* bash
* gnu make
