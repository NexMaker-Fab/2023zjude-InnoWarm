# Processing
## 3.1  introduction

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
## 3.2 Demo(use mouse or keyboard to interactive)

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

## 3.3 Demo in processing and arduino

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
    <img src="https://github.com/aooazja/2023zjude-zja/raw/main/IMG/of.png"  width="300" height="300">
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

## 3.4 New Tool

## Reference

https://en.wikipedia.org/wiki/Processing

https://www.bilibili.com/video/BV1MC4y1s7gm/?spm_id_from=333.999.0.0&vd_source=2401c15cc3a81cfb2753e3ea23639e6a

https://openprocessing.org/
