# 2.Fusion

本次《设计工程学》的课程，主要讲授了Fusion的使用方法。

## 2.1 插件安装过程
(1) 点击实用程序的附加模块里的Fusion 360 APP store，搜索需要的插件，如gear
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231019114347.png"  height="300px">
</div>
(2) 选择合适的插件下载（需要登陆账号）
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231019114416.png"  height="300px">
</div>
(3) 双击运行安装包
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231019114443.png"  height="300px">
</div>
(4) 安装完成后，在脚本和附加模块中就有了安装的插件
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231019114556.png"  height="300px">
</div>
(5) 在页面上出现图标，点击运行即可按照需求创建齿轮
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231019114655.png"  height="300px">
</div>


## 2.2 零件建模过程
(1) 在zju2023内新建小组文件夹，进入草图，绘制一个中心矩形，长宽都为200mm
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231018233509.png"  height="300px">
</div>
(2) 顶部视图完成中心矩形汇总后，倒四次圆角，得到圆角矩形，圆角40mm
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231019001118.png"  height="300px">
</div>
(3) 草图中绘制一个圆，准备扫掠
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231018234643.png"  height="300px">
</div>
(4) 通过绘制的圆角矩形和园进行扫掠
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231018235205.png"  height="300px">
</div>
(5) 从实体创建零件（后续部分都需要转化为零件，或者一开始就设置为零件），然后创建草图圆管
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231018235820.png"  height="300px">
</div>
环形阵列得到四个相同的部分，再完成一个圆和一条垂直直线的绘制
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231018235841.png"  height="300px">
</div>
(6) 移动复制圆，再用扫掠的方法得到圆环
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231018235907.png"  height="300px">
</div>
(7) 移动复制得到另一个圆环，再绘制轮廓线
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231018235948.png"  height="300px">
</div>
(8) 挤出后剪切掉圆环的一部分
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231019000015.png"  height="300px">
</div>
(9) 圆、直线、剪切命令绘制跑道圆，拉伸得到一个零件
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231019000038.png"  height="300px">
</div>
(10) 绘制两个圆，用于剪切
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231019000116.png"  height="300px">
</div>
(11) 拉伸后剪切得到下图，草图生成矩形后剪切得到下图
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231019000135.png"  height="300px">
</div>
(12) 环形阵列得到下图
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231019000204.png"  height="300px">
</div>
(13) 绘制圆柱，再做一个圆柱并合并
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231019001451.png"  height="300px">
</div>
(14) 绘制草图后挤出
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231019001520.png"  height="300px">
</div>
(15) 通过倒角和圆柱得到下图
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231019001548.png"  height="300px">
</div>
(16) 通过草图挤出得到下图，并绘制了一个圆柱减除部分零件
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231019001610.png"  height="300px">
</div>
(17) 绘制一个圆柱、一个圆管，两者可以组成一个伸缩结构
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231019001637.png"  height="300px">
</div>
(18) 人工智能的部件生成（生成效果一般，最终未采用）
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231019001719.png"  height="300px">
</div>
(19) 对细节进行补充
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231019001741.png"  height="300px">
</div>
(20) 倒圆角并且选择了材质方便观察
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231019001851.png"  height="300px">
</div>
(21) 最终在装配时系统多次崩溃，故存在一定的欠缺，暂未找到解决该问题的办法。
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231019001812.png"  height="300px">
</div>



## 2.3 零件建模图例

<iframe width=640 height=480 src="https://a360.co/48R9Go6" ></frame>
