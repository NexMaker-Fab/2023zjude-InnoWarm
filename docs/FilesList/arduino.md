# Arduino
## 3.1 Hardware

**(1)Raspberry Pi**

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/ea73bb4c98cc8244e128f393c5162e6.png"  width="300"height="280">
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
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/a716b575145fff15468c29549550531.jpg"  width="250"height="220">
</div>

STM32 is a series of 32-bit ARM Cortex-M microcontrollers launched by STMicroelectronics. They provide rich peripherals and processing capabilities, suitable for projects of various scales and complexities. The STM32 series consists of multiple families, each with different subfamilies to meet the requirements of different application scenarios. They cover applications for low-power, high-performance, and various peripheral interface requirements.

STM32 is widely used in industrial control, automation, embedded systems, and the Internet of Things (IoT), among other fields.

## 3.2 A Brief Introduction to Arduino IDE
### 3.2.1 Layout of Arduino IDE

<div class="center">
    <img src="https://github.com/Mia1210-my/MY/raw/main/img/IDE%20layput.jpg"  height="280">
</div>

The interface of the Arduino IDE is roughly divided into four sections:

① **Menu bar**. Includes File menu, Edit menu, Program menu, Tools menu and Help menu.

② **Toolbar**. Contains compile, upload, new programme (sketch), open programme (sketch), save programme (sketch) and serial monitor (Serial Monitor).

③ **Editing area**. The area for writing programme code.

④ **Status area**. Displays information such as compilation and uploading of the programme, and if the programme has errors, there will be an error message.

The Arduino IDE toolbar has some commonly used tools:

<div class="center">
    <img src="https://github.com/Mia1210-my/MY/raw/main/img/IDE%20tool%20bar.jpg"  height="50">
</div>

**Verify:** This button is used to check the correctness of your "syntax" or code. If your code has any syntax errors or undefined variables, an error message will appear at the bottom of the IDE screen. At the same time, the wrong line of code will be marked with a red background colour to make it easier to modify. However, if it is correct, you will see a message that the compilation is complete.

**Upload:** It allows us to upload programs to the Arduino. 

**Debug:** It basically goes through a program in a controlled manner, with the help of a hardware interface which can help navigate through the program's execution. This can be of aid in better understanding the program as well as helping spot potential flaws and code errors.

**Serial Plotter:** It provides a way through which we can graph the data printed in real time to the Arduino's serial port.

**Serial Monitor:** It receives data sent from the Arduino to the computer and is often used for debugging code.

### 3.2.2 Configure Arduino IDE

(1) Serial Port Configuration: Before we load the sample project to test the Arduino, we need to configure the IDE to use the Arduino connected to the computer by clicking "Tools -> Port" and then find the COM port of the Arduino.

<div class="center">
    <img src="https://github.com/Mia1210-my/MY/raw/main/img/IDE%20port.jpg"  height="280">
</div>

(2) Development board configuration:
Click Tools -> Board -> select the Arduino board model (Tools -> Board) e.g. Arduino Uno, you only need to configure it once here, and it will be used by default in all subsequent operations.

<div class="center">
    <img src="https://github.com/Mia1210-my/MY/raw/main/img/IDE%20board.jpg"  height="280">
</div>

(3) Selecting or writing a programme: In Arduino IDE, in order to facilitate the developer to learn, IDE internal integration of many Arduino routines, you can choose a trial run or write their own programs.

<div class="center">
    <img src="https://github.com/Mia1210-my/MY/raw/main/img/IDE%20programme.jpg"  height="280">
</div>

### 3.2.3 Compile and Upload

First, click the "Verify" icon to confirm whether the programme can be compiled.

<div class="center">
    <img src="https://github.com/Mia1210-my/MY/raw/main/img/IDE%20verify.jpg"  height="280">
</div>

Then click on the upload icon to download the code to the Arduino.

<div class="center">
    <img src="https://github.com/Mia1210-my/MY/raw/main/img/IDE%20upload.jpg"  height="100">
</div>

Finally, the programme can be seen actually running on the development board.


## 3.3 Example Project

Full video presentation: 

<iframe width="560" height="500" src="https://www.youtube.com/embed/Txcl4hPJX94?si=4RheGpBv1FPVdXJF" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

Key Point:

(1) Use fewer components but get an entertaining toy;

(2) Process is intuitive and easy to understand, and even novices can try it!


<a href="https://bit.ly/3paXTLP">Click to get the code</a>


## 3.4 Water Light

The Water Light consists of a set of LEDs whose brightness changes one after another, and it is inspired by the running lights used in Japanese horse racing. 

In this project, we have the following experimental equipments: Arduino UNO, breadborad, some LEDs, some 220 ohm resistors and some wires.

**(1)Simulation Circuit**

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-10-24%20194302.png"  height="280">
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


## 3.5 Arduino output

In this section, we begin by using the a LCD display and arduino to display a simple 'helloword' statement. The hardware connections and final results are as follows.

<iframe src="//player.bilibili.com/player.html?aid=620481802&bvid=BV1W84y197WL&cid=1320258345&p=1" aspectratio="16:9" width="100%" height="600"> </iframe>

Then we tried a more interesting and challenging task: making the Snake game. 

**(1)Simulation Circuit**

<div class="center">
    <img src="https://github.com/Mia1210-my/MY/raw/main/img/thinkercad1.jpg"  height="280">
</div>

**(2)Hardware Connect**

In the actual hardware circuit, we used an LCD display, a joystick and Arduino. The final presentation is as follows.

<iframe src="//player.bilibili.com/player.html?aid=407902575&bvid=BV1xG411X7Kb&cid=1320260598&p=1" aspectratio="16:9" width="100%" height="600"> </iframe>

**(3)Arduino IDE Code**
```
#include <LiquidCrystal.h>

LiquidCrystal lcd(12, 11, 5, 4, 3, 2);

// 定义LCD屏幕的尺寸
const int LCD_COLUMNS = 16;
const int LCD_ROWS = 2;

// 贪吃蛇变量
int snakeX = LCD_COLUMNS / 2;
int snakeY = LCD_ROWS / 2;
int foodX;
int foodY;
int snakeLength = 1;
int snakeDirectionX = 0;
int snakeDirectionY = 0;

// 按钮和摇杆引脚
const int BUTTON_XY_PIN = 8;
const int JOYSTICK_X_PIN = A0;
const int JOYSTICK_Y_PIN = A1;

// 按钮和摇杆状态变量
int buttonXYState = HIGH;
int lastButtonXYState = HIGH;
int joystickXValue = 0;
int joystickYValue = 0;

// 游戏状态变量
bool gameOver = false;

void setup() {
  lcd.begin(LCD_COLUMNS, LCD_ROWS);
  randomSeed(analogRead(0)); // 种子随机数生成器

  // 初始化按钮和摇杆引脚
  pinMode(BUTTON_XY_PIN, INPUT_PULLUP);

  // 打印初始消息
  lcd.print("贪吃蛇游戏");
  lcd.setCursor(0, 1);
  lcd.print("按下任意按钮");
}

void generateFood() {
  foodX = random(0, LCD_COLUMNS);
  foodY = random(0, LCD_ROWS);
}

void updateSnake() {
  snakeX += snakeDirectionX;
  snakeY += snakeDirectionY;

  // 检查贪吃蛇是否碰到屏幕边缘
  if (snakeX < 0 || snakeX >= LCD_COLUMNS || snakeY < 0 || snakeY >= LCD_ROWS) {
    gameOver = true;
    return;
  }

  // 检查贪吃蛇是否与食物碰撞
  if (snakeX == foodX && snakeY == foodY) {
    snakeLength++;
    generateFood();
  }
}

void drawSnake() {
  lcd.clear();
  lcd.setCursor(snakeX, snakeY);
  lcd.print("#");

  // 打印食物
  lcd.setCursor(foodX, foodY);
  lcd.print("*");
}

void handleInput() {
  buttonXYState = digitalRead(BUTTON_XY_PIN);

  if (buttonXYState != lastButtonXYState) {
    if (buttonXYState == LOW) {
      gameOver = true; // 当按下XY按钮时重新开始游戏
    }
    lastButtonXYState = buttonXYState;
  }

  joystickXValue = analogRead(JOYSTICK_X_PIN);
  joystickYValue = analogRead(JOYSTICK_Y_PIN);

  // 根据摇杆的X和Y值调整贪吃蛇的移动方向
  if (joystickXValue < 400) {
    snakeDirectionX = -1; // 向左移动
  } else if (joystickXValue > 600) {
    snakeDirectionX = 1; // 向右移动
  } else {
    snakeDirectionX = 0; // 停止水平移动
  }

  if (joystickYValue < 400) {
    snakeDirectionY = -1; // 向上移动
  } else if (joystickYValue > 600) {
    snakeDirectionY = 1; // 向下移动
  } else {
    snakeDirectionY = 0; // 停止垂直移动
  }
}

void loop() {
  if (gameOver) {
    lcd.clear();
    lcd.print("game over");
    return;
  }

  handleInput();
  updateSnake();
  drawSnake();

  delay(200);
}
```

## 3.6 Arduino intput

In this section, we first try a simple distance measurement using an ultrasonic sensor and display the distance in the serial monitor panel of the Arduino IDE. During this process we encountered problems with inaccurate display. After checking this, we found that it was because the values in the code did not correspond to the serial communication in the IDE, and then we fixed the problem.

Then we used an ultrasonic sensor to measure the distance and displayed the distance measurement on the LCD display. The process and results are shown below.

**(1)Simulation Circuit**

<div class="center">
    <img src="https://github.com/Mia1210-my/MY/raw/main/img/sensor.png"  height="280">
</div>

**(2)Hardware Connect**

In the actual hardware circuit, we only used a LCDdisplay and an ultrasonic sensor.

<iframe src="//player.bilibili.com/player.html?aid=450592435&bvid=BV16j411Y7G9&cid=1323637327&p=1" aspectratio="16:9" width="100%" height="600"> </iframe>

**(3)Arduino IDE Code**

```
#include <LiquidCrystal.h>

#define LM35 A0
#define Trig 8 //引脚Tring 连接 IO D8
#define Echo 9 //引脚Echo 连接 IO D9
 
float cm; //距离变量

LiquidCrystal lcd(12,11,5,4,3,2);      //构造一个LiquidCrystal的类成员。使用数字IO ，12,11,5,4,3,2

int val = 0;        //存放AD变量值
float temp = 0;     //存放温度值的10倍

void setup()
{
  lcd.begin(16,2);    //初始化LCD1602
  lcd.print("Welcome to use!");   //液晶显示Welcome to use！
  delay(1000);        //延时1000ms
  lcd.clear();        //液晶清屏
  
  pinMode(Trig, OUTPUT);
  pinMode(Echo, INPUT);
}

void loop()
{
  //给Trig发送一个低高低的短时间脉冲,触发测距
  digitalWrite(Trig, LOW); //给Trig发送一个低电平
  delayMicroseconds(2);    //等待 2微妙
  digitalWrite(Trig,HIGH); //给Trig发送一个高电平
  delayMicroseconds(10);    //等待 10微妙
  digitalWrite(Trig, LOW); //给Trig发送一个低电平
  
  temp = float(pulseIn(Echo, HIGH)); //存储回波等待时间,
  //pulseIn函数会等待引脚变为HIGH,开始计算时间,再等待变为LOW并停止计时
  //返回脉冲的长度
  
  //声速是:340m/1s 换算成 34000cm / 1000000μs => 34 / 1000
  //因为发送到接收,实际是相同距离走了2回,所以要除以2
  //距离(厘米)  =  (回波时间 * (34 / 1000)) / 2
  //简化后的计算公式为 (回波时间 * 17)/ 1000
  cm = (temp * 17 )/1000; //把回波时间换算成cm
  
  lcd.setCursor(0,0);       //设置液晶开始显示的指针位置
  lcd.print("Now Distance："); //液晶显示“LM35 temp =”
  lcd.setCursor(0,1);       //设置液晶开始显示的指针位置，在下一行显示
  lcd.print(cm);  //液晶显示距离
  
  
  delay(1000);              //延时1000ms
}
```


## 3.7 Cases similar to the final project

**Reference case III: LED integration**

This project uses Arduino board, RGB matrix, matrix power supply and so on to realise the change of pattern.

Advantages: the project is a combination of hardware and software, which is easier to reproduce and refer to.

Limitations: the project is complicated to operate, and the face rendering effect is poor.

<div class="center">
    <img src="https://github.com/Mia1210-my/MY/raw/main/img/project3.png"  height="250">
</div>


## 3.8 Reference 
www.arduino.cc


www.nexmaker.com/doc/5arduino


https://blog.csdn.net/weixin_44996090/article/details/105922780


https://blog.csdn.net/as480133937/article/details/105331315/
