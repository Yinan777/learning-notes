# ⭐Html基础知识

> **视频来源：** [【B站】黑马程序员 - 前端Web开发HTML5+CSS3+移动web](https://www.bilibili.com/video/BV1kM4y127Li)<br>
> **观看进度：** P1 ~ P15<br>
> **日期：** 2025-08-21

---

## ✨ 核心观点 (The Gist)
用一两句话总结你今天学到的**最重要**的一件事。强迫自己总结，这是记忆的关键。

---

## 📝 我的笔记 (My Notes)
在这里自由地记录。不要管顺序和结构，先把你听到、看到、想到的所有东西“倾倒”出来。
### 1.标签
*   **标签**可以分为**单标签**和**双标签**;<br>
*   **单标签**只有开始标签，无结束标签，**只需要一个效果而没有内容时使用**;<br>
  例：br:换行  hr:水平线<br>
*   **双标签**是成对出现的标签，**需要包裹内容时使用**
  例：strong加粗/strong等;
### 2.VS Code**快速生成骨架**：<br>
* 在HTML文件(.html)中，**!(英文)配合Enter/Tab键**
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
    </head>
    <body>
    
    </body>
    </html>
    ```
### 3.相关快捷键
*   注释快捷键**ctrl+/**
*   代码中间向下换行**ctrl+enter**
*   将左边栏收起**ctrl+b**
### 4.文本格式化标签
| 标签名 | 效果 |               
| :--- | :--- | 
| **strong** | 强调 |
| **em** | 倾斜 | 
| **ins** | 下划线|
| **del**|删除线|
### 5.图像标签
```html
<!-- 引号内为图片的URL -->
<!-- 以前网速慢，可能导致图片加载不出来，不想影响网页内容的浏览，用alt替换表明这张图片的内容 -->
<!-- title表示鼠标悬停在图片上显示文字，传达含义 -->
<!-- 浏览器缩放图片，只指定高度或者宽度时，默认是等比例缩放 -->
<img src="./img1.jpg" alt="这张图片的内容" title="这张图片的内容" width="100">

<!-- 图片的相对路径 -->
 <!-- 若当前HTML文件与图片在同一个文件夹中,使用"./图片名"  -->
<img src="./img1.jpg">
 <!-- 若当前HTML文件与包含所需图片的文件夹images在同一个文件夹中,使用"./images/图片名"  -->
<img src="./images/img2.jpg">
 <!-- 若所需图片在当前HTML文件的上一层文件夹中,使用"../图片名"  -->
<img src="../img3.jpg">
 <!-- 总结："."表示当前文件所在文件夹,".."表示当前文件上一级文件夹，"/"表示进入某个文件夹里面 -->
<!-- 图片的绝对路径 -->
 <!-- C盘images文件夹中的图 -->
 <img src="C:/images/img1.jpg">
 <!-- 网址上的图片，复制图片的地址 -->
 <img src="https://360.itheima.com/special/brandzly1/images/logohm.png">
```
| 属性 | 作用 | 说明 |
| :--- | :--- | :--- |
| **alt** | 替换文本 | 图片无法显示的时候显示的文字 |
| **title** | 提示文本 | 鼠标悬停在图片上面的时候显示的文字 |
| **width** | 图片的宽度| 值为数字|
| **height** | 图片的高度| 值为数字 |

### 6.超链接
```html
<!-- target="_blank"在新窗口跳转页面 -->
<a href="https：//www.baidu.com/" target="_blank">跳转到百度</a>
 <!-- href属性值写#，表示空链接 -->
<a href="#" target="_blank">无法跳转</a>
```

### 7.音频与视频
**音频**
```html
<!-- 在HTML5中，如果属性名和属性值完全一样，可以简写为一个单词 -->
<audio src="./media/music.mp3" controls loop></audio>
```
| 属性 | 作用 | 特殊说明 |
| :--- | :--- | :--- |
| **src(必须属性)** | 音频URL | 支持格式：MP3,Ogg,Wav |
| **Controls** | 显示音频控制面板 |  |
| **loop** | 循环播放| |
| **autoplay** | 自动播放| 为了提升用户体验，浏览器一般会禁用自动播放功能 |
 **视频**
 ```html
<video src="./media/vue.mp4" controls loop muted autoplay></video>
```
| 属性 | 作用 | 特殊说明 |
| :--- | :--- | :--- |
| **src(必须属性)** | 视频URL | 支持格式：MP3、4,WebM,Ogg |
| **Controls** | 显示视频控制面板 |  |
| **loop** | 循环播放| |
| **muted** | 静音播放| |
| **autoplay** | 自动播放| 为了提升用户体验，浏览器支持在静音状态下自动播放功能 |

---

## 🕰️ 基础项目制作
### 1.个人简介
## ❓ 问题与思考 (Questions & Thoughts)
*   这里记录你没听懂、或者想进一步探索的问题。
    *   例如：*Mermaid 图表和 PlantUML 有什么区别？*
*   也可以记录你自己的想法和灵感。
    *   例如：*这个概念好像可以用在我正在做的XX项目里。*

---

## 🔗 相关链接 (Links)
*   [这是一个有用的链接](https://example.com)
*   [[以后可能会链接到的另一篇笔记]]

---