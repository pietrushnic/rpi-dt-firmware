pietrushnic/rpi-dt-firmware
==========

Raspberry Pi Linux kernel 3.17.1+ (ARCH_BCM2835) with additional patches.

Install
-------

```text
sudo REPO_URI=https://github.com/pietrushnic/rpi-dt-firmware rpi-update
```




Changelog
---------
2014-10-28
* switch to 3.17.1
* add slave_sg for bcm2835-dma
* replace sdhci-bcm2835 with bcm2835-mmc
* fix issue with bcm2835-cpufreq with incorrect mbox status register in tx_done and send_data
* move DMA, MMC and IKCONFIG options to bcm2835_defconfig

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
* [raspberrypi/tools](https://github.com/raspberrypi/tools/archive/719ac36e09bbc30350e978a20c2828245222feed.tar.gz)
* [raspberrypi/firmware](https://github.com/raspberrypi/firmware/archive/5711461a29add5bf9e5f5c9dfc08aa12cdf0f19f.tar.gz)
* [http://git.denx.de/?p=u-boot/u-boot-arm.git](http://git.denx.de/?p=u-boot/u-boot-arm.git;a=snapshot;h=59a9cfdd16ad7ab14f22697bf1e049c6bea0d3e2;sf=tgz)


Patches
--------
None

Kernel config
-------------
Default config: bcm2835_defconfig



<p align="center">Built with <a href="https://github.com/notro/rpi-build/wiki">rpi-build</a></p>
