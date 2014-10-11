pietrushnic/rpi-dt-firmware
==========

Raspberry Pi Linux kernel 3.16.5+ (ARCH_BCM2835) with additional patches.

Install
-------

```text
sudo REPO_URI=https://github.com/pietrushnic/rpi-dt-firmware rpi-update
```




Changelog
---------
2014-10-12:
* Rebase to 3.16.5 - second release
* Built from GitHub repository [rpi-dt-linux](https://github.com/pietrushnic/rpi-dt-linux.git) - `rpi-3.16.y` branch

2014-09-28:
* First release

Links
* [Upstreaming](https://github.com/raspberrypi/linux/wiki/Upstreaming)
* [Device Tree on ARCH_BCM2708](https://github.com/raspberrypi/linux/wiki/Device-Tree-on-ARCH_BCM2708)


Sources
-------
* [raspberrypi/tools](https://github.com/raspberrypi/tools/archive/2324612605316a64f9daae33712e5afe762cf995.tar.gz)
* [raspberrypi/firmware](https://github.com/raspberrypi/firmware/archive/c786f85ea2495ca8ae239fb9575fbc1d85fb381e.tar.gz)
* [http://git.denx.de/?p=u-boot/u-boot-arm.git](http://git.denx.de/?p=u-boot/u-boot-arm.git;a=snapshot;h=3d420cbd355a5f09e4f113eb10579a264a8ef138;sf=tgz)
* [pietrushnic/rpi-dt-linux](https://github.com/pietrushnic/rpi-dt-linux/archive/1006e0fe1953ca53a1aabaaddf45c9b154ec4a93.tar.gz)


Patches
--------
None

Kernel config
-------------
Default config: bcm2835_defconfig



Added:
```text
IKCONFIG=y
IKCONFIG_PROC=y
MMC_BCM2835=y
```


<p align="center">Built with <a href="https://github.com/notro/rpi-build/wiki">rpi-build</a></p>
