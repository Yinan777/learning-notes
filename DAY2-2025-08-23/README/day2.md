# ⭐表格与表单

> **视频来源：** [【B站】黑马程序员 - 前端Web开发HTML5+CSS3+移动web](https://www.bilibili.com/video/BV1kM4y127Li)<br>
> **观看进度：** P16 ~ P27<br>
> **日期：** 2025-08-23

---

## ✨ 核心观点 (The Gist)
今天学会了表格中如何**合并单元格**，学会了表单中的许多种格式，也制作了一个**注册信息的表单**。
---

## 📝 我的笔记 (My Notes)

###  **1.定义列表**
可以运用在网页下部的帮助中心，一个标题对应多个内容
  ```html
  <dl>
    <dt>列表标题</dt>
    <dd>列表详情</dd>
    ...
</dl>
``` 
### 2.表格
| 标签名 | 解释 | 说明 |
| :--- | :--- | :--- |
| **table** | 表格 | |
| **tr** | 行 |  |
| **th** | 表头单元格| 单元格内默认居中加粗|
| **td** | 内容单元格| |
| **border** | 增加表格边框线| 值为1|

### 3.合并单元格
**合并单元格的步骤**
* 1.明确合并的目标（相同信息）
* 2.保留最左最上的单元格，添加属性（取值是数字，表示**需要合并的单元格数量**）<br>
  -跨行合并，保留最上单元格，添加属性**rowspan**<br>
  -跨列合并，保留最左单元格，添加属性**colspan**
* 3.删除其他单元格
```html
  <tr rowspan="1">1</tr>
```
### 4.表单
* **①input标签**<br>
input标签type属性值不同，则功能不同
```html
<!-- 1.placeholder默认显示浅色文字，用户输入即消失 -->
<input type="text" placeholder="请输入用户名">
<!-- 2.性别radio单选框 -->
<input type="radio" name="gender" checked>男
<input type="radio" name="gender">女
  <!-- name相同表示两个单选框为同一组，同一组只能选中一个（单选功能） -->
  <!-- checked表示默认选中 -->
<!-- 3.上传文件file -->
<input type="file" mutiple>
  <!-- mutiple可以实现文件多选功能 -->
<!-- 4.多选框checkbox -->
<input type="checkbox" checked>
```
| type属性 | 说明 | 
| :--- | :--- | 
| **text** | 文本框，用于输入单行文本 | 
| **password** | 密码框 |  
| **radio** | 单选框| 
| **checkbox** | 多选框| 
| **file** | 上传文件|
* **②下拉菜单**
```html
城市：
<!-- 无selected,默认第一位 -->
<select>
  <option>北京</option>
  <option>上海</option>
  <option>广州</option>
  <option>深圳</option>
  <option selected>武汉</option>
</select>
```
* **③文本域**
```html
  <!-- 事例：评论区回复 -->
  <!-- 右下角有拖拽功能，未来会禁用 -->
  <textarea>请输入评论</textarea>
```
* **④label标签**
  用label标签绑定文字和表单控件的关系，增大表单控件的点击范围。
```html 
  <!-- label标签for属性值和表单控件id属性值相同，可以增大点击范围,上方的type都可以用label -->
  <input type="radio" id="man">
  <label for="man">男</label >
  <!-- 另一种方法 -->
  <label><input type="radio">女</label>
```
* **⑤按钮button**
```html
  <!-- form表单区域，提交重置时确定需要的范围 -->
  <form action="">
    <!-- action=""发送数据的地址 -->
    <button type="">按钮</button>
```
| type属性 | 说明 | 
| :--- | :--- | 
| **submit** | 提交按钮，点击后可以提交数据到后台（默认功能） | 
| **reset** | 重置按钮，点击后将表单控件恢复默认值 |  
| **button** | 普通按钮，默认没有功能，一般配合javascript使用| 
* **5.无语义的布局标签**
用于布局网页
```html
<!-- div大盒子 -->
<div>div标签，独占一行</div>
<!-- span小盒子 -->
<span>span标签，不换行</span>
```
* **6.字符实体**<br>
在代码中敲键盘的空格，网页只识别一个。

| 显示结果 | 描述 | 实体名称 |
| :--- | :--- | :--- |
| **空格** | 空格 |&nbsp+; |
| **<** | 小于号 | &lt+; |
| **>** | 大于号| &gt+;|
---

## 🕰️ 基础项目制作
### 1.注册信息
* 📝完成一个包括个人信息，教育经历，工作经历的注册表单
* 🔗 相关链接(Links)：[注册信息表单HTML](../code-snippets/注册信息.html)


## ❓ 问题与思考 (Questions & Thoughts)
*   **问题**
    *   ⏳如何将表单提交到后台呢，后台如何建设呢？
*   **想法和灵感**
    *   💡对于各个网页的注册登录页面都需要用到表单的知识。

---