## Canvas

#### 一、什么是canvas

`canvas` (画布)是一个可以使用脚本(通常为JavaScript)来绘制图形的html标签.

`canvas` 元素本身是没有绘图能力的。所有的绘制工作必须在 JavaScript 内部完成，相当于使用画笔在画布上画.

`canvas` 默认大小W300*H150,是一个没有边框及内容的空白画布,可以通过width、height属性设置宽高.

```html
<canvas id="paint" width="100px" height="100px"></canvas>
```

#### 二、基本用法

##### 1.渲染上下文 getContext()

我们在页面中创建一个 canvas 标签之后，首先要使用 `getContext()` 获取 canvas 的上下文环境，这个方法用来获得渲染上下文和它的绘画功能.

`getContext("2d")` 对象是内建的 HTML5 对象，拥有多种绘制路径、矩形、圆形、字符以及添加图像的方法.

```js
let canvas = document.getElementById('paint')
let ctx = canvas.getContext('2d')
```



