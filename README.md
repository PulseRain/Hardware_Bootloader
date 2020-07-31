# Hardware_Bootloader
Hardware Based Bootloader for MCU

Traditionally, bootloaders are implemented in software, where the bootloader is the first piece of software to run. And most Arduino official boards, such as Arduino UNO Rev3 take this approach.

![Software Bootloader](https://github.com/PulseRain/Hardware_Bootloader/raw/master/doc/software_bootloader.png "Software Bootloader")

However, the drawback of this approach is that we have to find a way to put the bootloader into the non-volatile memory. Due to the the wide variety of FPGA based platforms, sometimes it is just infeasible, if not impossible to do so.

And the hardware based (RTL based) solution presented here takes the problem from a different vantage point, as illustrated below.


![Hardware Bootloader](https://github.com/PulseRain/Hardware_Bootloader/raw/master/doc/hardware_bootloader.png "Hardware Bootloader")

With this approach, a script will be executed on the host side to work with the hardware based bootloader inside FPGA, as shown below:

![MCU Config](https://github.com/PulseRain/Hardware_Bootloader/raw/master/doc/mcu_config.png "MCU Config")
