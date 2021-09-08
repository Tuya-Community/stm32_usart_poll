# stm32_usart_poll

[English](./README.md) | [中文](./README_zh.md)

## Introduction  

This Demo sends two characters received by serial port 2 in interrupt mode.

The implemented features include:

+ Polling for sending and receiving data


## Quick start  

### Compile & Burn
+ Download Tuya IoTOS Embeded Code
+ Execute the Project.uvprojx file
+ Click Compile in the software and complete the download


### File introduction 

```
├── Core
   ├── Src
       │   ├── main.c
       │   ├── gpio.c
       │   ├── usart.c
       │   ├── stm32l4xx_it.c
       │   ├── stm32l4xx_hal_msp.c
    ├── Inc
       │   ├── main.h
       │   ├── gpio.h
       │   ├── usart.h
       │   ├── stm32l4xx_it.h
       │   ├── stm32l4xx_hal_conf.h
├── Drivers
   ├── CMSIS
        ├── Device
           ├──ST
              ├──STM32L4xx
        ├── Include              
   ├── STM32L4xx_HAL_Driver
        ├── Inc
        └── Src
```



### Demo entry

Entry file：main.c

Important functions：main()

+ Initialize and configure MCU USART etc. All events are polled and judged in while(1)。



### I/O List  

| USART2  |
| :-----: |
| PA2 TXD |
| PA3 RXD |



## Related Documents

  Tuya Demo Center: https://developer.tuya.com/demo



## Technical Support

  You can get support for Tuya by using the following methods:

- Developer Center: https://developer.tuya.com
- Help Center: https://support.tuya.com/help
- Technical Support Work Order Center: [https://service.console.tuya.com](https://service.console.tuya.com/) 

