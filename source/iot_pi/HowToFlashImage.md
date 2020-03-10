title: How to Flash image to SD Card
---

The procedure to describes how to flash **Ubuntu/Yocto** image with u-boot, Linux kernel and filesystem to the SD Card



<br>

## To Flash Ubuntu Image

### Prerequisites

- Copy the prebuilt bootable Linux image to the working directory on your development host.
- In Windows environment, please download [rufus](https://rufus.ie/) to flash image to SD Card

​       **Note:** All files will be erased on SD Card. The size should be preferable 16 Gb or larger, a class 10 SD card or higher advised

<br>

### Windows Host:

1. Insert an empty MicroSD Card into the development host and execute rufus.exe as the below. it will auto-detected your storage.

<img align="center" src="HowToFlashImage.assets/rufus_1.png" style="zoom: 67%;" />



2. Press **SELECT button** and browse to the .img previously copied to your working directory on the development host and click **START**, wait for the process to be finished.

<img align="center" src="HowToFlashImage.assets/rufus_2.png" alt="win32diskimager_load_image" style="zoom: 67%;" />




### Linux Host:

1. Copy the prebuilt bootable Linux image to the working directory on your development host.Insert an empty SD Card into development host and enter the following command to copy .img to SDcard
   
   ```
   $ sudo dd if=[your image].img of=/dev/sd[x]
   ```
   
   **Warning**: Make sure the SDcard device is properly identified as /dev/sdb or /dev/sda  and verify that the device name is correct. Data loss may result if written to wrong device. 
   
2. After it completes, please enter the following command

   ```
   $ sync
   ```



<br>



## To Flash Yocto Image

### Prerequisites

- Copy the prebuilt bootable Linux image to the working directory on your development host.
- In Windows environment, please download [Rockchip SD Firmware tool](https://hq0epm0west0us0storage.blob.core.windows.net/development/LEC-PX30/Tools/SDDiskTool_v1.6.rar) to flash image to SD Card

​       **Note:** All files will be erased on SD Card. The size should be preferable 16 Gb or larger, a class 10 SD card or higher advised


<br>

### Windows Host:

Insert an empty MicroSD Card into the development host and execute Rockhip SD Firmware tool. in the below window; 

* Run **SD Firmware Tool**  as a administrator.

* Select "Choose removable disk" as your SD card

* Choose "Function mode" as **SD Boot**

* Lod your build Yocto image as "Firmware" 

then, click "Create button" to start.

<img src="HowToFlashImage.assets/image-20200303115215481.png" alt="image-20200303115215481" style="zoom:80%;" />

* It will prompt user that data will be lost. Select "Yes" to continue.
* Once done, click "OK" and close SD Firmware Tool. Eject SD card and insert in LEC-PX30 board and power on the board to boot up.




Now, remove the SDcard and insert it into the SDcard slot on the carrier.

**Note**: There is no need to configure the boot selector of **LEC-PX30 with Industrial-Pi** for SDcard booting. You can directly insert SD card and power on the system.

