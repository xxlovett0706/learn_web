# 走进前端之『HTML』篇

## Heading 标签

```html
<h1>h1</h1>
<h2>h2</h2>
<h3>h3</h3>
<h4>h4</h4>
<h5>h5</h5>
<h6>h6</h6>
```

特点：

1. 粗体
2. 独占一行
3. 大小不一致
4. 有上下 margin，em 单位
5. 字体大小为 em 单位

## Paragraph 标签

```html
<p>段落</p>
```

特点：

1. 独占一行 2.有上下 margin，1em 单位

### 如何做缩进

```html
<p style="text-indent: 2em;">段落</p>
```

## Strong 标签

表示内容强烈的重要性，`<b></b>`标签仅只是粗体样式。

```html
<strong>我是Strong标签</strong>
```

## Emphasize 标签

用来改变一个句子的意思

```html
我<em>喜欢</em>胡萝卜
```

```html
我喜欢<em>胡萝卜</em>
```

## Italic 标签

用于表现因某些原因需要区分普通文本的一系列文本。

但目前更多用于图标

```html
<i class="icon icon-list"></i>
```

## Delete 和 Insert 标签

表示一些被从文档中删除的文字内容。

```html
<del>我是del标签</del>
```

定义已经被插入文档中的文本。

```html
<ins>我是ins标签</ins>
```

## Address 标签

表示其中的 HTML 提供了某个人或某个组织（等等）的联系信息。

```html
<address>
    <a href="mailto:jim@rock.com">jim@rock.com</a><br />
    <a href="tel:+13115552368">(311) 555-2368</a>
</address>
```

## Division 标签

容器，也叫盒子，那么一定有宽和高

注意点：

1. 浏览器认识英文，当超过宽度根据空格换行。不认识中文，当超过宽度直接换行。
2. 浏览器合并多个空格（文本分隔符）

## html 实体字符

`<`用`&lt;`
`>`用`&gt;`
空格 用 `&nbsp;`

## Image 标签

```html
<img src="" alt="" />
```

`src` 是 source 缩写
`alt` 当图片失败时显示图片的主题
`title` 可选，当鼠标移动上时显示图片的主题

## inline 内联元素

不独占一行，无法定义宽高。

strong em ins

## block 块级元素

独占一行，可以定义宽高

h1 p div

## inline-block 内联块级元素

不独占一行，可以定义宽高

img

## Anchor 锚点标签

hypertext reference

1. 超链接
2. 打电话
3. 发邮件
4. 锚点
5. 协议限定符

```html
<a href="javascript:;"></a>
```

## 标签嵌套

内联元素可以嵌套内联元素

块级元素可以嵌套任何元素

p 标签不能嵌套 div 标签
a 标签不能嵌套 a 标签

## sup sub 标签

inline 内联元素

sup superscripted

sub subscripted

## span

## ol ul li

order list

type 属性
start 属性必须是数字
reversed 倒叙

unorder list

type disc square circle

都是块级元素

## dl dt dd

definition list 定义列表

```html
<dl>
    <dt>Firefox</dt>
    <dd>
        A free, open source, cross-platform, graphical web browser developed by
        the Mozilla Corporation and hundreds of volunteers.
    </dd>

    <!-- other terms and definitions -->
</dl>
```

## table

```html
<table border="1">
    <caption>
        VIP班级学生联络表
    </caption>
    <tr>
        <th>ID</th>
        <th>姓名</th>
        <th>年龄</th>
        <th>电话号码</th>
    </tr>
    <tr>
        <td>1</td>
        <td>MasK</td>
        <td>28</td>
        <td>18097331234</td>
    </tr>
</table>
```

border 属性
cellpadding 单元格内边距
cellspacing 单元格外边距

colspan 列合并
rowspan 行合并

align="left center right" 并不推荐使用

th 默认 left

加载顺序
thead -> tfoot -> tbody

## frameset 废弃

```html
<frameset rows="10%, 90%">
    <frame src="top.html" />
    <frameset cols="20%, 80%">
        <frame src="left.html" />
        <frame name="mainFrame" src="main.html" />
    </frameset>
</frameset>
```

缺点：1. 搜索引擎不友好 2. 数据交互很差 3. 请求过多 4. 不能写 body

## iframe

内联框架

内联块级元素

缺点：
1. 搜索引擎不友好
2. 滚动条
3. 数据交互很差

属性
freameborder
scrolling yes no auto