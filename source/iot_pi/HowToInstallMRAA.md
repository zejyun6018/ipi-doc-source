title: How to Install MRAA Library
---

Eclipse Mraa (Libmraa) is a C/C++ library with bindings to Java, Python and JavaScript to interface with the IO, with a structured and sensors API where port names/numbering matches the board that you are on. Use of libmraa does not tie you to specific hardware with board detection done at runtime you can create portable code that will work across the supported platforms.

The intent is to make it easier for developers and sensor manufacturers to map their sensors & actuators on top of supported hardware and to allow control of low level communication protocol by high level languages & constructs.

Our MRAA libraries has been ready on [**Eclipse MRAA GitHub**]( https://github.com/eclipse/mraa) to support **LEC-PX30 & LEC-AL-AI with industrial Pi-SMARC** as the following screen:



**Note:** By default, MRAA library is already on PX30 Yocto image & also mentioned in the section of Ubuntu instruction . 



## How to Build MRAA on your boards:

Please refer to [here](https://github.com/eclipse/mraa/blob/master/docs/building.md) to guide you how to build MRAA
