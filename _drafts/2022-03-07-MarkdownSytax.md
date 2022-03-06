---
layout: post
title:  MarkDown语法
date:   2022-03-07 00:20:00 +0800
categories: 杂项
tag: 教程
---


MarkDown是一种轻量级标记语言，可以将格式设置元素添加到纯文本中。可以用来创建网站，笔记，书籍等。  

Markdown的语法比较简单，而且每个处理器对于语法的支持也不太相同，这里只纪录Markdown基本都支持的通用语法。

## Markdown基本语法  

### 标题
标题以`#`号开头，几级标题就用几个`#`号，后接一个空格然后是标题内容。如：  

> `# 一级标题`  
> `## 二级标题`  
> `### 三级标题`  
> `#### 四级标题`  
> `##### 五级标题`  
> `###### 六级标题`  

展示结果如下图：  

![标题效果图]({{site.baseurl}}/styles/images/MarkdownSytax/head.png)

#### 标题替代语法
可以在标题下方行上添加任意数量的`=`来代表一级标题，或`-`代表二级标题。

> `一级标题`  
> `======`  
>
> `二级标题`  
> `------`  

效果如下图：  

![标题效果图2]({{site.baseurl}}/styles/images/MarkdownSytax/head2.png)


### 段落

可以使用空行来分隔段落，如：

> `This is paragraph1`  
>  
> `This is paragraph2`  

效果如下图：  

![段落效果图]({{site.baseurl}}/styles/images/MarkdownSytax/paragraph.png)

### 换行

在一行后添加两个或多个空格，然后回车，可以换行，如：

> `这是第一行<空格><空格>`  
> `这是第二行<空格><空格>`  
> `这是第三行<空格><空格>`  

效果如下图：  

![换行效果图]({{site.baseurl}}/styles/images/MarkdownSytax/line.png)

### 着重格式

着重格式主要是粗体和斜体，斜体可以在文字前后各添加一个`*`或一个`_`号来表示，粗体可以在文字前后各添加两个`*`或两个`_`，粗体斜体可以在文字前后各添加三个符号来表示。如：  

> `*斜体*, _斜体_`  
> `**粗体**, __粗体__`  
> `***粗体且斜体***, ___粗体且斜体___`  

效果如下图：  

![着重格式效果图]({{site.baseurl}}/styles/images/MarkdownSytax/bolditaly.png)

### 区块引用

在段落前添加一个大于号(>),可以创建区块引用  

> `> 区块引用`  

效果如下图：

![区块效果图]({{site.baseurl}}/styles/images/MarkdownSytax/blockquote.png)

区块引用中可以嵌套多种标记：  
1. 多级区块  
    多个`>`可以嵌套表示多级区块，如：  
    
    > `> 一层嵌套`  
    > `>> 二层嵌套`  
    > `>>> 三层嵌套`  
    
    效果如下图：
    
    ![区块效果图1]({{site.baseurl}}/styles/images/MarkdownSytax/blockquote1.png)
    
2. 区块引用中嵌套段落  
    区块引用中如果嵌套了段落，那么段落间的空行中也要添加大于号(>)，如：
    
    > `> 这是区块引用段落一`  
    > `>`  
    > `> 这是区块引用段落二`  
    
    效果如下图：
    
    ![区块效果图2]({{site.baseurl}}/styles/images/MarkdownSytax/blockquote2.png)

3. 区块引用中嵌套列表  
    区块引用中也可以嵌套列表（列表定义方式见[列表](#ListHead)），如：
    
    > `> 1. 有序列表1`  
    > `> 2. 有序列表2`  
    > `> 3. 有序列表3`  
    >  
    > `> - 无序列表1`  
    > `> - 无序列表2`  
    > `> - 无序列表3`  
    
    效果如下图：  
    
    ![区块效果图3]({{site.baseurl}}/styles/images/MarkdownSytax/blockquote3.png)

### 列表    {#ListHead}

列表分为有序列表和无序列表：  

#### 有序列表

有序列表直接在列表每一项添加 `数字. `， 如：

> `1. 有序列表1`  
> `2. 有序列表2`  
> `3. 有序列表3`  

效果如下图：

![有序列表效果图]({{site.baseurl}}/styles/images/MarkdownSytax/list.png)

#### 无序列表

无序列表可以在列表每一项添加`+`或`-`或`*`，如

> `+ 无序列表+1`  
> `+ 无序列表+2`  
> `+ 无序列表+3`  
>
> `- 无序列表-1`  
> `- 无序列表-2`  
> `- 无序列表-3`  
> 
> `* 无序列表*1`  
> `* 无序列表*2`  
> `* 无序列表*3`  
 
效果如下图：

![无序列表效果图]({{site.baseurl}}/styles/images/MarkdownSytax/list2.png)

### 代码

用反引号 ｀ 把代码字段包含起来可以表示代码， 如：  

> \`std::cout << "hello world" << std::endl;`

效果如下图：

![代码效果图]({{site.baseurl}}/styles/images/MarkdownSytax/code1.png)


### 水平线

一行上使用三个`*`或`-`或`_`可以表示水平线  

> `***`  
> `---`  
> `___`  


三个效果相同，如下图：

![水平线效果图]({{site.baseurl}}/styles/images/MarkdownSytax/horizontalline.png)


### 超链接

超链接使用`[]`把链接文字包含起来，后面接`()`里是链接地址，如：  

我输入以下文字：
> `[这里是我的网站链接](https://snownight22.github.io/TTworksBlog/)`

效果如下面，点击文字可以链接到百度  
[这里是我的网站链接](https://snownight22.github.io/TTworksBlog/)

#### 给链接添加标题

在`()`内地址后添加一个空格，后跟双引号`“`括起来的文字，这些文字代表链接标题。

> `[这里是我的网站链接](https://snownight22.github.io/TTworksBlog/ "链接添加标题")`

效果如下面，鼠标放在文字上面可以显示标题  
[这里是我的网站链接](https://snownight22.github.io/TTworksBlog/ "链接添加标题")

#### 格式化链接

可以给链接添加格式，即粗体或斜体，在`[`前面和`)`后面添加表示粗体或斜体的两个或一个`*`， 就可以将链接格式化：

> `***[这里是我的网站链接](https://snownight22.github.io/TTworksBlog/)***`

效果：  
***[这里是我的网站链接](https://snownight22.github.io/TTworksBlog/)***

#### 网址和邮箱

网址和邮箱可以添加`<>`，直接转换为链接，如：

> `<https://snownight22.github.io/TTworksBlog/>`
> `<s_peach@163.com>`

效果：

<https://snownight22.github.io/TTworksBlog/>  
<s_peach@163.com>  

### 图片

图片同链接方式有点类似，只是在链接前加`!`，如：

> `![图片标题](图片地址)`  

效果：

![示例图片]({{site.baseurl}}/styles/images/MarkdownSytax/example.jpeg)

还可以给图片添加链接， 如：

> `[![图片标题](图片地址)](链接地址)`

效果：

[![示例链接图片]({{site.baseurl}}/styles/images/MarkdownSytax/example.jpeg)](https://snownight22.github.io/TTworksBlog/)


上面写完已是深夜，后续再添加markdown拓展语法  
## MarkDown拓展语法




