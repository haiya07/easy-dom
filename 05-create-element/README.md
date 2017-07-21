Document 对象提供了可以创建元素节点、属性节点和文本节点的方法，方便 DOM 更新 HTML 页面中的元素。

## 创建元素节点

```javascript
element = document.createElement(tagName);
```

上述语法格式中，tagName 是参数，表示创建元素的元素名称。element 是返回值，表示创建的元素。

```javascript
var div = document.getElementById('group');
```

上述示例代码通过 createElement() 方法创建了 button 元素，并将其添加到 HTML 页面中。

> **完整示例代码请点击右边的链接:** [createElement() 方法完整示例代码](https://segmentfault.com/n/1330000010210326?token=03409d06612b86a67f0f1e550a43e731)

## 创建文本节点

```javascript
textNode = document.createTextNode(data);
```

上述语法格式中，data 是参数，包含了放在文本节点中的内容，是一个字符串。textNode 是返回值，表示创建的文本节点。

```javascript
var div = document.getElementById('group');
```

上述示例代码先通过 createElement() 方法创建了 button 元素，再通过 createTextNode() 方法创建了一个新的文本节点，并将其添加到新创建的 button 元素中。

> **完整示例代码请点击右边的链接:** [createTextNode() 方法完整示例代码](https://segmentfault.com/n/1330000010210372?token=4bdeba7f9b419ccd2f4ca5a464b09de0)

## 创建属性节点

```javascript
attributeNode = document.createAttribute(name);
```

上述语法格式中，name 是参数，属性节点的属性名称。attributeNode 是返回值，表示创建的属性节点。

> **值得注意的是:**  
> 
> 1. 创建属性节点方法只具有属性名称，没有属性值。想要设置属性值需要通过 nodeValue 属性完成。
> 2. 由于属性节点不是元素节点的子节点，不能使用添加子节点方式操作属性节点。想要添加属性节点需要通过 setAttributeNode() 方法完成。

```javascript
var div = document.getElementById('group');
```

上述示例代码先通过 createAtrribute() 方法创建了 ，再通过 createTextNode() 方法创建了一个新的文本节点，并将其添加到新创建的 button 元素中。最后，通过 createAttribute() 方法创建 class 属性节点，并设置了属性值为 button，再将该属性节点添加到新创建的 button 元素中。

> **完整示例代码请点击右边的链接:** [createAtrribute() 方法完整示例代码](https://segmentfault.com/n/1330000010210431?token=6d2d073c364591d7d908e52d140bf0d6)

---
本教程免费开源，任何人都可以免费学习、分享，甚至可以进行修改。但需要注明作者及来源，并且不能用于商业。

本教程采用[知识共享署名-非商业性使用-禁止演绎 4.0 国际许可协议](http://creativecommons.org/licenses/by-nc-nd/4.0/)进行许可。