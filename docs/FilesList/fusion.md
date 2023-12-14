# 2.Fusion

Fusion 360 is a comprehensive design software developed by Autodesk, originally known as "Inventor Fusion" when it was first introduced in 2009. It provides a powerful set of tools and features for 3D modeling, CAD (Computer-Aided Design), CAM (Computer-Aided Manufacturing), CAE (Computer-Aided Engineering), as well as collaboration and data management.
The design philosophy of Fusion 360 is to integrate design, engineering, and manufacturing into a unified platform, offering users a holistic design and manufacturing solution. It features an intuitive user interface, cloud storage, and collaboration capabilities, assisting designers, engineers, and manufacturers in creative design, product development, and optimization of manufacturing processes.

With Fusion 360, users can perform parametric modeling, assembly design, surface modeling, rendering, animation, and more. It also provides powerful simulation and analysis tools to validate design performance and behavior. Additionally, Fusion 360 supports integration with other design software, enabling collaboration and data exchange with professionals from different fields.

In summary, Fusion 360 is a powerful design software aimed at providing users with a comprehensive design, engineering, and manufacturing solution. Its design philosophy revolves around integrating various stages of the design and manufacturing process, offering an intuitive interface, and facilitating cloud-based collaboration. Through Fusion 360, users can achieve creative design, product development, and optimization of manufacturing processes.。

## Part Modeling
(1) 在zju2023内新建小组文件夹，进入草图，绘制一个中心矩形，长宽都为200mm
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/1.png"  style="width:70%;">
</div>
(2) 顶部视图完成中心矩形汇总后，倒四次圆角，得到圆角矩形，圆角40mm
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/2.png"  style="width:70%;">
</div>
(3) 草图中绘制一个圆，准备扫掠
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/3.png" style="width:70%;">
</div>
(4) 通过绘制的圆角矩形和园进行扫掠
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/4.png"  style="width:70%;">
</div>
(5) 从实体创建零件（后续部分都需要转化为零件，或者一开始就设置为零件），然后创建草图圆管
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/5.png" style="width:70%;">
</div>
环形阵列得到四个相同的部分，再完成一个圆和一条垂直直线的绘制
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/6.png"  style="width:70%;">
</div>
(6) 移动复制圆，再用扫掠的方法得到圆环
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/7.png"  style="width:70%;">
</div>
(7) 移动复制得到另一个圆环，再绘制轮廓线
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/8.png"  style="width:70%;">
</div>
(8) 挤出后剪切掉圆环的一部分
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/9.png"  style="width:70%;">
</div>
(9) 圆、直线、剪切命令绘制跑道圆，拉伸得到一个零件
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/10.png"  style="width:70%;">
</div>
(10) 绘制两个圆，用于剪切
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/11.png"  style="width:70%;">
</div>
(11) 拉伸后剪切得到下图，草图生成矩形后剪切得到下图
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/12.png"  style="width:70%;">
</div>
(12) 环形阵列得到下图
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/13.png"  style="width:70%;">
</div>
(13) 绘制圆柱，再做一个圆柱并合并
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/14.png"  style="width:70%;">
</div>
(14) 绘制草图后挤出
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/14-1.png"  style="width:70%;">
</div>
(15) 通过倒角和圆柱得到下图
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/15.png"  style="width:70%;">
</div>
(16) 通过草图挤出得到下图，并绘制了一个圆柱减除部分零件
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/16.png"  style="width:70%;">
</div>
(17) 绘制一个圆柱、一个圆管，两者可以组成一个伸缩结构
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/17.png"  style="width:70%;">
</div>
(18) 人工智能的部件生成（生成效果一般，最终未采用）
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/18.png"  style="width:70%;">
</div>
(19) 对细节进行补充
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/19.png"  style="width:70%;">
</div>
(20) 倒圆角并且选择了材质方便观察
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20.png"  style="width:70%;">
</div>


## Simulation Video

Motion simulation model building process video:

<iframe style="width:70%;" height=500 src="//player.bilibili.com/player.html?aid=832564395&bvid=BV1834y1u7Hv&cid=1311044014&p=1"  frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


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

## Automated Modeling Examples
AI automated modeling process video:

<iframe style="width:70%;" height=500 src="////player.bilibili.com/player.html?aid=962553267&bvid=BV11H4y197KG&cid=1311074464&p=1"  frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

## Other Software
(1) <a href="https://www.zwcad.com/">ZWSOFT CAD</a>

ZWSOFT（中望） CAD is a professional engineering modeling software independently developed in China, widely used in fields such as architecture, mechanical engineering, and power industry. It is based on an independent kernel and is a 2D CAD platform that is fully compatible with the DWG format. It extensively supports mainstream industry applications and customized development of user-specific functions. Since its launch in 2002, ZWSOFT CAD has helped users in various industries such as architecture, surveying, urban planning, mechanical manufacturing, electronics, and power achieve efficient design and domestic innovation.

ZWSOFT CAD provides powerful modeling, analysis, and design functions, assisting engineers in precise 3D modeling and simulation analysis. It features efficient algorithm optimization and high versatility, including batch printing, sheet sets, dynamic blocks, PDF import, and lasso selection. The software operates at high speed, offers comprehensive functionality, and has a high level of intelligence, enabling designers to rapidly complete complex design tasks.
<div class="center">
    <img src="https://raw.githubusercontent.com/ingw3216/blogimage/main/img/CAD6.png" style="width:70%;">
</div>

a.Main Features
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/CAD7.png" style="width:70%;">
</div>

b.Functionality
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

a.Different Version
<div class="center">
    <img src="https://raw.githubusercontent.com/ingw3216/blogimage/main/img/CAD4.jpg" style="width:70%;">
</div>

b.Basic Functions
<div class="center">
    <img src="https://raw.githubusercontent.com/ingw3216/blogimage/main/img/CAD5.png" style="width:70%;">
</div>