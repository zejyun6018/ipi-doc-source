title: Ubuntu Images
---

 ### Ubuntu Bionic 18.04 LTS Xfce Desktop Environment

Boot the system with the SD card placed in the slot located on the carrier, once booted you will see the login screen

<img src="UbuntuImages.assets/Screenshot_2020-01-08_11-51-14.png" alt="Screenshot_2020-01-08_11-51-14" style="zoom: 33%;" />

Ubuntu is not available for download but has to be compiled by the user himself, please follow [the steps](https://ipi.wiki/iot_pi/HowToBuildUbuntu.html) in “build your OS” to do this.



**Note:** Note: The kernel used is not Ubuntu native. Ubuntu rootfs image which is bootstrapped by the PX30 u-boot & Kernel.



<br>

### Usernames and passwords

   * Two users are defined for use on the system: **adlink** and **root**.

   * Passwords is **adlink123** for two users.

     

<br>

### Supported features & interfaces 

* Linux Kernel version: **4.4.167**
* [40 Pin expansion Header](https://ipi.wiki/iot_pi/UserInterfaces.html) with [Eclipse Mraa library](https://github.com/eclipse/mraa) which supports C/C++, Python, JAVA and Javascript	
* USB 2.0/3.0  ports
* Two 10/100 Mb LAN ports 
* HDMI output with resolution 1920x1080@60Hz
* CAN FD Bus interface
* Analog to Digital input 
* Audio & speaker



**Note**: Rockchip PX30 ARM Mali-G31 GPU doesn't support x11 display server. Therefore, the default is Mesa GPU driver which supported on xfce Ubuntu image. 

