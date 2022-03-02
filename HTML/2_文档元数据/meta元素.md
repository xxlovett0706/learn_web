# `<meta>`

meta 元素表示那些**不能**由其它 HTML 元相关（meta-related）元素（`<base>`、`<link>`, `<script>`、`<style>` 或 `<title>`）之一表示的任何元数据信息。

## 用法

```html
<meta charset="UTF-8" />
<meta http-equiv="x-ua-compatible" content="IE=edge" />
<!-- HTML 规范中定义的标准元数据名称 -->
<meta name="author" content="MasK" />
<meta name="keywords" content="关键字" />
<meta name="description" content="描述" />
<meta name="generator" content="VSCode" />
<meta name="referrer" content="no-referrer-when-downgrade" />
```

## 属性

### charset

    来告诉浏览器该用哪种字符集解析。

    -   GB2312 中国信息处理国家标准码 简体中文
    -   GBK 汉字扩展规范 扩大汉字收录，增加了繁体中文和藏蒙维等少数民族的文字
    -   UTF-8 Unicode 万国码

### name 和 content

`<meta>`元素可用于提供 key-value 对形式的文档元数据，`name`属性为元数据条目提供名称，而`content`属性提供值。

#### HTML 规范中定义的标准元数据名称

- author 作者
- keywords 网站关键字
- description 网站描述
- generator 生成此网页的软件标识符
- referrer 设置
