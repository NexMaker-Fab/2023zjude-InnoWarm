# 1. Webpage

The second session of Design Engineering focused on the steps involved in building a website. Utilizing the html/markdown language, the group stored process data (including images, text, etc.) in both github and local disks, and generated the webpage architecture.

## 1.1 Basic Framework 
We created a public repository on Github (following pictures are not this web but an example)

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231023213201.png" >
  </div>

Create a new file on the Github web and edit it.

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231023212722.png" >
  </div>

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231023212746.png" >
  </div>

After repository had been built, we opened the Github Desktop and find our repository which we wanted to clone to the local disk.

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231025104307.png" >
  </div>
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231025104345.png" >
  </div>


Once the repository has been cloned, we can open and edit it offline.

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231025104431.png" >
  </div>

Finally, with the following steps we can configure and initialize the local environment.

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



>**Problem**: Unable to load docsify.ps1, because running scripts is prohibited on this system!
>
>**Solution**: Run Powershell with administrator privileges and type "Set-ExecutionPolicy -ExecutionPolicy RemoteSigned"to change the script execution policy.

<body>
  <div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231005234205.png" alt="Fig3. Solution">
  </div>
</body>

## 1.2 Markdown
When writing the website, we  build the basic framework  by comprehensively studying and referring to the syntax rules and typical cases given by NexMakerLab, ChatGPT, Github and other platforms, and some cases are given below.

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

## 1.3 Picture Upload
We adopted a suggestion from Zhihu user <a href="https://zhuanlan.zhihu.com/p/489236769">@小小芋子</a>, uploading the image on PicGo to another repository on Github, and invocates the image via Personal Access Tokens to reduce the burden on the web page file.


We go to https://github.com/settings/tokens

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231023215041.png" >
</div>

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231023215214.png" >
</div>

In Pic Go, we select the "Github" option of the settings and paste the copied Tokens accordingly.

<body>
  <div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231025111355.png" alt="Fig4. Github setting">
  </div>
</body>

<body>
  <div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231005235451.png" alt="Fig5. blogimage">
  </div>
</body>



## 1.4 Video Upload

We made an attempt to upload the Asian Games opening ceremony video from CCTV news on Bilibili

The initial version of the video was as follows:

  <iframe src="//player.bilibili.com/player.html?aid=661274868&bvid=BV1hh4y1a79W&cid=1277112324&p=1"></iframe>


>**Problem**：The video cannot be viewed properly due to the restricted height.
>
>**Solution**：Set: width="600" height="auto"

<iframe width="600" height="atuo" 
src="//player.bilibili.com/player.html?aid=661274868&bvid=BV1hh4y1a79W&cid=1277112324&p=1" 
scrolling="no" border="0" frameborder="0" allowfullscreen>
</iframe>

```
{
<iframe width="600" height="500" src="//player.bilibili.com/player.html?aid=661274868&bvid=BV1hh4y1a79W&cid=1277112324&p=1" scrolling="no" border="0" frameborder="0" allowfullscreen></iframe>
}
``` 
## 1.5 Group Invitation

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231025112242.png">
  </div>

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231025112322.png">
  </div>

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231025112400.png">
  </div>

## 1.6 Future Enhancements

The interface is simple and the content is thin. In the subsequent lessons, we can refer to different materials and tutorials, and continue to explore more diversified screens and more interesting web interactions~

## 1.7 Reference & Acknowledgment

This coursework was completed with reference to the 2022 course work, thanks to the SoFarSoGood team, and thanks to Xinrui Li, Software Engineering 2023, for providing valuable suggestions for revisions.
