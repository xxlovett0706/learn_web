# 走进前端之『HTML』篇










## Address 标签

表示其中的 HTML 提供了某个人或某个组织（等等）的联系信息。

```html
<address>
    <a href="mailto:jim@rock.com">jim@rock.com</a><br />
    <a href="tel:+13115552368">(311) 555-2368</a>
</address>
```

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


## sup sub 标签

inline 内联元素

sup superscripted

sub subscripted



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