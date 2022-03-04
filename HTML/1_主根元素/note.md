# 主根元素

只有一个 `<html>` 元素。

## `<html>`

表示一个 HTML 的根，也被成为就是根元素。

### 用法

```html
<html lang="zh-CN"></html>
```

### 属性

`lang` 属性，将有助于屏幕阅读技术确定要陈述的正确语言。

-   en 英文
-   zh-CN 简体中文
-   zh-Hans/zh-CHS 简体中文
-   zh-Hant/zh-CHT 繁体中文

### 注意事项

`<html>`元素只能允许一个`<head>`元素，后跟一个`<body>`元素

## 浏览器模式声明 

存在怪异模式、接近标准模式和标准模式三种模式。浏览器使用文件开头的`DOCTYPE`来决定用怪异模式处理或标准模式处理。

### 用法

```html
<!DOCTYPE html>
```

`<!DOCTYPE html>`是标准模式，也是最推荐使用的模式。

使用`document.compatMode`可以看到当前的浏览器模式。

-   `CSS1Compat`W3C 标准模式
-   `BackCompat`怪异模式
