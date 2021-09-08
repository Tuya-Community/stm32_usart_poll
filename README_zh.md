# stm32_usart_poll

[English](./README.md) | [中文](./README_zh.md)

## 简介 

本Demo通过轮询方式把串口2接收到的2个字符发送出去。

已实现功能包括：

+ 轮询收发数据

  

## 快速上手 

### 编译与烧录
+ 下载Tuya IoTOS嵌入式代码

+ 执行Project.uvprojx文件

+ 点击软件中的编译，并完成下载


### 文件介绍 

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



### Demo入口

入口文件：main.c

重要函数：main()

+ 对mcu的USART等进行初始化配置，所有事件在while(1)中轮询判断。



### I/O 列表 

| USART2  |
| :-----: |
| PA2 TXD |
| PA3 RXD |

## 相关文档

涂鸦Demo中心：https://developer.tuya.com/demo



## 技术支持

您可以通过以下方法获得涂鸦的支持:

- 开发者中心：https://developer.tuya.com
- 帮助中心: https://support.tuya.com/help
- 技术支持工单中心: [https://service.console.tuya.com](https://service.console.tuya.com/) 

