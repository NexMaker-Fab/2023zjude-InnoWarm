# 4. Interface application programming
## 4.1  introduction

Processing is a free graphical library and integrated development environment (IDE) built for the electronic arts, new media art, and visual design communities with the purpose of teaching non-programmers the fundamentals of computer programming in a visual context.

Processing uses the Java language, with additional simplifications such as additional classes and aliased mathematical functions and operations. It also provides a graphical user interface for simplifying the compilation and execution stage.

The Processing language and IDE have been the precursor to other projects including Arduino and Wiring.

**(1)p5.js**

<div class="center">
    <img src="https://github.com/aooazja/2023zjude-zja/raw/main/IMG/p5js.jpg"  width="300"height="280">
</div>

This is a JavaScript-based creative programming library focused on art and visualization. Its syntax is very similar to Processing, but it is web-based and can be used to create interactive web works.



**(2)OpenFrameworks**

<div class="center">
    <img src="https://github.com/aooazja/2023zjude-zja/raw/main/IMG/of.png"  width="300" height="300">
</div>

This is a C++ creative programming toolkit for visual arts, graphics and audio processing. It provides a rich library that allows users to explore and create a variety of creative projects.


**(3)Cinder**

<div class="center">
    <img src="https://github.com/aooazja/2023zjude-zja/raw/main/IMG/cinder.png"   width="300" height="140">
</div>

Similar to OpenFrameworks, Cinder is a creative programming library for C++ that specializes in graphics and audio applications. It provides a range of tools and features for developing creative art projects.

**(4)vvvv**

<div class="center">
    <img src="https://github.com/aooazja/2023zjude-zja/raw/main/IMG/vvvv.jpg"  width="250"height="220">
</div>

This is a visual programming tool for creative programming and visual design. It uses a graphical interface to create and edit nodes, allowing users to build complex art projects by connecting nodes.
## 4.2 Demo(use mouse or keyboard to interactive)

**(1)Processing code**

```
ArrayList<Particle> particles;

void setup() {
  size(800, 600);
  particles = new ArrayList<Particle>();
}

void draw() {
  background(255);
  
  if (mousePressed) {
    float mY = map(mouseY, 0, height, 1, -1);
    PVector force = new PVector(random(-0.05, 0.05), mY);
    particles.add(new Particle(mouseX, mouseY, force));
  }
  
  for (int i = particles.size()-1; i >= 0; i--) {
    Particle p = particles.get(i);
    p.update();
    p.display();
    if (p.isDead()) {
      particles.remove(i);
    }
  }
}

class Particle {
  PVector acceleration;
  PVector velocity;
  PVector position;
  float lifespan;
  float radius;
  color col;
  
  Particle(float x, float y, PVector force) {
    acceleration = new PVector(0, 1);
    velocity = new PVector(random(-1, 1), random(-1, 1));
    lifespan = 255;
    position = new PVector(x, y);
    radius = random(10, 50);
    col = color(255, random(200), 0);
    velocity.add(force);
  }
  
  void applyForce() {
    acceleration.add(velocity);
  }
  
  void update() {
    velocity.add(acceleration);
    position.add(velocity);
    lifespan -= 5.0;
    acceleration = new PVector(0, 0);
    col = color(red(col), green(col), blue(col), (int)lifespan);
    radius -= 1;
  }
  
  void display() {
    noStroke();
    fill(col);
    ellipse(position.x, position.y, radius, radius);
  }
  
  boolean isDead() {
    return lifespan < 0.0;
  }
}
```

**(2)Demonstration**

When the mouse is clicked, traces appear on the screen to generate interactions：

<iframe width="560" height="500" src="//player.bilibili.com/player.html?aid=964094838&bvid=BV1hH4y1176L&cid=1350323084&p=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>

## 4.3 Demo in processing and arduino

**(1)Processing code**

```
import processing.serial.*;
Serial port;

int diam = 50;

void setup(){
  size(500,500);
  background(#ffffff);
  
  fill(#f3a694);
  noStroke();
  ellipse(200 , 200 , diam , diam);
  
  String portName = Serial.list()[1];
  port = new Serial(this, portName ,9600);
  println(portName);
}

void draw() {
  
  while(port.available()>0)
  {
    diam = port.readChar();
    //println(diam);
    clear();
    background(#ffffff);
    ellipse(200, 200, diam, diam);
  }
  
  
  
  //println(777);
  
  //delay(100);
  
}
```

**(2)arduino**

arduino connection

<div class="center">
    <img src="https://github.com/aooazja/2023zjude-zja/raw/main/IMG/WechatIMG14.jpg"  width="300" height="280">
</div>

arduino code

```
int size = 0;

void setup() {
  
  Serial.begin(9600);


}

void loop() {
  
  size = map(analogRead(A0), 0, 1023, 5, 190);

  Serial.write(size);

//  delay(10)
}
```

**(3)Demonstration**

<iframe width="560" height="500" src="//player.bilibili.com/player.html?aid=877935782&bvid=BV1zN4y1q7UU&cid=1384859693&p=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>

<iframe width="560" height="500" src="//player.bilibili.com/player.html?aid=283228357&bvid=BV1dc411b7Rn&cid=1391705018&p=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>

## 4.4 New Tool:Kineck
Microsoft Kinect is the next generation of Computing. Kinect is a motion sensing input device by Microsoft for the Xbox 360 video game console and Windows PCs. Based around a webcam-style add-on peripheral for the Xbox 360 console, it enables users to control and interact with the Xbox 360 without the need to touch a game controller, through a natural user interface using gestures and spoken commands. [The project is aimed at broadening the Xbox 360's audience beyond its typical gamer base. Kinect competes with the Wii Remote Plus and PlayStation. Move with PlayStation Eye motion controllers for the Wii and PlayStation 3 home consoles, respectively. The Kinect for Windows sensor is a fully-tested and supported Kinect experience on Windows with features such as “near mode,” skeletal tracking control, API improvements, and improved USB support across a range of Windows computers and Windows-specific 10’ acoustic models. The sensor was specifically designed to be used with computers, and includes a shortened USB cable to ensure reliability across a broad range of computers. Kinect for Xbox 360 was built for and tested with the Xbox 360 only, not with any other platform, which is why it is not licensed for general commercial use, supported, or under warranty when used on any other platform. Kinect for Xbox 360, on the other hand, was built for and tested with the Xbox 360 only, not with any other platform, which is why it is not licensed for general commercial use, supported, or under warranty when used on any other platform. Microsoft has a large team of engineers that is dedicated to continual improvements of the hardware and software associated with Kinect for Windows, and is committed to providing ongoing access to Microsoft's deep investment in human tracking and speech recognition. But both can be used for development.

**Core Technologies:**
- Depth Sensing: Kinect incorporates a depth camera that generates a depth map, enabling precise measurement of distances between objects.
- RGB Camera: In addition to the depth camera, it includes a regular RGB camera for capturing color images.
- Microphone Array: An integrated array of microphones is used for sound recognition and localization.

**Applications:**
- Gaming: Initially designed for Xbox games, Kinect revolutionized gaming by allowing users to control games through body movements and voice commands.
- Virtual Reality (VR) and Augmented Reality (AR): Kinect finds extensive use in VR and AR applications, enhancing immersive experiences by capturing user movements and the environment.
- Art and Creative Programming: Artists and developers leverage Kinect for various creative projects, including interactive art installations and real-time animations.

**Development Support:**
- Kinect provides a set of development tools and an SDK (Software Development Kit), empowering developers to access depth maps, color images, and audio data for diverse applications.

**Evolution of Kinect:**
- Subsequent versions, such as Kinect for Windows v2, offer enhanced depth sensing and features specifically tailored for the Windows platform.
- Microsoft introduced the Azure Kinect DK, expanding Kinect's capabilities beyond gaming to support a broader range of computer vision and deep learning applications.

Kinect stands as a remarkable technology with applications spanning gaming, virtual interaction, and creative programming. Its depth sensing capabilities and full-body motion capture make it a powerful tool for various innovative endeavors.

## Reference

https://en.wikipedia.org/wiki/Processing

https://www.bilibili.com/video/BV1MC4y1s7gm/?spm_id_from=333.999.0.0&vd_source=2401c15cc3a81cfb2753e3ea23639e6a

https://openprocessing.org/

https://learn.microsoft.com/zh-cn/windows/apps/design/devices/kinect-for-windows
