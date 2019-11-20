title: Pinout Summary
---



## Edge Connector supported singals





The below table is a comprehensible list of
all signal pins on the MXM 3 connector in the standard specification SMARC 2.1.



Those signals not supported on LEC-PX30 are strikethrough ~~STRIKETHROUGH~~  





![1566748596672](PinoutSummary.assets/1566748596672.png)                ![1566748622830](PinoutSummary.assets/1566748622830.png)



| P-Pin | Primary    (Top) Side    |      | S-Pin | Secondary    (Bottom) Side        |
| ----- | ------------------------ | ---- | ----- | --------------------------------- |
|       |                          |      | S1    | ~~CSI1_TX+ / I2C_CAM1_CK~~        |
| P1    | ~~SMB_ALERT_1V8#~~       |      | S2    | ~~CSI1_TX- / I2C_CAM1_DAT~~       |
| P2    | GND                      |      | S3    | GND                               |
| P3    | CSI1_CK+                 |      | S4    | RSVD                              |
| P4    | CSI1_CK-                 |      | S5    | CSI0_TX- / I2C_CAM0_CK            |
| P5    | GBE1_SDP                 |      | S6    | CAM_MCK                           |
| P6    | GBE0_SDP                 |      | S7    | CSI0_TX+ / I2C_CAM0_DAT           |
| P7    | ~~CSI1_RX0+~~            |      | S8    | CSI0_CK+                          |
| P8    | ~~CSI1_RX0-~~            |      | S9    | CSI0_CK-                          |
| P9    | GND                      |      | S10   | GND                               |
| P10   | ~~CSI1_RX1+~~            |      | S11   | CSI0_RX0+                         |
| P11   | ~~CSI1_RX1-~~            |      | S12   | CSI0_RX0-                         |
| P12   | GND                      |      | S13   | GND                               |
| P13   | ~~CSI1_RX2+~~            |      | S14   | CSI0_RX1+                         |
| P14   | ~~CSI1_RX2-~~            |      | S15   | CSI0_RX1-                         |
| P15   | GND                      |      | S16   | GND                               |
| P16   | ~~CSI1_RX3+~~            |      | S17   | GBE1_MDI0+                        |
| P17   | ~~CSI1_RX3-~~            |      | S18   | GBE1_MDI0-                        |
| P18   | GND                      |      | S19   | GBE1_LINK100#                     |
| P19   | ~~GBE0_MDI3-~~           |      | S20   | GBE1_MDI1+                        |
| P20   | ~~GBE0_MDI3+~~           |      | S21   | GBE1_MDI1-                        |
| P21   | GBE0_LINK100#            |      | S22   | ~~GBE1_LINK1000#~~                |
| P22   | ~~GBE0_LINK1000#~~       |      | S23   | GBE1_MDI2+                        |
| P23   | GBE0_MDI2-               |      | S24   | GBE1_MDI2-                        |
| P24   | GBE0_MDI2+               |      | S25   | GND                               |
| P25   | GBE0_LINK_ACT#           |      | S26   | ~~GBE1_MDI3+~~                    |
| P26   | GBE0_MDI1-               |      | S27   | ~~GBE1_MDI3-~~                    |
| P27   | GBE0_MDI1+               |      | S28   | ~~GBE1_CTREF~~                    |
| P28   | ~~GBE0_CTREF~~           |      | S29   | PCIE_D_TX+ / SERDES_1_TX+         |
| P29   | GBE0_MDI0-               |      | S30   | PCIE_D_TX- / SERDES_1_TX-         |
| P30   | GBE0_MDI0+               |      | S31   | GBE1_LINK_ACT#                    |
| P31   | SPI0_CS1#                |      | S32   | PCIE_D_RX+ / SERDES_1_RX+         |
| P32   | GND                      |      | S33   | PCIE_D_RX- / SERDES_1_RX-         |
| P33   | SDIO_WP                  |      | S34   | GND                               |
| P34   | SDIO_CMD                 |      | S35   | USB4+                             |
| P35   | SDIO_CD#                 |      | S36   | USB4-                             |
| P36   | SDIO_CK                  |      | S37   | USB3_VBUS_DET                     |
| P37   | SDIO_PWR_EN              |      | S38   | AUDIO_MCK                         |
| P38   | GND                      |      | S39   | I2S0_LRCK                         |
| P39   | SDIO_D0                  |      | S40   | I2S0_SDOUT                        |
| P40   | SDIO_D1                  |      | S41   | I2S0_SDIN                         |
| P41   | SDIO_D2                  |      | S42   | I2S0_CK                           |
| P42   | SDIO_D3                  |      | S43   | ESPI_ALERT0#                      |
| P43   | SPI0_CS0#                |      | S44   | ESPI_ALERT1#                      |
| P44   | SPI0_CK                  |      | S45   | MDIO_CLK                          |
| P45   | SPI0_DIN                 |      | S46   | MDIO_DAT                          |
| P46   | SPI0_DO                  |      | S47   | GND                               |
| P47   | GND                      |      | S48   | I2C_GP_CK                         |
| P48   | ~~SATA_TX+~~             |      | S49   | I2C_GP_DAT                        |
| P49   | ~~SATA_TX-~~             |      | S50   | HDA_SYNC / I2S2_LRCK              |
| P50   | GND                      |      | S51   | HDA_SDO / I2S2_SDOUT              |
| P51   | ~~SATA_RX+~~             |      | S52   | HDA_SDI / I2S2_SDIN               |
| P52   | ~~SATA_RX-~~             |      | S53   | HDA_CK / I2S2_CK                  |
| P53   | GND                      |      | S54   | SATA_ACT#                         |
| P54   | ESPI_CS0# / SPI1_CS0#    |      | S55   | USB5_EN_OC#                       |
| P55   | ESPI_CS1# / SPI1_CS1#    |      | S56   | ESPI_IO_2                         |
| P56   | ESPI_CK / SPI1_CK        |      | S57   | ESPI_IO_3                         |
| P57   | ESPI_IO_1 / SPI1_DIN     |      | S58   | ESPI_RESET#                       |
| P58   | ESPI_IO_0 / SPI1_DO      |      | S59   | USB5+                             |
| P59   | GND                      |      | S60   | USB5-                             |
| P60   | USB0+                    |      | S61   | GND                               |
| P61   | USB0-                    |      | S62   | USB3_SSTX+                        |
| P62   | USB0_EN_OC#              |      | S63   | USB3_SSTX-                        |
| P63   | USB0_VBUS_DET            |      | S64   | GND                               |
| P64   | USB0_OTG_ID              |      | S65   | USB3_SSRX+                        |
| P65   | USB1+                    |      | S66   | USB3_SSRX-                        |
| P66   | USB1-                    |      | S67   | GND                               |
| P67   | USB1_EN_OC#              |      | S68   | USB3+                             |
| P68   | GND                      |      | S69   | USB3-                             |
| P69   | USB2+                    |      | S70   | GND                               |
| P70   | USB2-                    |      | S71   | USB2_SSTX+                        |
| P71   | USB2_EN_OC#              |      | S72   | USB2_SSTX-                        |
| P72   | RSVD                     |      | S73   | GND                               |
| P73   | RSVD                     |      | S74   | USB2_SSRX+                        |
| P74   | USB3_EN_OC#              |      | S75   | USB2_SSRX-                        |
|       |                          |      |       |                                   |
|       | Key                      |      |       | Key                               |
|       |                          |      |       |                                   |
| P75   | PCIE_A_RST#              |      | S76   | PCIE_B_RST#                       |
| P76   | USB4_EN_OC#              |      | S77   | PCIE_C_RST#                       |
| P77   | PCIE_B_CKREQ#            |      | S78   | PCIE_C_RX+ / SERDES_2_RX+         |
| P78   | PCIE_A_CKREQ#            |      | S79   | PCIE_C_RX- / SERDES_2_RX-         |
| P79   | GND                      |      | S80   | GND                               |
| P80   | PCIE_C_REFCK+            |      | S81   | PCIE_C_TX+ / SERDES_2_TX+         |
| P81   | PCIE_C_REFCK-            |      | S82   | PCIE_C_TX- / SERDES_2_TX-         |
| P82   | GND                      |      | S83   | GND                               |
| P83   | PCIE_A_REFCK+            |      | S84   | PCIE_B_REFCK+                     |
| P84   | PCIE_A_REFCK-            |      | S85   | PCIE_B_REFCK-                     |
| P85   | GND                      |      | S86   | GND                               |
| P86   | PCIE_A_RX+               |      | S87   | PCIE_B_RX+                        |
| P87   | PCIE_A_RX-               |      | S88   | PCIE_B_RX-                        |
| P88   | GND                      |      | S89   | GND                               |
| P89   | PCIE_A_TX+               |      | S90   | PCIE_B_TX+                        |
| P90   | PCIE_A_TX-               |      | S91   | PCIE_B_TX-                        |
| P91   | GND                      |      | S92   | GND                               |
| P92   | HDMI_D2+ / DP1_LANE0+    |      | S93   | DP0_LANE0+                        |
| P93   | HDMI_D2- / DP1_LANE0-    |      | S94   | DP0_LANE0-                        |
| P94   | GND                      |      | S95   | DP0_AUX_SEL                       |
| P95   | HDMI_D1+ / DP1_LANE1+    |      | S96   | DP0_LANE1+                        |
| P96   | HDMI_D1- / DP1_LANE1-    |      | S97   | DP0_LANE1-                        |
| P97   | GND                      |      | S98   | DP0_HPD                           |
| P98   | HDMI_D0+ / DP1_LANE2+    |      | S99   | DP0_LANE2+                        |
| P99   | HDMI_D0- / DP1_LANE2-    |      | S100  | DP0_LANE2-                        |
| P100  | GND                      |      | S101  | GND                               |
| P101  | HDMI_CK+ / DP1_LANE3+    |      | S102  | DP0_LANE3+                        |
| P102  | HDMI_CK- / DP1_LANE3-    |      | S103  | DP0_LANE3-                        |
| P103  | GND                      |      | S104  | USB3_OTG_ID                       |
| P104  | HDMI_HPD / DP1_HPD       |      | S105  | DP0_AUX+                          |
| P105  | HDMI_CTRL_CK / DP1_AUX+  |      | S106  | DP0_AUX-                          |
| P106  | HDMI_CTRL_DAT / DP1_AUX- |      | S107  | LCD1_BKLT_EN                      |
| P107  | DP1_AUX_SEL              |      | S108  | LVDS1_CK+ / eDP1_AUX+ / DSI1_CLK+ |
| P108  | GPIO0 / CAM0_PWR#        |      | S109  | LVDS1_CK- / eDP1_AUX- / DSI1_CLK- |
| P109  | GPIO1 / CAM1_PWR#        |      | S110  | GND                               |
| P110  | GPIO2 / CAM0_RST#        |      | S111  | LVDS1_0+ / eDP1_TX0+ / DSI1_D0+   |
| P111  | GPIO3 / CAM1_RST#        |      | S112  | LVDS1_0- / eDP1_TX0- / DSI1_D0-   |
| P112  | GPIO4 / HDA_RST#         |      | S113  | eDP1_HPD / DSI1_TE                |
| P113  | GPIO5 / PWM_OUT          |      | S114  | LVDS1_1+ / eDP1_TX1+ / DSI1_D1+   |
| P114  | GPIO6 / TACHIN           |      | S115  | LVDS1_1- / eDP1_TX1- / DSI1_D1-   |
| P115  | GPIO7                    |      | S116  | LCD1_VDD_EN                       |
| P116  | GPIO8                    |      | S117  | LVDS1_2+ / eDP1_TX2+ / DSI1_D2+   |
| P117  | GPIO9                    |      | S118  | LVDS1_2- / eDP1_TX2- / DSI1_D2-   |
| P118  | GPIO10                   |      | S119  | GND                               |
| P119  | GPIO11                   |      | S120  | LVDS1_3+ / eDP1_TX3+ / DSI1_D3+   |
| P120  | GND                      |      | S121  | LVDS1_3- / eDP1_TX3- / DSI1_D3-   |
| P121  | I2C_PM_CK                |      | S122  | LCD1_BKLT_PWM                     |
| P122  | I2C_PM_DAT               |      | S123  | GPIO13                            |
| P123  | BOOT_SEL0#               |      | S124  | GND                               |
| P124  | BOOT_SEL1#               |      | S125  | LVDS0_0+ / eDP0_TX0+ / DSI0_D0+   |
| P125  | BOOT_SEL2#               |      | S126  | LVDS0_0- / eDP0_TX0- / DSI0_D0-   |
| P126  | RESET_OUT#               |      | S127  | LCD0_BKLT_EN                      |
| P127  | RESET_IN#                |      | S128  | LVDS0_1+ / eDP0_TX1+ / DSI0_D1+   |
| P128  | POWER_BTN#               |      | S129  | LVDS0_1- / eDP0_TX1- / DSI0_D1-   |
| P129  | SER0_TX                  |      | S130  | GND                               |
| P130  | SER0_RX                  |      | S131  | LVDS0_2+/eDP0_TX2+/ DSI0_D2+      |
| P131  | SER0_RTS#                |      | S132  | LVDS0_2- / eDP0_TX2- / DSI0_D2-   |
| P132  | SER0_CTS#                |      | S133  | LCD0_VDD_EN                       |
| P133  | GND                      |      | S134  | LVDS0_CK+/eDP0_AUX/ DSI0_CLK+     |
| P134  | SER1_TX                  |      | S135  | LVDS0_CK-/eDP0_AUX-/ DSI0_CLK-    |
| P135  | SER1_RX                  |      | S136  | GND                               |
| P136  | SER2_TX                  |      | S137  | LVDS0_3+ / eDP0_TX3+ / DSI0_D3+   |
| P137  | SER2_RX                  |      | S138  | LVDS0_3- / eDP0_TX3- / DSI0_D3-   |
| P138  | SER2_RTS#                |      | S139  | I2C_LCD_CK                        |
| P139  | SER2_CTS#                |      | S140  | I2C_LCD_DAT                       |
| P140  | SER3_TX                  |      | S141  | LCD0_BKLT_PWM                     |
| P141  | SER3_RX                  |      | S142  | GPIO12                            |
| P142  | GND                      |      | S143  | GND                               |
| P143  | CAN0_TX                  |      | S144  | eDP0_HPD / DSI0_TE                |
| P144  | CAN0_RX                  |      | S145  | WDT_TIME_OUT#                     |
| P145  | CAN1_TX                  |      | S146  | PCIE_WAKE#                        |
| P146  | CAN1_RX                  |      | S147  | VDD_RTC                           |
| P147  | VDD_IN                   |      | S148  | LID#                              |
| P148  | VDD_IN                   |      | S149  | SLEEP#                            |
| P149  | VDD_IN                   |      | S150  | VIN_PWR_BAD#                      |
| P150  | VDD_IN                   |      | S151  | CHARGING#                         |
| P151  | VDD_IN                   |      | S152  | CHARGER_PRSNT#                    |
| P152  | VDD_IN                   |      | S153  | CARRIER_STBY#                     |
| P153  | VDD_IN                   |      | S154  | CARRIER_PWR_ON                    |
| P154  | VDD_IN                   |      | S155  | FORCE_RECOV#                      |
| P155  | VDD_IN                   |      | S156  | BATLOW#                           |
| P156  | VDD_IN                   |      | S157  | TEST#                             |
|       |                          |      | S158  | GND                               |