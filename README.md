pietrushnic/rpi-dt-firmware
==========

Raspberry Pi Linux kernel 3.16.4+ (ARCH_BCM2835) with additional patches.

Install
-------

```text
sudo REPO_URI=https://github.com/pietrushnic/rpi-dt-firmware rpi-update
```




Changelog
---------
2014-09-28:
* First release

Links
* [Upstreaming](https://github.com/raspberrypi/linux/wiki/Upstreaming)
* [Device Tree on ARCH_BCM2708](https://github.com/raspberrypi/linux/wiki/Device-Tree-on-ARCH_BCM2708)



Sources
-------
* [raspberrypi/tools](https://github.com/raspberrypi/tools/archive/f8e07cca589beb7c2cba6c4d4ab7a404fe91e8d3.tar.gz)
* [raspberrypi/firmware](https://github.com/raspberrypi/firmware/archive/c786f85ea2495ca8ae239fb9575fbc1d85fb381e.tar.gz)
* [http://git.denx.de/?p=u-boot/u-boot-arm.git](http://git.denx.de/?p=u-boot/u-boot-arm.git;a=snapshot;h=be9f643ae6aa9044c60fe80e3a2c10be8371c692;sf=tgz)
* [linux-3.16.4.tar.xz](https://www.kernel.org/pub/linux/kernel/v3.x/linux-3.16.4.tar.xz)


Patches
--------
* /home/pietrushnic/src/rpi-bcm2835/patches/0001_mailbox__rename_pl320-ipc_specific_mailbox.h.patch
* /home/pietrushnic/src/rpi-bcm2835/patches/0002_mailbox__Introduce_framework_for_mailbox.patch
* /home/pietrushnic/src/rpi-bcm2835/patches/0003_doc__add_documentation_for_mailbox_framework.patch
* /home/pietrushnic/src/rpi-bcm2835/patches/0004_dt__mailbox__add_generic_bindings.patch
* /home/pietrushnic/src/rpi-bcm2835/patches/0020_ARM__bcm2835__Enable_USB_DWC2_HOST_in_bcm2835_defconfig.patch
* /home/pietrushnic/src/rpi-bcm2835/patches/0040_MMC__added_alternative_MMC_driver.patch
* /home/pietrushnic/src/rpi-bcm2835/patches/0041_dt_bcm2835_add_mmc_node.patch


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
