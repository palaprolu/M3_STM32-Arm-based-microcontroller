# Wiper System Of The Car :-


This firmware is a hacky mishmash of VW and Nissan CAN code. It talks to the Nissan BMS (aka LBC) to find out cell voltages and such. It also produces all messages needed for satisfying the various controllers in newer VW cars (my testbed is a 2004 Touran). That means all warning lights are off. It also implements the ChaDeMo protocol and has been successfully tested on various fast chargers.

## Features :-
* Send all messages necessary to make the DSC light go off
* Do simple traction control by comparing rear and front axle speeds
* Fake the oil pressure sensor depending on motor rpm
* Map the electric motor speed onto the speed dial
* Map the electric motor temperature onto the temp dial
* Map the momentary electric power onto the fuel economy display
* Read key switch, brake switch and cruise control buttons from CAN bus
* Read brake vacuum sensor and control vacuum pump
* Read throttle pedal and put it on the CAN bus
* Including support for dual channel throttles
* Read individual cell voltages from Nissan Leaf BMS (LBC)
* Read SoC, SoH etc. from LBC
* Read power limits from LBC and use them for inverter power limit and charge current control
* Implement ChaDeMo protocol with values obtained from LBC
* Control analog fuel gauge via two current source channels

## IO Pins :-


* Throttle1 (pot) - PC1
* Throttle2 (pot2) - PC0
* Vacuum sensor - PC2
* 12V level - PA3
* Digital start input - PB6
* Digital brake input - PA2
* DC switch output - PC13
* Precharge output - PC11
* Vacuum pump output - PB1
* Oil sensor simulation - PC5
* Fuel sensor simulation - PB7, PB8 (positive, negative)






[![CI](https://github.com/palaprolu/M3_STM32-Arm-based-microcontroller/actions/workflows/CI%20main.yml/badge.svg)](https://github.com/palaprolu/M3_STM32-Arm-based-microcontroller/actions/workflows/CI%20main.yml)

[![BUILD WINDOWS](https://github.com/palaprolu/M3_STM32-Arm-based-microcontroller/actions/workflows/BUILD%20WINDOWS%20main.yml/badge.svg?branch=main)](https://github.com/palaprolu/M3_STM32-Arm-based-microcontroller/actions/workflows/BUILD%20WINDOWS%20main.yml) 


[![BULD LINUX](https://github.com/palaprolu/M3_STM32-Arm-based-microcontroller/actions/workflows/BUILD%20LINUX%20main.yml/badge.svg)](https://github.com/palaprolu/M3_STM32-Arm-based-microcontroller/actions/workflows/BUILD%20LINUX%20main.yml)


[![GIT INSPECTOR](https://github.com/palaprolu/M3_STM32-Arm-based-microcontroller/actions/workflows/GIT%20INSPECTOR%20main.yml/badge.svg)](https://github.com/palaprolu/M3_STM32-Arm-based-microcontroller/actions/workflows/GIT%20INSPECTOR%20main.yml)


[![CPP CHECK](https://github.com/palaprolu/M3_STM32-Arm-based-microcontroller/actions/workflows/CPP%20CHECK%20main.yml/badge.svg)](https://github.com/palaprolu/M3_STM32-Arm-based-microcontroller/actions/workflows/CPP%20CHECK%20main.yml)


[![DYNAMIC CHECK](https://github.com/palaprolu/M3_STM32-Arm-based-microcontroller/actions/workflows/DYNAMIC%20CHECKmain.yml/badge.svg)](https://github.com/palaprolu/M3_STM32-Arm-based-microcontroller/actions/workflows/DYNAMIC%20CHECKmain.yml)


[![STATIC CODE](https://github.com/palaprolu/M3_STM32-Arm-based-microcontroller/actions/workflows/STATIC%20CODE%20main.yml/badge.svg?branch=main)](https://github.com/palaprolu/M3_STM32-Arm-based-microcontroller/actions/workflows/STATIC%20CODE%20main.yml)


[![VALGRIND](https://github.com/palaprolu/M3_STM32-Arm-based-microcontroller/actions/workflows/VALGRIND%20main.yml/badge.svg)](https://github.com/palaprolu/M3_STM32-Arm-based-microcontroller/actions/workflows/VALGRIND%20main.yml)


[![UNIT TESTING](https://github.com/palaprolu/M3_STM32-Arm-based-microcontroller/actions/workflows/UNIT%20TESTING%20main.yml/badge.svg)](https://github.com/palaprolu/M3_STM32-Arm-based-microcontroller/actions/workflows/UNIT%20TESTING%20main.yml)
