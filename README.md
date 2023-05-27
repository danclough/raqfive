# The RaQFive Project
A project to restore and repurpose Cobalt RaQ servers as a modern low-power web appliance

## Project Summary
RaQFive is a project aimed at restoring and repurposing Cobalt RaQ servers. This project seeks to breathe new life into this legacy form factor by transforming a RaQ server into a functional server appliance with a fast and open RISC-V processor and a modern, secure operating system.

## Table of Contents
* [Introduction](./#Introduction)
* [Usage](./#Usage)
* [Contributing](./#Contributing)
* [License](./#License)

## Introduction

Cobalt RaQ servers were once popular web hosting appliances in the early 2000s. However, with advancements in software and hardware, these servers became outdated and were eventually abandoned. The RaQFive project aims to revive these machines by retrofitting them with new hardware.  A retrofitted RaQFive server will be an ideal platform for running a web server stack or serving as a development environment.

## Hardware
The RaQFive project is a combination of open hardware and software components to replace proprietary parts of the Cobalt RaQ platform.

The motherboard will be a StarFive VisionFive 2 RISC-V Single Board Computer.  The RISC-V architecture was specifically chosen to bring the Cobalt RaQ back to its roots as a RISC system, as the original RaQ and RaQ 2 were based on the MIPS R5000 processor.  The VisionFive 2 is comparable in performance to a Raspberry Pi 4 but offers more connectivity options and interfaces in the form of dual Gigabit Ethernet, NVMe storage, and eMMC.

The Cobalt RaQ's front panel featured an integrated 1602 LCD display and menu buttons for monitoring and servicing the system.  The original system's front panel was connected via a parallel interface with a ribbon cable.

The RaQFive will replace all of the front panel components with modern equivalents - a newer 1602 LCD, status LEDs, and menu buttons, all interfacing with the system over the two-wire I2C protocol.  Additionally, the front panel will also provide a hardware clock RTC module over I2C to maintain the system clock across reboots.

All of the hardware designs for the RaQFive, including a modified front panel LCD bracket and the front panel PCB, will be released under the CERN Open Hardware License.  All CAD models, schematics, and PCB layouts will be made available to allow anyone to build their own RaQFive system.

## Software
The RaQFive project will also cover software for interfacing with the new hardware components, including drivers for status LEDs, displaying information via the LCD module, and interfacing with the system via the front panel buttons.  The code will be released through this project repository under the MIT License.

## Contributing
Contributions to RaQFive are welcome and encouraged! If you have ideas, bug reports, or feature requests, please submit them through the project's GitHub repository by opening an issue. Additionally, you can also contribute by improving the documentation or submitting pull requests for bug fixes and enhancements.

Please read the Contribution Guidelines for more details on how to contribute to the project.

## License

RaQFive's software is released under the MIT License. You are free to use, modify, and distribute the software in accordance with the terms of the license.
RaQFive's hardware is released under the CERN-OHL-P-2.0 Open Hardware License Permissive, Version 2.  You are free to use, modify, and distribute the hardware design in accordance with the terms of the license.
