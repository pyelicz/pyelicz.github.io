---
layout: raw
permalink: zh_cn/tutorial.html
mathjax: true
---

# 欢迎使用AceMark
AceMark 致力于打造一款易用、专业的 Markdown 编辑工具。

## 什么是 Markdown?
Markdown 是一种轻量级的标记语言。它允许人们使用易读易写的纯文本格式编写文档，并支持图片、图表、数学公式等，然后转换成有效的 HTML 文档。
AceMark 采用[GitHub Flavored Markdown](https://github.github.com/gfm/)语法（简称 GFM），并支持一些扩展语法。下面我们来熟悉下 AceMark 的常用标记说明。 

## 标题
AceMark 最高支持六级标题，一级标题在行首使用一个`#`，二级标题使用两个`##`，以此类推。如下：

	# 一级标题
	## 二级标题
	### 三级标题
	#### 四级标题
	##### 五级标题
	###### 六级标题

以下是展示效果：
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题

------

## 样式
+ `**粗体**`用于表示**粗体**
+ `*斜体*`用于表示*斜体*
+ `~~删除线~~`用于表示~~删除线~~

## 引用
	> 这是一个引用
	
效果：
> 这是一个引用

## 数学公式
这是一个抛物线方程

$$
f(x) = a x^2 + b x + c
$$

这是一个积分方程

$$
F(\omega)=\int_{-\infty}^{+\infty} {f(t)e^{-i\omega t}dt}
$$


矩阵

$$
\begin{bmatrix}
1 & x & x^2 \\
1 & y & y^2 \\
1 & z & z^2 \\
\end{bmatrix}
$$