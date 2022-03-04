# 文档元数据

元数据通常含有页面信息，如页面样式、脚本及数据。

## `<head>`

`<head>`元素用来包裹不同元数据,本身并没有

`<head>`元素里包含`<title>`、`<meta>`、`<link>`、`<style>`、`<script>`、`<noscript>`、`<base>`和`<command>`8 种元素，至少包含`<title>`元素。

### 用法

```html
<html>
    <head>
        <title>标题</title>
    </head>
</html>
```

## `<title>`

网页标题，`<head>`元素必须包含的一个元素。

### 用法

```html
<title>标题</title>
```

## `<meta>`

表示那些**不能**由其它 HTML 元相关（meta-related）元素（`<base>`、`<link>`, `<script>`、`<style>` 或 `<title>`）之一表示的任何元数据信息。

### 用法

```html
<meta charset="UTF-8" />
<meta http-equiv="content-type" content="text/html; charset=utf-8" />
<meta name="keywords" content="关键字" />
```

### 属性

#### charset

```html
<meta charset="UTF-8" />
```

来告诉浏览器该用哪种字符集解析。

    -   GB2312 中国信息处理国家标准码 简体中文
    -   GBK 汉字扩展规范 扩大汉字收录，增加了繁体中文和藏蒙维等少数民族的文字
    -   UTF-8 Unicode 万国码

#### http-equiv 和 content

```html
<meta http-equiv="content-security-policy" content="default-src 'self'" />
<meta http-equiv="content-type" content="text/html; charset=utf-8" />
<meta
    http-equiv="default-style"
    content="the document's preferred stylesheet"
/>
<meta http-equiv="x-ua-compatible" content="IE=edge" />
<meta http-equiv="refresh" content="3; url=https://www.baidu.com" />
```

等同于 设置 HTTP 头部信息

-   content-security-policy 设置允许的内容策略
-   content-type 如果要设置这个属性，则必须是 text/html; charset=utf-8，推荐用 meta charset 代替
-   default-style 设置默认 CSS 样式表（暂时未使用过）
-   x-ua-compatible 如果指定，则 content 属性必须具有值 "IE=edge"。
-   refresh 重新加载 单位为秒，后可根 url`300; url=https://www.baidu.com`

#### name 和 content

`<meta>`元素可用于提供 key-value 对形式的文档元数据，`name`属性为元数据条目提供名称，而`content`属性提供值。

```html
<meta name="author" content="MasK" />
<meta name="keywords" content="关键字" />
<meta name="description" content="描述" />
<meta name="generator" content="VSCode" />
<meta name="referrer" content="no-referrer-when-downgrade" />
```

##### HTML 规范中定义的标准元数据名称

-   author 作者
-   keywords 网站关键字
-   description 网站描述
-   generator 生成此网页的软件标识
-   referrer 设置当前文档发出 HTTP Referer 请求头 默认 no-rederrer-when-downgrade

## `<link>`

```html
<link rel="stylesheet" href="style/main.css" />
```

## `<style>`

```html
<style>
    .main {
        background-color: #999;
    }
</style>
```

## `<base>`

```html
<base href="https://www.example.com" />
```

定义文档所有相对 URL 的根 URL。
