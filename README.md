# Linux Surface

Linux running on the Microsoft Surface devices.
Follow the instructions below to install the latest kernel.

### Supported Devices

* Surface Book
* Surface Book 2
* Surface 3
* Surface Go
* Surface Go 2
* Surface Laptop
* Surface Laptop 2
* Surface Laptop 3
* Surface Laptop Go
* Surface Pro 3
* Surface Pro 4
* Surface Pro 2017
* Surface Pro 6
* Surface Pro 7
* Surface Pro 7+
* Surface Studio

### Features / What's Working

See the [feature matrix](https://github.com/linux-surface/linux-surface/wiki/Supported-Devices-and-Features#feature-matrix) for more information about each device.

### Disclaimer

* For the most part, things are tested on a Surface Book 2.
  While most things are reportedly fully working on other devices, your mileage may vary.
  Please look at the issues list for possible exceptions.

## Installation and Setup

We provide package repositories for the patched kernel and other utilities.
Please refer to the [detailed installation and setup guide][wiki-setup].
There, you may also find device-specific caveats.
After installation, you may want to have a look at the [wiki][wiki] and the `contrib/` directory for useful tweaks.

If you want to compile the kernel yourself (e.g. if your distribution is not supported), please have a look at the [wiki][wiki-compiling].

## Additional Information

### Notes

* If you are getting stuck at boot when loading the ramdisk, you need to install the Processor Microcode Firmware for Intel CPUs (usually found under Additional Drivers in Software and Updates).
* Using TLP can cause slowdowns, laggy performance, and occasional hangs if not configured properly! You have been warned.
* If you want to use hibernate instead of suspend, you need to create a swap partition or file, please follow your distribution's instructions (or [here][hibernate-setup]).

### Support

If you have questions or need support, please use our [Gitter Community][gitter]!
For development related questions and discussions, please consider joining our IRC channel on freenode (`freenode/##linux-surface`) or the [equivalent Matrix bridge](https://matrix.to/#/#freenode_##linux-surface:matrix.org).

## License
This repository contains patches, which are either derivative work targeting a specific already licensed source, i.e. parts of the Linux kernel, or introduce new parts to the Linux kernel.
These patches fall thus, if not explicitly stated otherwise, under the license of the source they are targeting, or if they introduce new code, the license they explicitly specify inside of the patch.
Please refer to the specific patch and source in question for further information.
License texts can be obtained at https://github.com/torvalds/linux/tree/master/LICENSES.

[wiki]: https://github.com/linux-surface/linux-surface/wiki
[wiki-setup]: https://github.com/linux-surface/linux-surface/wiki/Installation-and-Setup
[wiki-compiling]: https://github.com/linux-surface/linux-surface/wiki/Compiling-the-Kernel-from-Source

[gitter]: https://gitter.im/linux-surface
[hibernate-setup]: https://fitzcarraldoblog.wordpress.com/2018/07/14/configuring-lubuntu-18-04-to-enable-hibernation-using-a-swap-file
[releases]: https://github.com/linux-surface/linux-surface/releases

[linux-surface-kernel]: https://github.com/linux-surface/kernel/
