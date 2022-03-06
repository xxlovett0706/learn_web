# CSS

cascading style sheets 层叠样式表

## 用法

```css
选择器 {
    属性名: 属性值;
    属性名: 属性值;
}
```

### 内联样式

```html
<div style="width: 100px; height: 100px;"></div>
```

### 内部样式表

```html
<style type="text/css">
    div {
        width: 100px;
        height: 100px;
    }
</style>
```

type 属性可不写

`<style>`元素写在 `<head>`里最后面。

### 外部样式表

```html
<link rel="stylesheet" type="text/css" href="index.css" />
```

rel 属性必写

type 属性可不写
