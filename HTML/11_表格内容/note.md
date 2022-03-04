# 表格内容

## 常用元素

`<table>`、`<caption>`、`<tr>`、`<th>`、`<td>`、`<thead>`、`<tbody>`和`<tfoot>`

```html
<table>
    <caption>
        表格标题
    </caption>
    <thead>
        <tr>
            <th>ID</th>
            <th>姓名</th>
            <th>地区</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>1</td>
            <td>MasK</td>
            <td rowspan="2">冰岛</td>
        </tr>
        <tr>
            <td>2</td>
            <td>TT</td>
        </tr>
    </tbody>
    <tfoot>
        <tr>
            <td colspan="3">页脚</td>
        </tr>
    </tfoot>
</table>
```

### 各个元素 display 属性的值

`<table>` table
`<caption>` table-caption
`<tr>` table-row
`<th>` table-cell
`<td>` table-cell
`<thead>` table-header-group
`<tbody>` table-row-group
`<tfoot>` table-footer-group

### 合并单元格

`<td>`设置 rowspan 和 colspan 属性可以合并单元格。

## 不常用元素

`<colgroup>` 和`<col>`

```html
<colgroup>
    <col class="red" span="1" />
    <col class="green" span="2" />
</colgroup>
```

用来定义表格中的列

## 注意事项

加载顺序：`<thead>` -> `<tfoot>` -> `<tbody>`

设置`<thead>`和`<tfoot>`可以避免`<tbody>`内容过多，优先加载页眉和页脚内容
