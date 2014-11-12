pietrushnic/rpi-dt-firmware
==========

Raspberry Pi Linux kernel 3.17.2+ (ARCH_BCM2835) with additional patches.

Install
-------

```text
sudo REPO_URI=https://github.com/pietrushnic/rpi-dt-firmware rpi-update
```




Changelog
---------
2014-11-11
* switch to 3.17.2
* remove bcm2835-mmc and options related with it
* add sdhci-bcm2835 improvements by Scott Branden <sbranden@broadcom.com>

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
* [raspberrypi/tools](https://github.com/raspberrypi/tools/archive/aeb175171947230d943d61a5a375ef61041f579d.tar.gz)
* [raspberrypi/firmware](https://github.com/raspberrypi/firmware/archive/778b37038a781bed340358a9d533579756562139.tar.gz)
* [http://git.denx.de/?p=u-boot/u-boot-arm.git](http://git.denx.de/?p=u-boot/u-boot-arm.git;a=snapshot;h=868de51ddee75d65f3ca4235f97900410f424def;sf=tgz)


Patches
--------
None

Kernel config
-------------
Default config: bcm2835_defconfig



Deleted:
```text
MMC_SDHCI_BCM2835_VERIFY_WORKAROUND=y
```


<p align="center">Built with <a href="https://github.com/notro/rpi-build/wiki">rpi-build</a></p>
