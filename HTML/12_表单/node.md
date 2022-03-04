# 表单

非常重要的元素，用于数据交互。

## 常用元素

### `<form>`

Form 表单元素，用来提交表单。

```html
<form action="" method="get"></form>
```

用户提交数据，数据名称 + 数据值，通过每个组件的`name`属性和`value`属性分别获取。

前端验证长度和字符格式；后端也同要验证，然后对比数据库。

#### 属性

##### action

提交地址 URL。

##### method

提交方式，有`get`和`post`。

### `<input>`

inline-block 内联块级元素

#### 用法

##### 输入框

```html
<input type="text" name="username" />
```

##### 密码框

```html
<input type="password" name="password" />
```

##### 单选框

```html
<input type="radio" name="sex" value="male" />
<input type="radio" name="sex" value="female" />
```

如果不加`value`属性，默认值是`on`

##### 复选框

```html
<input type="checkbox" name="favorite" value="java" />
<input type="checkbox" name="favorite" value="rust" />
<input type="checkbox" name="favorite" value="javascript" />
```

如果不加`value`属性，默认值是`on`

##### 提交按钮

```html
<input type="submit" />
```

如果不加`value`属性，默认值是`提交`

### `<button>`

### `<select>`、`<optgroup>` 和 `<option>`

`<select>` inline-block 内联块级元素
`<option>` block 块级元素

```html
<select name="lang">
    <option value="">请选择</option>
    <option value="js">JavaScript</option>
    <option value="rust">Rust</option>
</select>
```

当`<option>`没有 value 属性时，value 值为内容。
可以通过`value`是否为空判断用户是否选择。

### `<textarea>`

inline-block 内联块级元素

```html
<textarea name="remarks"></textarea>
```

`<textarea>`的值存在于标签之间，所以不能有空格和换行。

所以获取里面的值用 value 而不是 innerHTML

### `<label>`

inline 内联元素

#### for 属性

for 属性 对应 id 值

```html
<label for="username">用户名</label>
<input id="username" type="text" name="username" />
```

### `<fieldset>` `<legend>`

表单分组，都是 block 块级元素

```html
<fieldset>
    <legend>用户登录</legend>
    <label for="loginUsername">用户名</label>
    <input id="loginUsername" type="text" name="username" />
    <label for="loginPassword">密码</label>
    <input id="loginPassword" type="password" name="password" />
</fieldset>
```

### 注意事项

placeholder 可以用 js 模拟实现更好的效果。

readonly 只读属性，不可输入，表单提交时，正常提交。

disable 不可用属性，不可输入，表单提交时，数据不提交。

## 不常用元素

### `<datalist>` `<option>`

### `<meter>`

### `<progress>`

### `<output>`
