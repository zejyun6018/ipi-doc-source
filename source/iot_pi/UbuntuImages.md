title: Ubuntu Images
---

 ### Ubuntu Bionic 18.04 LTS Xfce Desktop Environment

<img src="UbuntuImages.assets/Screenshot_2020-01-08_11-51-14.png" alt="Screenshot_2020-01-08_11-51-14" style="zoom: 33%;" />

Please place SD card into the slot for your development kit. After the bootup for a while, you will see the above screen. If your kit arrived without SD card contact your distributor to obtain one.



**Note**: This kernel is not native from Ubuntu. Here is the [instructions](https://ipi.wiki/iot_pi/HowToBuildUbuntu.html) to build Ubuntu rootfs image which is attached to PX30 u-boot & Kernel.



<br>

### Usernames and passwords

   * Two users are defined for use on the system: **adlink** and **root**.

   * Passwords is **adlink123** for two users.

     

<br>

### What's feature enabled:

* Linux Kernel version: **4.4.167**
* [40 Pin expansion Header](https://ipi.wiki/iot_pi/UserInterfaces.html) with [Eclipse Mraa library](https://github.com/eclipse/mraa) which supports C/C++, Python, JAVA and Javascript	
* USB 2.0/3.0  ports
* Two 10/100 Mb LAN ports 
* HDMI output with resolution 1920x1080@60Hz
* CAN FD Bus interface
* Analog to Digital input 
* Audio & speaker



**Note**: From [Rockchip document wiki page, **ARM Mali-G31 GPU** doesn't support x11 display server. Therefore, the default is Mesa GPU driver which supported on xfce Ubuntu image. 

