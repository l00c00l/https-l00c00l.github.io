---
​---
layout: post
title:  github上怎样搞定数学公式？-中文版
categories: [工具, 效率]
description: Typora能自动显示公式，什么时候github会支持呢
keywords: markdown, 公式，输入，Latex
​---
---


标记支持内联HTML。内联HTML既可以用于快速简单的内联公式，也可以用于更复杂的外部工具呈现。
快速简单的内联
对于快速而简单的内联项，请使用HTML与号和实体代码。将此思想与标记中的下标文本相结合的一个示例是：hθ（x）=θox+θ1x，代码如下。
h<sub>&amp;theta；</sub>（x）=&amp;theta；<sub>o</sub>x+&amp;theta；<sub>1</sub>x
常见数学符号的HTML符号和实体代码可以在这里找到。这里是希腊字母的代码。
虽然这种方法有局限性，但它实际上适用于所有标记，不需要任何外部库。
使用乳胶和编解码器的复杂可伸缩内联渲染
如果需要更多，请使用外部乳胶渲染器（如CodeCogs）。使用CodeCogs编辑器创建公式。选择svg进行渲染，选择HTML进行嵌入代码。Svg在调整大小时表现良好。HTML允许在查看源代码时轻松读取LaTeX。从页面底部复制嵌入代码并将其粘贴到标记中。
<img src=“https://latex.codecogs.com/svg.latex？\大&amp;space；x=\frac{-b\pm\sqrt{b^2-4ac}{2a}“title=”\Large x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}“/>
这是这个答案和这个答案的结合。
GitHub只支持使用上述原始html语法为我的可读乳胶工作了一些次。如果上述方法对您不起作用，则另一个选项是选择URL编码呈现，并使用该输出手动创建如下链接：
![\Large x=\frac{-b\pm\sqrt{b^2-4ac}{2a}]（https://latex.codecogs.com/svg.latex？x%3D%5crac%7B-b%5Cpm%5Csqrt%7Bb%5E2-4ac%7D%7D%7B2a%7D）
这将在alt图像文本中手动合并乳胶，并使用编码的URL在GitHub上进行呈现。
多行渲染
如果需要多行渲染，请查看此答案。


> --------------------------------------------------------------

Markdown supports inline HTML. Inline HTML can be used for both quick and simple inline equations and, with and external tool, more complex rendering.
Quick and Simple Inline
For quick and simple inline items use HTML ampersand entity codes. An example that combines this idea with subscript text in markdown is: hθ(x) = θo x + θ1x, the code for which follows.
    h<sub>&theta;</sub>(x) = &theta;<sub>o</sub> x + &theta;<sub>1</sub>x
HTML ampersand entity codes for common math symbols can be found here. Codes for Greek letters here.
While this approach has limitations it works in practically all markdown and does not require any external libraries.
Complex Scalable Inline Rendering with LaTeX and Codecogs
If your needs are greater use an external LaTeX renderer like CodeCogs. Create an equation with CodeCogs editor. Choose svg for rendering and HTML for the embed code. Svg renders well on resize. HTML allows LaTeX to be easily read when you are looking at the source. Copy the embed code from the bottom of the page and paste it into your markdown.
<img src="https://latex.codecogs.com/svg.latex?\Large&space;x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}" title="\Large x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}" />
This combines this answer and this answer.
GitHub support only somtimes worked using the above raw html syntax for readable LaTeX for me. If the above does not work for you another option is to instead choose URL Encoded rendering and use that output to manually create a link like:
![\Large x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}](https://latex.codecogs.com/svg.latex?x%3D%5Cfrac%7B-b%5Cpm%5Csqrt%7Bb%5E2-4ac%7D%7D%7B2a%7D)
This manually incorporates LaTex in the alt image text and uses an encoded URL for rendering on GitHub.
Multi-line Rendering
If you need multi-line rendering check out this answer.
shareedit
edited Apr 1 '19 at 16:40
answered Dec 13 '17 at 17:17

SpeedCoder5
3,38244 gold badges1818 silver badges2525 bronze badges
• 1
this worked great. I had to convert a jupyter notebook (.ipynb) to .md and the equations were essentially multiline latex code. – Marc Maxmeister Jun 17 '19 at 18:21
• 1
works great! and is SVG 💯 – HerberthObregon Mar 13 at 20:22 

来自 <https://stackoverflow.com/questions/11256433/how-to-show-math-equations-in-general-githubs-markdownnot-githubs-blog> 



