# Arduino
## 3.1 Hardware

**(1)Raspberry Pi**

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/ea73bb4c98cc8244e128f393c5162e6.png"  width="300"height="280">
</div>

Raspberry Pi is designed for learning computer programming education, a miniature computer the size of a credit card, with its system based on Linux. With the release of IoT, users can now use Raspberry Pi running Windows. It has complete computing capabilities, capable of running operating systems similar to desktop computers. 

Raspberry Pi is commonly used in various projects, including smart home systems, media centers, gaming machines, and servers.



**(2)BeagleBoard**

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/d46d2ac3aca5a32a622f23f5d951a7f.jpg"  width="300" height="300">
</div>

BeagleBoard is a low-power open-source single-board computer jointly produced by Texas Instruments with Digi-Key and Newark. It is designed for open-source software development and serves as a demonstration of the Texas Instruments OMAP3530 system-on-a-chip. Similar to Raspberry Pi, BeagleBoard is also a low-cost, open-source hardware platform that provides a complete single-board computer solution. 

BeagleBoard is commonly used in fields such as embedded system development, robotics, medical equipment, and industrial control.


**(3)ESP32**

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/c2b1e9d0ba7c8f4f17fc7c6656a8a48.png"   width="300" height="280">
</div>

ESP32 is a series of low-cost, low-power microcontroller units that integrate Wi-Fi and dual-mode Bluetooth. The ESP32 series adopts the Tensilica Xtensa LX6 microprocessor, including dual-core and single-core versions, with built-in antenna switches, RF RF modules, power amplifiers, low-noise receive amplifiers, filters, and power management modules. Currently, the product models in the ESP32 series include ESP32 S2 (single-core + 2.4G Wi-Fi), ESP32 S3 (dual-core + 2.4G Wi-Fi + Bluetooth 5), ESP32 C2 (single-core + 2.4G Wi-Fi + Bluetooth 5), ESP32 C3 (single-core + 2.4G Wi-Fi + Bluetooth 5), and traditional ESP32 modules.

ESP32 is widely used in Internet of Things (IoT) applications and projects. They can be used as standalone microcontrollers or as wireless communication modules for other main controllers.


**(4)STM32**

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/a716b575145fff15468c29549550531.jpg"  width="250"height="220">
</div>

STM32 is a series of 32-bit ARM Cortex-M microcontrollers launched by STMicroelectronics. They provide rich peripherals and processing capabilities, suitable for projects of various scales and complexities. The STM32 series consists of multiple families, each with different subfamilies to meet the requirements of different application scenarios. They cover applications for low-power, high-performance, and various peripheral interface requirements.

STM32 is widely used in industrial control, automation, embedded systems, and the Internet of Things (IoT), among other fields.

## 3.2 Example Project

Full video presentation: 

<iframe width="560" height="500" src="https://www.youtube.com/embed/Txcl4hPJX94?si=4RheGpBv1FPVdXJF" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

Key Point:

(1) Use fewer components but get an entertaining toy;

(2) Process is intuitive and easy to understand, and even novices can try it!


<a href="https://bit.ly/3paXTLP">Click to get the code</a>

## 3.3 Water Light
The Water Light consists of a set of LEDs whose brightness changes one after another, and it is inspired by the running lights used in Japanese horse racing. 

In this project, we have the following experimental equipments: Arduino UNO, breadborad, some LEDs, some 220 ohm resistors and some wires.

**(1)Simulation Circuit**

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-10-24%20194302.png">
</div>

**(2)Hardware Connect**
In the actual hardware circuit, we only used 6 resistors and LEDs

<iframe src="//player.bilibili.com/player.html?aid=662503306&bvid=BV1Kh4y1i7xW&cid=1310962757&p=1" aspectratio="16:9" width="100%" height="600"> </iframe>

**(3)Arduino IDE Code**

```
void setup() 
{
  // 初始化引脚
  for (int i = 2; i < 8; i++) {
    pinMode(i, OUTPUT);
  }
}

void loop() 
{
  // 主循环
  for (int i = 2; i < 7; i++) {
    digitalWrite(i, HIGH);
    delay(200);
    digitalWrite(i, LOW);
    delay(200);
  }
  for (int i = 7; i > 2; i--) {
    digitalWrite(i, HIGH);
    delay(200);
    digitalWrite(i, LOW);
    delay(200);
  }
}
``` 

## 3.4 Reference 
www.arduino.cc

www.nexmaker.com/doc/5arduino