pietrushnic/rpi-dt-firmware
==========

Raspberry Pi Linux kernel 3.17.1+ (ARCH_BCM2835) with additional patches.

Install
-------

```text
sudo REPO_URI=https://github.com/pietrushnic/rpi-dt-firmware BRANCH=mmc-dma rpi-update
```




Changelog
---------
2014-10-21:
* Fix bcm2835-mbox issues with checking wrong mailbox
* Enable DMA_BCM2835

2014-10-15:
* Rebase to 3.16.6

2014-10-15:
* Third release
* bcm2835-mbox, bcm2835-cpufreq and bcm2835-thermal drivers based on Lubomir Rintel [work](https://github.com/hackerspace/rpi-linux/commits/lr-raspberry-pi-new-mailbox)

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
* [raspberrypi/firmware](https://github.com/raspberrypi/firmware/archive/c23c0022740bb4531e841bd1321d2a652c8b3b0d.tar.gz)
* [http://git.denx.de/?p=u-boot/u-boot-arm.git](http://git.denx.de/?p=u-boot/u-boot-arm.git;a=snapshot;h=3d420cbd355a5f09e4f113eb10579a264a8ef138;sf=tgz)


Patches
--------
None

Kernel config
-------------
Default config: bcm2835_defconfig



Added:
```text
BUILD_BIN2C=y
DMADEVICES=y
DMA_BCM2835=y
DMA_ENGINE=y
DMA_OF=y
DMA_VIRTUAL_CHANNELS=y
IKCONFIG=y
IKCONFIG_PROC=y
MMC_BCM2835=y
MMC_BCM2835_DMA=y
MMC_BCM2835_PIO_DMA_BARRIER=2
```


<p align="center">Built with <a href="https://github.com/notro/rpi-build/wiki">rpi-build</a></p>
