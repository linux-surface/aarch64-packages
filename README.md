# Arch Linux Packages for AArch64 Surface Devices


## `linux-firmware`

Linux firmware package with additions and changes for the Surface Pro X.
See https://github.com/linux-surface/aarch64-firmware for more information.


## `linux-surface`

Linux kernel packages for the Surface Pro X.
Use `makepkg-aarch64` to cross-compile from any host, e.g. `x86_64`.
Set `MAKEFLAGS="-j$(nproc)"` (or similar) to use all available cores for building.


## `makepkg-aarch64`

`makepkg-aarch64` command for (cross-)compiling Arch Linux AArch64 packages from any host system (e.g. `x86_64`).
_Warning: This will only work for some packages._
_In particular, this will not work for packages linking to external libraries._


## `rmtfs-dummy`

Patched Qualcomm Remote File System ([`rmtfs`](https://github.com/linux-msm/rmtfs)) service.
Uses dummy files instead of vendor-provided EFS partitions.
This is currently required on the Surface Pro X as the EFS partitions are not available to us yet.


## `shim-aarch64-signed`

Signed Secure-Boot `shim.efi` executable and associated tools for AArch64, as provided by openSUSE (https://software.opensuse.org/package/shim).
