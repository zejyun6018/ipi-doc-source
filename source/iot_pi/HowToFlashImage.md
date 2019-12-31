title: How to flash image to SD Card
---

The procedure to describes how to flash the image to the SD Card



## Prerequisites



- Copy the prebuilt bootable Linux image to the working directory on your development host.
- In Windows environment, please download [rufus](https://rufus.ie/) to flash image to SD Card


## Getting Started

This procedure describes how to install u-boot, Linux kernel and filesystem images to MicroSD Card.

​       **Note:** All of files will be erased on MicroSD Card. The size should be at least 16 Gb.


### Windows Host:

1. Insert an empty MicroSD Card into development host and execute rufus.exe as the below. it will auto-detected your storage.

<img align="center" src="HowToFlashImage.assets/rufus_1.png" style="zoom: 67%;" />



2. Press **SELECT button** and browse to the .img previously copied to your working directory on the development host and click **START**, wait for the process to be finished.

<img align="center" src="HowToFlashImage.assets/rufus_2.png" alt="win32diskimager_load_image" style="zoom: 67%;" />




### Linux Host:

1. Insert an empty SD Card into development host and enter the following command to copy .img to MicroSD Card

   ```
   $ sudo dd if=[your image].img of=/dev/sd[x]
   ```
   
   **Note**: please look for the location of MicroSD card device, such as /dev/sdb or /dev/sda and also verify the correct device name. if writing to the wrong device, it might result in data loss
   
   
   
2. After done, please enter the following command

   ```
   $ sync
   ```
   



Insert the prepared MicroSD card into the MicroSD card slot on the carrier. 



**Note**: No need to configure on Boot selector of **LEC-PX30 with Industrial-Pi** for MicroSD card Booting. Only directly insert MicroSD Card and power on.

<img class="center" src="HowToFlashImage.assets/switch.png" style="zoom: 67%;" />