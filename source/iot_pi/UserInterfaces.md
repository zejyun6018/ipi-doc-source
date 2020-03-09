title:  User Interfaces
---



## Industrial -Pi SMARC with SMARC LEC-PX30 SoM


<img src="UserInterfaces.assets/UserInterface.png" style="zoom:67%;" />

|      | Component           | Description                                                  |
| ---- | :------------------ | ------------------------------------------------------------ |
| A    | LAN 1               | 10/100 Mb network connector                                  |
| B    | LAN 2               | 10/100 Mb network connector                                  |
| C    | USB 3 Type A        | USB host stacked connector                                   |
| D    | USB 2 Type A        | USB host stacked connector                                   |
| E    | 40-Pin HEADER       | RBP  compatible 40 pins signal header                        |
| F    | ADC  header         | Analog signal input                                          |
| G    | BOOT  select        | Selector  to change boot modes                               |
| H    | HDMI  port          | For  connecting external displays via HDMI (**Only for Industrial Pi**) |
| I    | Micro-SD  Card Slot | Boot OS  via Micro-SD                                        |
| J    | Power  Button       | Power on your system                                         |
| K    | CAN  bus Header     | Screw  type header for CAN bus                               |
| L    | Power Jack          | 12Vdc barrel jack ( min 2A )                                 |
| M    | USB OTG             | Micro-USB OTG port                                           |
| N    | HDMI  port          | For  connecting external displays via HDMI ( **Only for Neuron Pi** ) |
| O    | Audio Jack          | 3.5 mm Audio jack                                            |
| P    | Reset  Button       | Forcefully  reboot your system                               |



## 40 Pin Expansion Header Pin-Out


| Linux GPIO (/sys/class/gpio) | Function  | MRAA number | MRAA number | Function  | Linux GPIO (/sys/class/gpio) |
| :--------------------------: | :-------: | :---------: | :---------: | :-------: | :--------------------------: |
|                              |    3V3    |      1      |      2      |    5V     |                              |
|                              | I2C_0 SDA |      3      |      4      |    5V     |                              |
|                              | I2C_0 SCL |      5      |      6      |    GND    |                              |
|             116              |   GPIO    |      7      |      8      |  UART TX  |                              |
|                              |    GND    |      9      |     10      |  UART RX  |                              |
|             118              |   GPIO    |     11      |     12      |   GPIO    |             117              |
|             107              |   GPIO    |     13      |     14      |    GND    |                              |
|             104              |   GPIO    |     15      |     16      |   GPIO    |             109              |
|                              |    3V3    |     17      |     18      |   GPIO    |             121              |
|                              | SPI MOSI  |     19      |     20      |    GND    |                              |
|                              | SPI MISO  |     21      |     22      |   GPIO    |             122              |
|                              | SPI SCLK  |     23      |     24      |  SPI CS0  |                              |
|                              |    GND    |     25      |     26      |    n/a    |                              |
|                              | I2C_1 SDA |     27      |     28      | I2C_1 SCL |                              |
|             496              | GPIO/PWM  |     29      |     30      |    GND    |                              |
|             497              | GPIO/PWM  |     31      |     32      | GPIO/PWM  |             498              |
|             499              | GPIO/PWM  |     33      |     34      |    GND    |                              |
|             500              | GPIO/PWM  |     35      |     36      | GPIO/PWM  |             501              |
|             502              | GPIO/PWM  |     37      |     38      | GPIO/PWM  |             503              |
|                              |    GND    |     39      |     40      | GPIO/PWM  |             504              |

*The 40 pin header is compatible with Raspberry PI HAT's and is accessible via the MRAA library *



## **Power Supply**

The Industrial Pi-SMARC is powered by a 12V DC power supply, make sure this supply can reach 1.5A@12V DC.", standard a compatible power supply is delivered together with your development board



## **Displays & User Input**

Following items are needed when connecting your Ipi-SMARC to an external display  for use as a desktop computer or media center.  > HDMI 1.4 Cable  and a  (Wireless) USB Keyboard + Mouse



## **Linux OS image**

The Industrial Pi-SMARC is equipped with a MICRO SD card slot to boot a compatible operating system and OS image, this also includes MRAA Library & sample codes.
