# 2.Fusion

Fusion 360 is a comprehensive design software developed by Autodesk, originally known as "Inventor Fusion" when it was first introduced in 2009. It provides a powerful set of tools and features for 3D modeling, CAD (Computer-Aided Design), CAM (Computer-Aided Manufacturing), CAE (Computer-Aided Engineering), as well as collaboration and data management.
The design philosophy of Fusion 360 is to integrate design, engineering, and manufacturing into a unified platform, offering users a holistic design and manufacturing solution. It features an intuitive user interface, cloud storage, and collaboration capabilities, assisting designers, engineers, and manufacturers in creative design, product development, and optimization of manufacturing processes.

With Fusion 360, users can perform parametric modeling, assembly design, surface modeling, rendering, animation, and more. It also provides powerful simulation and analysis tools to validate design performance and behavior. Additionally, Fusion 360 supports integration with other design software, enabling collaboration and data exchange with professionals from different fields.

In summary, Fusion 360 is a powerful design software aimed at providing users with a comprehensive design, engineering, and manufacturing solution. Its design philosophy revolves around integrating various stages of the design and manufacturing process, offering an intuitive interface, and facilitating cloud-based collaboration. Through Fusion 360, users can achieve creative design, product development, and optimization of manufacturing processes.。

## 2.1 Part Modeling
(1) Create a new group folder within zju2023, enter the sketch, and draw a central rectangle with dimensions of 200mm for both length and width. (Sketches all need constraints)
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/1.png"  style="width:70%;">
</div>
(2) After completing the central rectangle in the top view, round the corners four times to obtain a rounded rectangle with a corner radius of 40mm.
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/2.png"  style="width:70%;">
</div>
(3) In the sketch, draw a circle in preparation for a sweep.
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/3.png" style="width:70%;">
</div>
(4) Perform a sweep operation using the drawn rounded rectangle and circle.
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/4.png"  style="width:70%;">
</div>
(5) Create a part from the solid entities (subsequent parts should also be created or set as parts from the beginning), and then create a sketch for a cylindrical pipe.
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/5.png" style="width:70%;">
</div>
(6) Create an array of four identical parts in a circular pattern, and then complete the drawing of a circle and a vertical line.
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/hxzl.png"  style="width:70%;">
</div>
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/6.png"  style="width:70%;">
</div>
(7) Move and copy the circle, then use the sweep method to create a torus (ring-shaped object).
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/7.png"  style="width:70%;">
</div>
(8) Move and copy the torus to create another one, then draw the contour lines.
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/8.png"  style="width:70%;">
</div>
(9) After extruding, cut off a portion of the torus.
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/9.png"  style="width:70%;">
</div>
(10) Use the circle, line, and trim commands to draw a circular track, then extrude it to create a part.
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/10.png"  style="width:70%;">
</div>
(11) Draw two circles for the purpose of performing a cut.
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/11.png"  style="width:70%;">
</div>
(12) After extruding and performing the cut operation, the resulting image is obtained. Similarly, after generating a rectangle in the sketch and performing the cut operation, the resulting image is obtained.
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/12.png"  style="width:70%;">
</div>
(13) The circular array produces the image shown below.
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/13.png"  style="width:70%;">
</div>
(14) Draw a cylinder, then create another cylinder and merge them together.
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/14.png"  style="width:70%;">
</div>
(15) After sketching, extrude the geometry.
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/14-1.png"  style="width:70%;">
</div>
(16) Obtain the image shown below by applying fillets and adding cylinders.
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/15.png"  style="width:70%;">
</div>
(17) Obtain the image shown below by extruding the sketch, and create a cylindrical subtractive component.
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/16.png"  style="width:70%;">
</div>
(18) Draw a cylinder and a cylindrical pipe, which can be combined to form an expandable structure.
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/17.png"  style="width:70%;">
</div>
(19) Artificial Intelligence Component Generation (Generated results were unsatisfactory and ultimately not adopted).
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/18.png"  style="width:70%;">
</div>
(20) Add details.
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/19.png"  style="width:70%;">
</div>
(21) The corners are rounded and the material is selected for easy observation.
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20.png"  style="width:70%;">
</div>
(22) Add details through chamfers to complete the model.
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/yuanjiao.png"  style="width:70%;">
</div>



## 2.3 Part models and Drawings
（1）Model 1
<iframe style="width:70%;" height=500 src="https://a360.co/48R9Go6" ></frame>

（2）Model 2
<iframe style="width:70%;" height=500 src="https://a360.co/3THz6zy" ></frame>
Engineering drawings of model 2
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/gct.png"  style="width:70%;">
</div>





## 2.4 Simulation Video

Motion simulation model building process video:

<iframe style="width:70%;" height=500 src="//player.bilibili.com/player.html?aid=832564395&bvid=BV1834y1u7Hv&cid=1311044014&p=1"  frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


## 2.5 Plugin Installation and Usage

**Plugin Installment**

(1) Click on the <a href="https://www.autodesk.com/fusionappstore/">Fusion 360 APP store</a> in the Add-ons section of the utility and search for the desired plug-in, such as gear
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/a1.png"  style="width:70%;">
</div>
(2) Select the appropriate plug-in to download (login account required)
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/a2.png"  style="width:70%;">
</div>
(3) Double-click to run the installation package
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/a3.png"  style="width:70%;">
</div>
(4) Once the installation is complete, the installed plugin is available in the Scripts and Add-ons module
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/a4.png"  style="width:70%;">
</div>
(5) An icon appears on the page, click Run to create the gears as required.
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/a5.png"  style="width:70%;">
</div>


**Fusion 360 add-on module modeling video:**

<iframe style="width:70%;" height=500 src="//player.bilibili.com/player.html?aid=280081570&bvid=BV1Uc411o72A&cid=1311464501&p=1"  frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

## 2.6 Automated Modeling Examples
AI automated modeling process video:

<iframe style="width:70%;" height=500 src="////player.bilibili.com/player.html?aid=962553267&bvid=BV11H4y197KG&cid=1311074464&p=1"  frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

## 2.7 Other Software
(1) <a href="https://www.zwcad.com/">ZWSOFT CAD</a>

ZWSOFT（中望） CAD is a professional engineering modeling software independently developed in China, widely used in fields such as architecture, mechanical engineering, and power industry. It is based on an independent kernel and is a 2D CAD platform that is fully compatible with the DWG format. It extensively supports mainstream industry applications and customized development of user-specific functions. Since its launch in 2002, ZWSOFT CAD has helped users in various industries such as architecture, surveying, urban planning, mechanical manufacturing, electronics, and power achieve efficient design and domestic innovation.

ZWSOFT CAD provides powerful modeling, analysis, and design functions, assisting engineers in precise 3D modeling and simulation analysis. It features efficient algorithm optimization and high versatility, including batch printing, sheet sets, dynamic blocks, PDF import, and lasso selection. The software operates at high speed, offers comprehensive functionality, and has a high level of intelligence, enabling designers to rapidly complete complex design tasks.
<div class="center">
    <img src="https://raw.githubusercontent.com/ingw3216/blogimage/main/img/CAD6.png" style="width:70%;">
</div>

**a.Main Features**
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/CAD7.png" style="width:70%;">
</div>

**b.Functionality**
<div class="center">
    <img src="https://raw.githubusercontent.com/ingw3216/blogimage/main/img/CAD2.jpg" style="width:70%;">
</div>


(2) <a href="https://www.yaocsoft.com/index.html">Yaochuang CAD</a>

Yaochuang(尧创) CAD is a professional drawing software with complete independent intellectual property rights. It is fully compatible with AutoCAD, offering powerful functionality and cost-effectiveness, and has been widely used in industries such as mechanical engineering, electronics, chemical engineering, architecture, shipbuilding, and aviation.

Yaochuang Mechanical CAD is a CAD product specifically developed to meet the drawing needs of the mechanical and complete equipment manufacturing industry. It not only includes the powerful drawing, annotation, and editing functions of the AutoCAD platform software but also provides practical and professional extensions specifically tailored to the mechanical industry. It features an efficient drawing mode with quick coordinate input.

Yaochuang CAD V10 is the flagship product of Yaochuang CAD in 2019. Compared to previous versions, it significantly improves the performance of the product, supporting fast and smooth editing of large and extra-large drawings. It also provides comprehensive support for dimension and entity associations. The newly added enterprise resource library functionality enables companies to independently establish their own libraries and material databases.

<div class="center">
    <img src="https://raw.githubusercontent.com/ingw3216/blogimage/main/img/CAD3.png" style="width:70%;">
</div>

**a.Different Version**
<div class="center">
    <img src="https://raw.githubusercontent.com/ingw3216/blogimage/main/img/CAD4.jpg" style="width:70%;">
</div>

**b.Basic Functions**
<div class="center">
    <img src="https://raw.githubusercontent.com/ingw3216/blogimage/main/img/CAD5.png" style="width:70%;">
</div>