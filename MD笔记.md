#MarkDown笔记

##标题设置（让字体变大，和word的标题意思一样）
在Markdown当中设置标题，有两种方式：
第一种：通过在文字下方添加“=”和“-”，他们分别表示一级标题和二级标题。
第二种：在文字开头加上 “#”，通过“#”数量表示几级标题。（一共只有1~6级标题，1级标题字体最大）

##粗体
将需要设置为粗体的文字两端使用2个“*”或者“_”夹起来

##斜体
将需要设置为斜体的文字两端使用1个“*”或者“_”夹起来

##块注释（blockquote）
通过在文字开头添加“>”表示块注释。（当>和文字之间添加五个blank时，块注释的文字会有变化。）
##居中
> 可以在Git上居中的方法


文字居中：
<p align="center"> 文字居中</p>

图片居中：
<div align="center">
 	  <img src="图片居中" >
</div>

> 在本地编辑器居中的方法

文字居中：
<center> 文字</center>

图片居中：
<center>
![image]()
</center>

##链接

> 链接

页内链接：[链接名字](#链接的ID或网址)

页间链接到指定位置：[链接名字](页面目录/#ID)

##图片

![image](图片路径)


##列表

1. 有序列表：使用数字后面跟上句号。（还要有空格）
2. 无序列表：在文字开头添加(*, +, and -)实现无序列表。但是要注意在(*, +, and -)和文字之间需要添加空格。（建议：一个文档中只是用一种无序列表的表示方式）