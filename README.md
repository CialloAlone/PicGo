# Markdown语法概述

Markdown是一种方便记忆、书写的纯文本标记语言，用户可以使用这些标记符号以最小的输入代价生成极富表现力的文档：譬如您正在阅读的这份文档。它使用简单的符号标记不同的标题，分割不同的段落，**粗体** 或者 *斜体* 某些文字

## 1. 斜体和粗体

使用 * 和 ** 表示斜体和粗体。

示例：

这是 *斜体*，这是 **粗体**。

## 2. 分级标题

在行首加井号表示不同级别的标题 (H1-H6)，例如：# H1, ## H2, ### H3，#### H4。

## 3. 外链接

使用 \[描述](链接地址) 为文字增加外链接。

示例：

这是去往 [百度网盘](pan.baidu.com) 的链接。

## 4. 无序列表

使用 *，+，- 表示无序列表。

示例：

+ 无序列表项 一
+ 无序列表项 二
+ 无序列表项 三

## 5. 有序列表

使用数字和点表示有序列表。

示例：

1. 有序列表项 一
2. 有序列表项 二
3. 有序列表项 三

## 6. 文字引用

使用 > 表示文字引用。

示例：

>野火烧不尽，春风吹又生。

## 7. 行内代码块


使用 \`代码\` 表示行内代码块。

示例：

让我们聊聊 `html`。

## 8.代码块

使用 四个缩进空格 表示代码块。

示例：

	这是一个代码块，此行左侧有四个不可见的空格。

## 9. 插入图片

使用 \!\[描述](图片链接地址) 插入图像。

示例：![弱气角色友崎君Lv.9](https://img.rruu.net/image/6012f6f279fea)

## 10. 删除线


使用 ~~ 表示删除线。

~~这是一段错误的文本。~~

## 11. 注脚


使用 \^[keyword] 表示注脚。

这是一个注脚^[这里写注释]的样例。

这是第二个注脚^[这里写注释]的样例。

## 12. KaTeX 公式

$ 表示行内公式：

质能守恒方程可以用一个很简洁的方程式 $E=mc^2$ 来表达。

\$$ 表示整行公式:

$$ \sum_{i=1}^na_i=0 $$

$$
f(x_1,x_x,\ldots,x_n)=x_1^2+x_2^2+\cdots+x_n^2
$$

$$ x={-b\pm\sqrt{b^2-4ac}\over2a}. $$

## 13. 加强的代码块

支持四十一种编程语言的语法高亮的显示，行号显示。

非代码示例：

	$ sudo apt-get install vim-gnome
    
Python 示例：

```py
@requires_authorization
def somefunc(param1='', param2=0):
    '''A docstring'''
    if param1 > param2: # interesting
        print 'Greater'
    return (param2 - param1 + 1) or None

class SomeClass:
    pass

>>> message = '''interpreter
... prompt'''
```

JavaScript 示例：
```js
/**
* nth element in the fibonacci series.
* @param n >= 0
* @return the nth element, >= 0.
*/
function fib(n) {
  var a = 1, b = 1;
  var tmp;
  while (--n >= 0) {
    tmp = a;
    a += b;
    b = tmp;
  }
  return a;
}

document.write(fib(10));
```

## 14. HTML标签

软件支持在 Markdown 语法中嵌套 Html 标签，譬如，你可以用 Html 写一个纵跨两行的表格：

```html
<table>
    <tr>
        <th rowspan="2">值班人员</th>
        <th>星期一</th>
        <th>星期二</th>
        <th>星期三</th>
    </tr>
    <tr>
        <td>李强</td>
        <td>张明</td>
        <td>王平</td>
    </tr>
</table>
```

<table>
    <tr>
        <th rowspan="2">值班人员</th>
        <th>星期一</th>
        <th>星期二</th>
        <th>星期三</th>
    </tr>
    <tr>
        <td>李强</td>
        <td>张明</td>
        <td>王平</td>
    </tr>
</table>

## 15. 