[update-readmes]   Mode: rewrite — migrating to template structure...
# gentoo-install

[![Built with Ona](https://ona.com/build-with-ona.svg)](https://app.ona.com/#https://github.com/Interested-Deving-1896/gentoo-install)

<!-- AI:start:what-it-does -->
_Description pending._
<!-- AI:end:what-it-does -->

## Architecture

<!-- AI:start:architecture -->
_Architecture documentation pending._
<!-- AI:end:architecture -->

## Install

<!-- Add installation instructions here. This section is yours — the AI will not modify it. -->

```bash
git clone https://github.com/Interested-Deving-1896/gentoo-install.git
cd gentoo-install
```

## Usage


First, boot into a live environment of your choice. I recommend using an [Arch Linux](https://www.archlinux.org/download/) live ISO,
as the installer will then be able to automatically download required programs or setup ZFS support on the fly.
Afterwards, proceed with the following steps:

```bash
pacman -Sy git  # (Archlinux) Install git in live environment, then clone:
git clone "https://github.com/oddlama/gentoo-install"
cd gentoo-install
./configure     # configure to your liking, save as gentoo.conf
./install       # begin installation
```

Every option is explained in detail in `gentoo.conf.example` and in the help menus of the TUI configurator.
When installing, you will be asked to review the partitioning before anything critical is done.

The installer should be able to run without any user supervision after partitioning, but depending
on the current state of the gentoo repository, you might need to intervene in case a package fails
to emerge. The critical commands will ask you what to do in case of a failure. If you encounter a
problem you cannot solve, you might want to consider getting in contact with some experienced people
on [IRC](https://www.gentoo.org/get-involved/irc-channels/) or [Discord](https://discord.com/invite/gentoolinux).

If you need to enter an installed system in a chroot to fix something (e.g. after rebooting your live system),
you can always clone the installer, mount your main drive under `/mnt` and use `./install --chroot /mnt` to
just chroot into your system.

## Configuration

<!-- Document configuration options here. This section is yours — the AI will not modify it. -->

## CI

<!-- AI:start:ci -->
_CI documentation pending._
<!-- AI:end:ci -->

## Mirror chain

<!-- AI:start:mirror-chain -->
This repo is maintained in [`Interested-Deving-1896/gentoo-install`](https://github.com/Interested-Deving-1896/gentoo-install) and mirrored through:

```
Interested-Deving-1896/gentoo-install  ──►  OpenOS-Project-OSP/gentoo-install  ──►  OpenOS-Project-Ecosystem-OOC/gentoo-install
```

Changes flow downstream automatically via the hourly mirror chain in
[`fork-sync-all`](https://github.com/Interested-Deving-1896/fork-sync-all).
Direct commits to OSP or OOC are detected and opened as PRs back to `Interested-Deving-1896`.
<!-- AI:end:mirror-chain -->

## Contributors

<!-- AI:start:contributors -->
_Contributors pending._
<!-- AI:end:contributors -->

## Origins

<!-- AI:start:origins -->
_Original project — no upstream fork._
<!-- AI:end:origins -->

## Resources

<!-- AI:start:resources -->
_No additional resource files found._
<!-- AI:end:resources -->

## License

<!-- AI:start:license -->
[MIT](https://github.com/Interested-Deving-1896/gentoo-install/blob/main/LICENSE) © 2026 [Interested-Deving-1896](https://github.com/Interested-Deving-1896)
<!-- AI:end:license -->
