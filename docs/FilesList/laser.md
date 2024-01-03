# 6. Laser Cutting

## 6.1 Background
Laser cutting is a technology that uses a laser to cut materials, and is typically used for industrial manufacturing applications, but is also starting to be used by schools, small businesses, and hobbyists. Laser cutting works by directing the output of a high-power laser most commonly through optics. The laser optics and CNC (computer numerical control) are used to direct the material or the laser beam generated. A typical commercial laser for cutting materials uses a motion control system to follow a CNC or G-code of the pattern to be cut onto the material. The focused laser beam is directed at the material, which then either melts, burns, vaporizes away, or is blown away by a jet of gas, leaving an edge with a high-quality surface finish. Industrial laser cutters are used to cut flat-sheet material as well as structural and piping materials.

## 6.2 Materials of Laser Cutting
### (1) Metallic materials
**Steel**: Laser cutters can cut stainless steel. The laser cutting machine precisely cuts the stainless steel sheet through a high-power laser beam, which can guarantee the minimum heat input during the cutting process, so as to maintain the good corrosion resistance of the stainless steel.

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/steel.png" style="width:75%;">
  </div>

**Aluminum**: Laser cutting machines can cut aluminum and alloys. Aluminum and alloys are commonly used metal materials that can be cut by laser cutting machines. The laser cutting machine is able to blow away the molten material in the cutting area by means of an auxiliary gas, so as to obtain a better cut quality. However, it is necessary to pay attention to avoid the formation of intergranular microcracks on the surface of the slit, so choose the appropriate gas as the auxiliary vapor to ensure the quality of laser cutting. At the same time, it is also necessary to pay attention to avoid the conversion of the laser cutting machine into an air oxide layer during trimming, so as not to continue to cause coarse crystals..

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/alu.png" style="width:75%;">
  </div>

## (2) Non-metallic materials
**Acrylic**: also known as plexiglass, plexiglass, PMMA

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/acrylic.png" style="width:75%;">
  </div>

**Wood**: Various types of wood, including plywood and MDF, can be laser cut, but some oily woods carry the risk of ignition and should be used with special care.

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/wood.png" style="width:75%;">
  </div>

**Paper**: Cardboard can be laser cut because cardboard is thinner and more fragile, using laser cutting can avoid thermal damage to the cardboard and can maintain the aesthetics and flatness of the cardboard. 


<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/paper.png" style="width:75%;">
  </div>

**Glass**: Laser cutters can cut glass because of its fragile and reflective properties, which can guarantee a good finish on the edges. Due to its fragile and reflective properties, the quality of the cut can be guaranteed by using a laser cutting machine. However, it is necessary to pay attention to the fact that the glass is not easy to cut, and the cutting speed should be controlled to avoid the formation of cracks.

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/glasscutting.png" style="width:75%;">
  </div>



## 6.3 Kerf Experiment

Apparently, the laser also has diameter. We could test the kerf(the diameter of laser) by using 5 rectanges to measure it.

>(1) The width of each rectange in the Powercut is 10mm.

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/power.jpg" style="width:75%;">
  </div>

>(2) Next step, we find a 3mm acrylic plate for cutting:

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/cutting.jpg" style="width:75%;">
  </div>

>(3) Final step, we use the vernier caliper to measure the outside length of 5 rectangles:

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/measure.jpg" style="width:75%;">
  </div>

After the procedure, we measured the outside length of 5 rectangles is 51.34mm,so the kerf is

__kerf= (51.34-50)/10=0.134mm__

## 6.4 Laser Cutting Project

>(1) Drawing design: AI is used to make a rotating arm assembly, and the aperture is designed according to the servo hole. Mode selection laser cutting
assemble laser cutter part.

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/drawdesign.jpg" style="width:75%;">
  </div>

>(2) Turn on the laser cutting machine, confirm the safe operation status of the machine, and perform operations such as resetting, positioning, and cutting the frame.

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/preparelaser.jpg" style="width:75%;">
  </div>

>(3) Parameter adjustment: the parameter of laser cutting is speed 10mm/s, the maximum power is 100%, the minimum power is 90%, and the parameter of laser scanning is speed 500mm/s

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/paras.jpg" style="width:75%;">
  </div>

>(4) Make a cut, and one part of laser cutting is completed.

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/carrot.jpg" style="width:75%;">
  </div>

## 6.4 Assemble with Arduino

<iframe width="100%" height="650" 
src="//player.bilibili.com/player.html?aid=965745190&bvid=BV1JW4y1P7Ha&cid=1392645038&p=1" 
scrolling="no" border="0" frameborder="0" allowfullscreen>
</iframe>

## 6.5 Assemble laser cutter parts together

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/workonlaser.jpg" style="width:75%;">
  </div>

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/laserparts.jpg" style="width:75%;">
  </div>

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/laserconnect.jpg" style="width:75%;">
  </div>

**final video：**

<iframe width="100%" height="650" 
src="//player.bilibili.com/player.html?aid=453167656&bvid=BV1j5411z7Gy&cid=1392705846&p=1" 
scrolling="no" border="0" frameborder="0" allowfullscreen>
</iframe>
