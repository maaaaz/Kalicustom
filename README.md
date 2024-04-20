Kali custom
===========

Description
-----------
Some Kali VM builds, based on the [official Kali VM builds](https://www.kali.org/get-kali/#kali-virtual-machines), but with customizations

Additions
---------
Everything is documented in the [Github action build workflow](https://github.com/maaaaz/Kalicustom/blob/main/.github/workflows/build.yml) but here is a quick summary:
- These packages (utilities, infosec tools etc.):
  - https://github.com/maaaaz/dotfiles/blob/master/debian_ubuntu_packages.txt
  - https://github.com/maaaaz/dotfiles/blob/master/kali_missing_packages.txt
  - Microsoft Sysmon and ProcDump for Linux
  - [Escobar](https://github.com/savely-krasovsky/escobar)
- Bash as default shell
- A friendlier [`.vimrc`](https://github.com/maaaaz/dotfiles/blob/master/.vimrc) in the `root` and `kali` homes
- VMWare and VirtualBox compatibility
- Virtualbox shared folders permission fix by adding the `kali` user to the `vboxsf` group
- A Python `venvcommon` virtualenv (in the `root` home, use `workon venvcommon`), containing [common infosec Python packages](https://github.com/maaaaz/dotfiles/blob/master/python_common.txt)
- azerty keymap and France timezone (sorry, I am french), but you can easily change these settings afterward

Releases
---------
- See https://github.com/maaaaz/Kalicustom/releases
- Releases are hosted on `archive.org` (https://archive.org/details/@maaaaz/) because:
  - `archive.org` accepts larger files than the Github release feature one (2 GB, which is not enough)
  - `archive.org` provides multiple useful downloading capabilities: direct download, torrent etc.
  - `archive.org` is an awesome project
- Release files currently are **8 GB compressed | 25 GB decompressed**

Changelog
---------
2024-04-20: first release

Copyright and license
---------------------
* All trademarks, service marks, trade names and product names appearing on this repository are the property of their respective owners 
