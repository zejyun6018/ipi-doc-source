title: Signal Descriptions
---



## Signal Terminology Descriptions

Meaning of the terms used for signal
description tables



| **Term**    | **Description**                                              |
| ----------- | ------------------------------------------------------------ |
|             |                                                              |
| I           | Input to the module                                          |
| O           | Output from the module                                       |
| O OD        | Open drain output from the module                            |
| I OD        | Open drain input to the module, with mandatory PU   (pull up) on module |
| OD          | Open drain                                                   |
| I/O         | Bi-directional Input/Output                                  |
| PU          | PU (pull-up) resistor on module                              |
| PD          | PD (pull-down) resistor on module                            |
| VDD_IN      | Main power source  from carrier to module                    |
| CMOS        | Logic input or output                                        |
| GBE MDI     | Differential analog signaling for Gigabit Media   Dependent Interface |
| LVDS DP     | Low Voltage Differential Signal for DisplayPort   interface  |
| LVDS D-PHY  | Low Voltage Differential Signal for MIPI CSI-2 cameras   and DSI displays |
| LVDS M-PHY  | Low Voltage Differential Signal for MIPI CSI-3   cameras     |
| LVDS LCD    | Low Voltage Differential Signal for LCD displays             |
| LVDS PCIE   | Low Voltage Differential Signal for PCIe                     |
| LVDS SATA   | Low Voltage Differential Signal for SATA                     |
| TMDS HDMI   | Transition Minimized Differential Signal for HDMI   displays |
| USB         | DC coupled differential signaling for traditional   (non-Superspeed) USB signals |
| USB SS      | Differential signal for SuperSpeed USB signals               |
| USB VBUS 5V | 5V tolerant input for USB VBUS detection                     |
| 3.3V        | 3.3V Power Domain: Active while CARRIER_PWRON is   high and CARRIER_SBY# is NOT active (i.e. both signals are high) |
| 1.8V        | 1.8V Power Domain: Active while CARRIER_PWRON is   high and CARRIER_SBY# is NOT active (i.e. both signals are high) |
| 3.3Vsb      | 3.3V Power Domain: Active while CARRIER_PWRON is   high (regardless of CARRIER_SBY#) |
| 1.8Vsb      | 1.8V Power Domain: Active while CARRIER_PWRON is   high (regardless of CARRIER_SBY#) |





### First Display Interface

This is a group of 30 pins that is split
into a channel 0 and channel 1 and can support either dual channel LVDS ports,
2 separate single channel LVDS ports, 2 MIPI DSI ports of 4 lanes each or 2 eDP
ports 4 lanes each. 

Any mix of the same or different display types, such as DSI0 and eDP1, is permitted. 



| Pin #                                                        | LVDS Name                                                    | MIPI DSI Name                                                | eDP Name                                                     |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| **Channel 0**                                                |                                                              |                                                              |                                                              |
| S125<br>S126<br>S128<br>S129<br>S131<br>S132<br>S137<br>S138 | LVDS0_0+<br/>LVDS0_0-<br/>LVDS0_1+<br/>LVDS0_1-<br/>LVDS0_2+<br/>LVDS0_2-<br/>LVDS0_3+<br/>LVDS0_3- | DSI0_D0+<br>DSI0_D0-<br>DSI0_D1+<br>DSI0_D1-<br>DSI0_D2+<br>DSI0_D2-<br>DSI0_D3+<br>DSI0_D3- | ~~eDP0_TX0+<br>eDP0_TX0-<br>eDP0_TX1+<br>eDP0_TX1-<br>eDP0_TX2+<br>eDP0_TX2-<br>eDP0_TX3+<br>eDP0_TX3-~~ |
| S134<br>S135                                                 | LVDS0_CK+<br>LVDS0_CK-                                       | DSI0_CLK+<br>DSI0_CLK-                                       | eDP0_AUX+<br>eDP0_AUX-                                       |
| S133                                                         | LCD0_VDD_EN                                                  | LCD0_VDD_EN                                                  | LCD0_VDD_EN                                                  |
| S127                                                         | LCD0_BKLT_EN                                                 | LCD0_BKLT_EN                                                 | LCD0_BKLT_EN                                                 |
| S141                                                         | LCD0_BKLT_PWM                                                | LCD0_BKLT_PWM                                                | LCD0_BKLT_PWM                                                |
| S144                                                         |                                                              | DSI0_TE                                                      | eDP0_HPD                                                     |
|                                                              |                                                              |                                                              |                                                              |
| **Channel 1**                                                |                                                              |                                                              |                                                              |
| S111<br>S112<br>S114<br>S115<br>S117<br>S118<br>S120<br>S121 | ~~LVDS1_0+<br>LVDS1_0-<br>LVDS1_1+<br>LVDS1_1 -<br>LVDS1_2+<br>LVDS1_2-<br>LVDS1_3+<br>LVDS1_3-~~ | ~~DSI1_D0+<br>DSI1_D0-<br>DSI1_D1+<br>DSI1_D1-<br>DSI1_D2+<br>DSI1_D2-<br>DSI1_D3+<br>DSI1_D3-~~ | ~~eDP1_TX0+<br>eDP1_TX0-<br>eDP1_TX1+<br>eDP1_TX1-<br>eDP1_TX2+<br>eDP1_TX2-<br>eDP1_TX3+<br>eDP1_TX3~~- |
| S108<br>S109                                                 | ~~LVDS1_CK+<br>LVDS1_CK-~~                                   | ~~DSI1_CLK+<br>DSI1_CLK-~~                                   | ~~eDP1_AUX+<br>eDP1_AUX-~~                                   |
| S116                                                         | ~~LCD1_VDD_EN~~                                              | ~~LCD1_VDD_EN~~                                              | ~~LCD1_VDD_EN~~                                              |
| S107                                                         | ~~LCD1_BKLT_EN~~                                             | ~~LCD1_BKLT_EN~~                                             | ~~LCD1_BKLT_EN~~                                             |
| S122                                                         | ~~LCD1_BKLT_PWM~~                                            | ~~LCD1_BKLT_PWM~~                                            | ~~LCD1_BKLT_PWM~~                                            |
| S113                                                         |                                                              | ~~DSI1_TE~~                                                  | ~~eDP1_HPD~~                                                 |
|                                                              |                                                              |                                                              |                                                              |
| **Shared I2C Channel 0/1**                                   |                                                              |                                                              |                                                              |
| S139                                                         | I2C_LCD_CK                                                   | I2C_LCD_CK                                                   | I2C_LCD_CK                                                   |
| S140                                                         | I2C_LCD_DAT                                                  | I2C_LCD_DAT                                                  | I2C_LCD_DAT                                                  |





