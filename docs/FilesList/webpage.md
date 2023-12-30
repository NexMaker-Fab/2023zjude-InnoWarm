# 1. Webpage

The second session of Design Engineering focused on the steps involved in building a website. Utilizing the html/markdown language, the group stored process data (including images, text, etc.) in both github and local disks, and generated the webpage architecture.

## 1.1 Basic Framework 
We created a public repository on Github (following pictures are not this web but an example)

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231023213201.png" style="width:75%;" >
  </div>

Create a new file on the Github web and edit it.

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231023212722.png" style="width:75%;" >
  </div>

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231023212746.png" style="width:75%;" >
  </div>

After repository had been built, we opened the Github Desktop and find our repository which we wanted to clone to the local disk.

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231025104307.png" style="width:75%;" >
  </div>
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231025104345.png" style="width:75%;">
  </div>


Once the repository has been cloned, we can open and edit it offline.

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231025104431.png" style="width:75%;">
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
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231005234205.png" style="width:75%;">
  </div>
</body>

Fold and File Relationship
<body>
  <div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/foldandfile.png" style="width:75%;" >
  </div>
</body>

## 1.2 Markdown
When writing the website, we  build the basic framework  by comprehensively studying and referring to the syntax rules and typical cases given by NexMakerLab, ChatGPT, Github and other platforms, and some cases are given below.

(1) headers

```
{
  # First-Level Title
  ## Second-Level Title
  ### Third-Level Title
}
``` 
Display results:
  # First-Level Title
  ## Second-Level Title
  ### Third-Level Title
(2) emphasis
```
{
  italics use single star/underscore: *text* or_text_ 
  bold use double stars/underscores: **text** or __text__
  Strikethrough use double tildes: ~~text~~
}
``` 
Display Results:

italics use single star/underscore: *text* or _text_ 

bold use double stars/underscores: **text** or __text__

Strikethrough use double tildes: ~~text~~

(3) picture

**Markdown method:**

```
{
  <div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231005231359.png" alt="Fig1. Install docsify">
  </div>
}
``` 
Display results:
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231005231359.png" style="width:75%;">
  </div>


**Origin Method:**
```
{
  ![Fig1. Install docsify](https://github.com/ingw3216/blogimage/raw/main/img/20231005231359.png)
}
```
Display results:

![Fig1. Install docsify](https://github.com/ingw3216/blogimage/raw/main/img/20231005231359.png)

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
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231023215041.png" style="width:75%;" >
</div>

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231023215214.png" style="width:75%;">
</div>

In Pic Go, we select the "Github" option of the settings and paste the copied Tokens accordingly.

<body>
  <div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231025111355.png" style="width:75%;">
  </div>
</body>

<body>
  <div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231005235451.png" style="width:75%;">
  </div>
</body>



## 1.4 Video Upload

We made an attempt to upload the Asian Games opening ceremony video from CCTV news on Bilibili

The initial version of the video was as follows:

  <iframe src="//player.bilibili.com/player.html?aid=661274868&bvid=BV1hh4y1a79W&cid=1277112324&p=1"></iframe>


>**Problem**：The video cannot be viewed properly due to the restricted height.
>
>**Solution**：Set: aspectratio="16:9" width="100%" height="600"

<iframe width="100%" height="650" 
src="//player.bilibili.com/player.html?aid=661274868&bvid=BV1hh4y1a79W&cid=1277112324&p=1" 
scrolling="no" border="0" frameborder="0" allowfullscreen>
</iframe>

```
{
<iframe src="//player.bilibili.com/player.html?aid=661274868&bvid=BV1hh4y1a79W&cid=1277112324&p=1" aspectratio="16:9" width="100%" height="600"> </iframe>
}
``` 
## 1.5 Group Invitation

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231025112242.png" style="width:75%;">
  </div>

<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231025112322.png" style="width:75%;">
  </div>

In order to protect the safety of the project, team members are given permission to write only.
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/20231108225447.png" style="width:75%;">
  </div>

## 1.6 Project Update

We use Github Desktop to update the project. The following is the update process of the project.
<div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/update.png" style="width:75%;">
  </div>

  <div class="center">
    <img src="https://github.com/ingw3216/blogimage/raw/main/img/update1.png" style="width:75%;">
  </div>


## 1.7 Reference & Acknowledgment

This coursework was completed with reference to zjude2022, thanks to the SoFarSoGood team, and thanks to Xinrui Li, Software Engineering 2023, for providing valuable suggestions for revisions.
