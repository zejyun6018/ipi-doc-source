title: How to flash Yocto image to SD Card
---

The procedure to describes how to flash the image with u-boot, Linux kernel and filesystem to the SD Card



## Prerequisites

- Copy the prebuilt bootable Linux image to the working directory on your development host.
- In Windows environment, please download [Rockchip SD Firmware tool](https://hq0epm0west0us0storage.blob.core.windows.net/development/LEC-PX30/Tools/SDDiskTool_v1.6.rar) to flash image to SD Card

​       **Note:** All of files will be erased on SD Card. The size should be at least 16 Gb.




### Windows Host:

Insert an empty MicroSD Card into development host and execute Rockhip SD Firmware tool. in the below, 

* Select "Choose removable disk" as your SD card

* Choose "Function mode" as **SD Boot**

* Lod your build Yocto image as "Firmware" 

then, click "Create button" to start.


![image-20200302114938191](HowToFlashYoctoImage.assets/image-20200302114938191.png)




Now, remove the SDcard and insert it into the SDcard slot on the carrier.

**Note**: There is no need to configure the boot selector of **LEC-PX30 with Industrial-Pi** for SDcard booting. You can directly insert SD card and power on the system.

