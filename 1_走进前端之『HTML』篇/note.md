# 走进前端之『HTML』篇

## head 三大关键标签

`title` `keywords` 和 `description`

```html
<html>
    <head>
        <title></title>
        <meta name="keywords" content="" />
        <meta name="description" content="" />
    </head>
    <body></body>
</html>
```

`title` 标题
主页： 网站名称 + 主要的关键字/关键字的描述
详情页：详情名称 + 网站名称 + 简介
列表页：分类名称 + 关键字 + 网站名称
文章页：标题 + 分类 + 网站名称

`keywords` 关键字
100 个字符，用`,`隔开，网站名称 + 分类信息 + 网站名称，越靠前权重越高。

`description` 描述信息
80-120 个汉字，综合 `title` + `keywords`的简单描述

### 搜索引擎认知的优先级

`title` > `description` > `keywords`

## html 语言设置

```html
<html lang="zh-CN"></html>
```

en 英文
zh-CN 简体中文
zh-Hans zh-CHS 简体中文
zh-Hant zh-CHT 繁体中文

## 编码字符集

```html
<html lang="zh-CN">
    <head>
        <meta charset="UTF-8" />
    </head>
</html>
```

GB2312 中国信息处理国家标准码 简体中文
GBK 汉字扩展规范 扩大汉字收录，增加了繁体中文和藏蒙维等少数民族的文字
UTF-8 Unicode 万国码

## html 声明

`<!DOCTYPE html>`

```javascript
console.log(document.compatMode);
```

CSS1Compat W3C 标准模式
BackCompat 怪异模式

## Heading 标签

```html
<h1>h1</h1>
<h2>h2</h2>
<h3>h3</h3>
<h4>h4</h4>
<h5>h5</h5>
<h6>h6</h6>
```

浏览器默认字体大小 16px

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
