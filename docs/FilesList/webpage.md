# 1. Webpage

第二次《设计工程学》的课程，主要讲授了网站搭建的相关步骤。利用html/markdown语言，本小组将过程数据同时储存在github及本地磁盘中（包括图片、文本等），并生成网页架构。 

## 1.1 框架搭建
We created a public repository on Github (following pictures are not this web but an example)

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231023213201.png" >
  </div>

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231023212722.png" >
  </div>

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231023212746.png" >
  </div>

After repository had been built, we opened the Github Desktop and find our repository which we wanted to clone to the local disk.

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231023212840.png" >
  </div>

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231023212939.png" >
  </div>
  
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231023213003.png" >
  </div>

最后，我们按照如下步骤进行本地环境配置与初始化。

```
{
PS C:\Users\yw\Desktop\InnoWarm> npm i docsify-cli -g
changed 204 packages in 1m
16 packages are looking for funding
run ‘npm fund‘ for details
}
```

```
PS C:\Users\yw\Desktop\InnoWarm> npm i docsify-sidebar-collapse
added 1 package in 7s

```

```
{
PS C:\User\yw\Desktop\InnoWarm> docsify serve docs
Serving C: Users\yw\Desktop\InnoWarm\docs now.
Listening at http://localhost:3000
}
```

>**遇到问题**：无法加载docsify.ps1，因为在此系统上禁止运行脚本
>
>**解决方案**：管理员权限运行Powershell，输入Set-ExecutionPolicy -ExecutionPolicy RemoteSigned，更改脚本执行策略。


<body>
  <div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231005234205.png" alt="Fig3. Solution">
  </div>
</body>

## 1.2 Markdown语言
在编写网站时，我们通过综合学习与参考NexMakerLab、ChatGPT、Github等平台给出的语法规则与典型案例，逐步地搭建出本网站的基本框架，以下给出部分案例。

(1) title/sidebar/search

```
{
  <body>
  <div id="app"></div>
  <script>
    window.$docsify = {
      name: 'InnoWarm',
      repo: '',
      loadSidebar: true,
      loadNavbar: true,
      subMaxLevel: 2,
      search: {
        paths: 'auto',
        placeholder: '搜索',
        noData: '无结果',
        depth: 4,
      },
    }

}
``` 

(2) header

```
{
  # First-Level Title
  ## Second-Level Title
  ### Third-Level Title
}
``` 

(3) picture

```
{
  <div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231005231359.png" alt="Fig1. Install docsify">
  </div>
}
``` 

(4) link

```
{
 <a href="https://www.zju.edu.cn">标题</a>
}
``` 

## 1.3 图片上传

小组采用了知乎用户@小小芋子的<a href="https://zhuanlan.zhihu.com/p/489236769">
建议</a>，在PicGo上将图片上传至专门Github的另一Repository内，通过Personal Access Tokens调用图片以减轻网页文件的负担。

We created a repository to save public images, and got Personal Access Tokens by taking steps as follow:

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231023215041.png" >
</div>

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231023215214.png" >
</div>
我们在Pic Go中选择图床设置的“Github”选项，并进行相应设置


<body>
  <div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231005235445.png" alt="Fig4. Github setting">
  </div>
</body>

<body>
  <div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231005235451.png" alt="Fig5. blogimage">
  </div>
</body>



## 1.4 视频上传

我们将Bilibili上央视新闻的亚运会开幕式视频进行了上传尝试：
最初版本的代码如下：

  <iframe src="//player.bilibili.com/player.html?aid=661274868&bvid=BV1hh4y1a79W&cid=1277112324&p=1"></iframe>


>**遇到问题**：视频的高度受限，视频无法正常观看。
>
>**解决方案**：设置width="600" height="auto"

<iframe width="600" height="500" src="//player.bilibili.com/player.html?aid=661274868&bvid=BV1hh4y1a79W&cid=1277112324&p=1" scrolling="no" border="0" frameborder="0" allowfullscreen></iframe>

## 1.5 可待改进

界面单调，内容单薄。在后续的课程中，我们可以参考不同的素材与教程，继续探索更为多元的画面、更加有趣的网页交互方式~

## 1.6 Reference & Acknowledgment

本次课程作业的完成参考了2022年的课程作品，感谢SoFarSoGood小组，感谢软件工程23级李新锐同学提供的宝贵修改建议。
