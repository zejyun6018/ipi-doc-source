title: How to Build U-boot
---

The procedure to describes how to build u-boot for LEC-PX30.



## **Prerequisites**

* Please click [here](https://hq0epm0west0us0storage.blob.core.windows.net/development/LEC-PX30/SDK/px30_buildroot_es2_sdk_20191218.tar.gz) to download PX30 buildroot SDK on the development host PC with Ubuntu OS

  

## **Getting Started**

1. After download SDK, please extract it

2. Change directory to u-boot

   ```
   $ cd px30_buildroot/u-boot
   ```

3. For LEC-PX30 board. Use below command to build the U-Boot: 

   ```
   $ sudo ./make.sh evb-px30
   ```

    **Note**: It will use RK_UBOOT_DEFCONFIG in device/rockchip/.BoardConfig.mk to build U-Boot. Please modify RK_UBOOT_DEFCONFIG if it don't match your board. 
   
   
   
4. It will generate 3 binary image: px30_loader_vx.xx.xxx.bin, trust.img, uboot.img. 

   * **px30_loader_vx.xx.xxx.bin**: Rockchip miniloader. Please flash this binary to miniloader partition. 
   * **trust.img**: ARM Trusted Firmware, Please flash this binary to trust partition
   * **uboot.img**: The U-Boot image, Please flash this binary to uboot partition

   ```
u-boot/
├── px30_loader_v1.11.115.bin
├── trust.img
└── uboot.img
   ```
   

