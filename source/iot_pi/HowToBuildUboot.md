title: How to Build and Install custom U-boot
---

Building U-boot on I-Pi-SMARC using the LEC-PX30 SMARC module and downloading to the SDcard



## **Prerequisites**

* Development host running recent Ubuntu OS such as 18.04 with compile installed  

* Make sure it has the development environment installed :

  ```
  sudo apt install build-essential
  ```
  
* Download the PX30 buildroot SDK  [here](https://hq0epm0west0us0storage.blob.core.windows.net/development/LEC-PX30/SDK/px30_buildroot_es2_sdk_20191218.tar.gz)  to the development host (around) 8GB)

  

## **Building the binaries**

1. After downloading the SDK, extract it

2. Make sure you are in terminal mode and change directory to the u-boot directory

   ```
   $ cd px30_buildroot/u-boot
   ```

3. The SDK comes standard with buildroot optimized config file for the module in question
   If any changes are needed such as modifying the kernel type or location you can make those in the RK_UBOOT_DEFCONFIG section in px30_buildroot/u-boot/device/rockchip/.BoardConfig.mk 

4. Build U-Boot using below command: 

   ```
   $ sudo ./make.sh evb-px30
   ```



## Installing U-boot on the target

1. After a successful build you will end up with 3 binary images: 

   1. **px30_loader**_vx.xx.xxx.bin 
      this is the Rockchip miniloader flash install it to the miniloader partition on the target. 

   * **trust.img**: ARM Trusted Firmware, Please flash this binary to trust partition
   * **uboot.img**: The U-Boot image, Please flash this binary to uboot partition

   ```
   u-boot/
   ├── px30_loader_v1.11.115.bin
   ├── trust.img
   └── uboot.img
   ```













