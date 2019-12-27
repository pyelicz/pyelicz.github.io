---
layout: raw
permalink: doc/readme/zh.html
mathjax: true
---

# 欢迎使用AceMark

AceMark 致力于打造一款易用、专业的 Markdown 工具。


## 什么是 Markdown?

Markdown 是一种轻量级的标记语言。它允许人们使用易读易写的纯文本格式编写文档，并支持图片、图表、数学公式等，然后转换成有效的 HTML 文档。AceMark 采用 [GitHub Flavored Markdown](https://github.github.com/gfm/) 语法（简称 GFM），并支持一些扩展语法。下面我们来熟悉下 AceMark 的常用标记说明。 

为了方便导航，我们在这里插入目录。插入目录的语法如下：

```
[toc]
```

这是输出的目录：

* TOC 
{:toc}

## 标题

AceMark 最高支持六级标题，一级标题在行首使用一个`#`，二级标题使用两个`##`，以此类推。如下：

```
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
```

## 样式

+ `**粗体**`用于表示**粗体**
+ `*斜体*`用于表示*斜体*
+ `~~删除线~~`用于表示~~删除线~~

## 脚注

我们可以在这里插入一个脚注 [^footnote]。

[^footnote]: 这是脚注内容。

## 引用

    > 这是一个引用
    
效果：
> 这是一个引用


## 链接

```
[链接标题](http://www.acemark.net)
```
输出：[链接标题](http://www.acemark.net)

如果想要显示一张网络图片，方式和普通链接类似，但需要在前面加一个`!`符号。
```
![图片标题](http://www.acemark.net/img/icon.jpg)
```
![图片标题](http://www.acemark.net/img/icon.jpg)


## 表格

通过下面的标记，就可以输出一份表格

    | 标题1 | 标题2 | 标题3 |
    |------|-------|------|
    | 内容1 | 内容2 | 内容3 |
    | 内容4 | 内容5 | 内容6 |
    
输出表格：

| 标题1 | 标题2 | 标题3 |
|------|-------|------|
| 内容1 | 内容2 | 内容3 |
| 内容4 | 内容5 | 内容6 |


## 列表

### 有序列表


```
1. 第一项
2. 第二项
```

输出结果：

1. 第一项
2. 第二项

### 无序列表

`+`、`*`、`-`都可以用来标识无序列表项。例如：

```
+ 项目1
* 项目2
- 项目3
```

输出结果：

+ 项目1
* 项目2
- 项目3


### TODO 标记

```
- [ ] 未完成
- [X] 已完成
```

输出结果：

- [ ] 未完成
- [X] 已完成

## 代码
AceMark 支持几十种代码高亮。例如：

Lua

    ```lua
    local function Fibonacci(n)
        local function doFibonacci(n, ret1, ret2)
            if (n <= 1) then
                return ret2
            end
            return doFibonacci(n - 1, ret2, ret1 + ret2)
        end
        return doFibonacci(n, 1, 1)
    end
    ```
    
输出：

```lua
local function Fibonacci(n)
    local function doFibonacci(n, ret1, ret2)
        if (n <= 1) then
            return ret2
        end
        return doFibonacci(n - 1, ret2, ret1 + ret2)
    end
    return doFibonacci(n, 1, 1)
end
```

Go

    ```go
    func Fibonacci(n int) int {
        if n <= 1 {
            return n
        }
        return Fibonacci(n-1) + Fibonacci(n-2)
    }
    ```
    
输出：

```go
func Fibonacci(n int) int {
    if n <= 1 {
        return n
    }
    return Fibonacci(n-1) + Fibonacci(n-2)
}
```

JavaScript

    ```javascript
    function Fibonacci(num) {
        if (num <= 1) return 1;
        return Fibonacci(num - 1) + Fibonacci(num - 2);
    }
    ```

输出：

```javascript
function Fibonacci(num) {
    if (num <= 1) return 1;
    return Fibonacci(num - 1) + Fibonacci(num - 2);
}
```
## 数学公式

AceMark 支持 LaTeX 语法的数学公式。例如

```
$$
f(x) = a x^2 + b x + c
$$
```

会输出一个抛物线方程

$$
f(x) = a x^2 + b x + c
$$

而下面这个表达式
```
$$
F(\omega)=\int_{-\infty}^{+\infty} {f(t)e^{-i\omega t}dt}
$$
```

会输出一个傅里叶变换积分方程

$$
F(\omega)=\int_{-\infty}^{+\infty} {f(t)e^{-i\omega t}dt}
$$

要输出矩阵也很简单，只需要

```
$$
\begin{bmatrix}
1 & x & x^2 \\
1 & y & y^2 \\
1 & z & z^2 \\
\end{bmatrix}
$$
```

便可得到想要的效果

$$
\begin{bmatrix}
1 & x & x^2 \\
1 & y & y^2 \\
1 & z & z^2 \\
\end{bmatrix}
$$

公式也可以显示在行内。例如 `$f(x)=kx+b$` 就会输出 $f(x)=kx+b$，这是一个显示在行内的直线方程。

