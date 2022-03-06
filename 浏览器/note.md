# 浏览器

## 组成部分

shell + 内核（渲染引擎和 JS 引擎）

### 种类和内核

Chrome webkit/blink
Safari webkit
Edge
Firefox gecko
IE trident
Opera presto 已被 360 和昆仑万维收购

## 浏览器

首先下载 HTML 文件，解析形成 DOM tree，与此同时开辟一个线程下载 CSS 文件，解析后形成 CSS rule tree，两者共同构成 render tree。

回流 reflow 当 render tree 中的一部分（或全部）因为元素的规模尺寸、布局或隐藏等改变而需要重新构建。

重绘 repaint 当 render tree 中的一些元素需要更新属性，而这些属性只是影响元素的外观、风格，而不会影响布局。

区别： 回流必定重绘，重回不一定回流。
