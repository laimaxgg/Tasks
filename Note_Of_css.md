# CSS学习笔记

## 1. CSS的作用

CSS，即层叠样式表（Cascading Style Sheets），是一种用于描述文档样式的样式表语言。它为网页提供了丰富的样式控制，可以让页面变得更加美观和易于阅读。CSS的主要作用包括：

- **样式控制：** 通过CSS，可以控制页面中元素的外观，如颜色、大小、字体等，使页面更符合设计需求。

- **布局控制：** CSS允许定义元素在页面中的位置和排列方式，实现灵活的页面布局。

- **响应式设计：** CSS可以根据不同的设备和屏幕尺寸调整页面布局，以提供更好的用户体验。

## 2. CSS选择器

CSS选择器用于选择页面中的元素，从而应用样式。

- **通用选择器（`*`）：**用于选择页面上的所有元素。例如，要将所有元素的边框颜色设为红色，可以使用以下CSS规则：

- ```css
  * {
    border-color: red;
  }
  ```

- **元素选择器（例如，`p`、`div`）：** 用于选择特定的HTML元素。例如，要设置所有段落的文本颜色为蓝色，可以这样写：

  ```css
  p {
    color: blue;
  }
  ```

- **类选择器（`.`）：** 用于选择具有相同类名的元素。比如，有一个类名为 "highlight" 的样式：

  ```css
  .highlight {
    background-color: yellow;
  }
  ```

- **ID选择器（`#`）：** 用于选择具有唯一ID的元素。例如，要设置ID为 "header" 的元素的字体大小为20像素：

  ```css
  #header {
    font-size: 20px;
  }
  ```



## 3. 设置元素的基础样式

利用CSS设置元素的基础样式

- **大小：** 使用`width`和`height`属性设置元素的宽度和高度。

- **颜色：** 使用`color`属性设置文本颜色，使用`background-color`属性设置背景颜色。

- **文字字体：** 使用`font-family`属性设置字体，`font-size`设置字体大小。

### 示例：

```css
/* 设置文字颜色为绿色 */
body {
  color: green;
}

/* 设置标题的字体大小为24像素 */
h1 {
  font-size: 24px;
}

/* 设置段落的行高为1.5倍 */
p {
  line-height: 1.5;
}
```

## 4. CSS的盒模型

CSS中的盒模型是描述元素占用空间的模型，包括内容、内边距、边框和外边距。理解盒模型就像理解一个盒子的构成，有内容是盒子里的物品，内边距是物品与盒子边缘的距离，边框是盒子的边界，外边距是盒子与其他盒子之间的距离。

```css
/* 设置元素内边距为10像素 */
div {
  padding: 10px;
}

/* 设置元素边框为1像素实线，颜色为黑色 */
p {
  border: 1px solid black;
}

/* 设置元素外边距为20像素 */
img {
  margin: 20px;
}
```

## 5. CSS的position定位

CSS提供了5种定位方式，分别是：

- **static（默认）：** 元素在正常文档流中的位置，不受top、right、bottom、left的影响。

- **relative：** 相对于元素正常位置进行定位。

- **absolute：** 相对于最近的已定位父元素进行定位，如果没有已定位的父元素，则相对于`<html>`元素。

- **fixed：** 相对于浏览器窗口进行定位，元素固定在页面上。

- **sticky：** 元素根据用户滚动的位置定位，它的行为就像`relative`和`fixed`的组合。

```css
/* 相对定位，相对于元素原本的位置进行定位 */
div {
  position: relative;
  top: 10px;
  left: 20px;
}

/* 绝对定位，相对于最近的已定位父元素进行定位 */
p {
  position: absolute;
  top: 30px;
  right: 10px;
}

/* 固定定位，相对于浏览器窗口进行定位 */
header {
  position: fixed;
  bottom: 0;
  width: 100%;
}

/* 粘性定位，根据用户滚动的位置进行定位 */
nav {
  position: sticky;
  top: 0;
}

/* 静态定位，元素在正常文档流中的位置 */
span {
  position: static;
}
```

## 6. 常用布局方式

CSS提供了多种布局方式，其中一些常见的包括：

- **Flex布局：** 使用`display: flex`实现弹性盒子布局，方便地实现水平和垂直方向的布局。

- **Grid布局：** 使用`display: grid`实现网格布局，更灵活地控制元素的位置。

```css
/* 布局方式示例 */
.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.grid-container {
  display: grid;
  grid-template-columns: 1fr 2fr 1fr;
}
```

## 7. CSS的伪类

CSS伪类是一种用于向选择器添加特殊效果的关键字。常见的伪类包括`:hover`（鼠标悬停时应用样式）、`:active`（元素被激活时应用样式）等。

```css
/* 鼠标悬停时改变链接的颜色 */
a:hover {
  color: red;
}
```

