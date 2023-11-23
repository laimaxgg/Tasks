# HTML学习笔记

## 1. HTML基础

HTML（Hypertext Markup Language）是用于构建网页结构的标记语言。以下是一些常用的HTML标签，它们构成了网页的基本元素：

- `<html>`: HTML文档的根元素。

- `<head>`: 包含文档的元（meta）信息，如标题、字符集等。

- `<title>`: 定义网页的标题，显示在浏览器的标签页上。

- `<body>`: 包含页面的内容，如文本、图片、链接等。

- <mta>:标签定义字符集等元信息。

```html
- <!DOCTYPE html>
  <html>
  <head>
      <title>页面标题</title>
       <meta charset="UTF-8">
  </head>
  <body>
      <!-- 页面内容 -->
  </body>
  </html>
```


## 2. 常用HTML标签

### 2.1 块级元素

块级元素在页面中以块的形式展现，通常会占据一整行，常用的块级元素有：

- `<div>`: 定义文档中的一个区块，通常用于组织页面结构。
- `<p>`: 定义段落。
- `<h1>` to `<h6>`: 定义标题，数字越小，级别越大。

### 2.2 内联元素

内联元素只占据它所在标签的边框所包含的空间，常用的内联元素有：

- `<a>`: 定义超链接，用于跳转到其他页面。
```html 
<a href="https://github.com/laimaxgg/Tasks">我的GitHub仓库网址</a>
```

- `<span>`: 用于对文本的一部分进行样式设置或脚本操作。
- `<strong>`或`<b>`: 定义强调文本，通常以粗体显示。
```html
<strong>重要文本</strong>
```

-`<em>`或`<i>`:定义斜体文本。
```htnl
<em>斜体文本</em>
```

### 3. 块级元素与内联元素

理解块级元素和内联元素在页面布局中的不同是HTML学习的关键之一。

- **块级元素**：独占一行，从上至下垂直排列，可以包含其他块级元素和内联元素。常用于页面结构的划分，如`<div>`和`<p>`。
- **内联元素**：在同一行内水平排列，不会打断文本的流程，只包含对文本的处理。常用于设置文本样式，如`<a>`和`<span>`。

## 4. HTML标签的样式

HTML标签可以通过CSS（Cascading Style Sheets）来进行样式设置，以改变其外观和布局。以下是一些常见的样式相关的HTML属性：

- **class和id属性**：用于标识和选择特定的HTML元素，方便在CSS中进行样式定义。

  ```html
  htmlCopy code<div class="container" id="main-container">
    <!-- 内容 -->
  </div>

- **style属性**：直接在HTML标签中定义样式。

- ```<p style="color: blue; font-size: 16px;">这是一个蓝色的段落</p>```

- **链接样式**：通过CSS设置超链接的样式，定义未访问、已访问和悬停时的外观。

  ```css
  cssCopy codea:link {
    color: black;
  }
  
  a:visited {
    color: purple;
  }
  
  a:hover {
    color: red;
  }

