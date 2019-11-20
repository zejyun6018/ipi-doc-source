title: Module Introduction 
---

# LEC-PX30



![](HardwareDocs.assets/1566663260263.png)



![1566663628574](HardwareDocs.assets/1566663628574.png)

# 

## The SMARC Formfactor

The SMARC (“Smart Mobility ARChitecture”) is a versatile small form factor computer on Module definition targeting applications that require low power, low costs, and high performance. The Modules will typically use ARM SOCs similar or the same as those used in many familiar devices such as tablet computers and smart phones. Alternative low power SOCs and CPUs, such as tablet oriented X86 devices and other RISC CPUs may be used as well. The Module power envelope is typically under 6W.

Two Module sizes are defined: 82 mm x 50 mm and 82 mm x 80 mm. 

The Module PCBs have 314 edge fingers that mate with a low profile 314 pin 0.5 mm pitch right angle connector (the connector is sometimes identified as a 321 pin connector, but 7 pins are lost to the key).

The Modules are used as building blocks for portable and stationary embedded systems. The core CPU and support circuits, including DRAM, boot flash, power sequencing, CPU power supplies, GBE and a single channel LVDS display transmitter are concentrated on the Module. The Modules are used with application specific Carrier Boards that implement other features such as audio CODECs, touch controllers, wireless devices, etc. The modular approach allows scalability, fast time to market and upgradability while still maintaining low costs, low power and small physical size.

![1566664079224](HardwareDocs.assets/1566664079224.png)



SMARC module and carrier specifications are
available online at :    https://www.sget.org/standards/smarc.html





## Specifications



### Core System

**SoC**

Rockchip PX30 with Quad-core ARM Cortex-A35 CPU TrustZone technology support ARMv8 Cryptography Extensions”



**Memory**

1GB or 2GB DDR3L at 1066/1333 MHz, memory down (non ECC)



**L2 Cache**

256KB unified system L2 cache

 

**IoT security**

CryptoAuthentication™ Device, Microchip ATECC608A

Cryptographic co-processor with secure hardware-based key storage for sign-verify authentication provides Internet of Things (IoT) Protected 
Storage for up to 16 keys, certificates or data ECDH: FIPS SP800-56A Elliptic Curve Diffie-Hellman NIST standard P256, elliptic curve support SHA-256 & HMAC hash including off-chip context save/restore AES-128: encrypt/decrypt, galois field multiply for GCM”

 

## Video

LEC-PX30 standard display support is limited to either 4-lane MIPI DSI or single channel 24-bit LVDS. DSI and LVDS are multiplexed and either of them can simply be enabled at boot time.  HDMI panel support up to 1920x1080 resolution can be achieved by using a simple bridge on the carrier. A reference design based on ADV7335 “MIPI/DSI Receiver with HDMI Transmitter” is available

 

**GPU Core:** 

Mali-G31



**GPU Feature Support**

Supports DirectX 11 FL9_3, OpenGLES 1.1/ 2.0 / 3.2, Vulkan 1.0, OpenCL 2.0

Full Profile Video decoding: H.264 up to 1080p@60fps, H.265/HEVC up to 1080p@60fps

MPEG-4, ISO/IEC 14496-2, SP@L0-3, ASP@L0-5, up to 1080p@60fps VP8, up to 1080p@60fps

Video Encoding: H.264 video encoder at BP/MP/HP@level 4.2 1920x1080@30fps, 1x 1080p@30fps or 2x 720p@30fps encoding

 

**MIPI DSI**

MIPI DSI 4 lanes at max. 1080p@60fps display output (default, multiplexed with LVDS signal) 

 

**LVDS**

LVDS single channel 24-bit at max. 1280x800@60fps (multiplexed with MIPI DSI signal)

 

**Camera**

MIPI CSI RX Interface

\- Compatible with the MIPI Alliance Interface specification v1.0

\- Up to 4 data lanes, 1.0Gbps maximum data rate per lane, supporting MIPI-HS, MIPI-LP mode





