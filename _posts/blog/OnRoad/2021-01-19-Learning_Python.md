---
layout: post
title: Teaching Myself Python... 
categories: [Python, Learning]
description: Python自学总结
keywords: Python, 学习, 记录
---
------------------------------------------------


# 引言


从python123？下载的source.zip，文件名只有每章的编号，而且后面几章的编号和教材不一致！

## 考证

全国计算机等级考试（National Computer Rank Examination，简称NCRE）
Python 二级科目在 2018 年设立
《Python 语言程序设计 二级教程》、《高教版 Python 语言程序设计冲刺试卷》 https://python123.io/index/ncre



## 每章课后练习

## 每章自测


# 基础

### Python特点

Python 3.0 解释器内部采用面向对象方式实现，但Python语法层面却同时支持面向过程和面向对象两种编程方式???



## 搭建开发环境



## 开发工具


## 基本语法

### 语法元素

要点：Python程序包括格式框架、注释、变量、表达式、分支语句、循环语句、函数等语法元素

Python3新特性：
1.6.1，https://docs.python.org/3/whatsnew/3. 0.html

### 缩进

判断、循环、函数、类等语法形式能够通过缩进包含一批代码


### 变量命名
合法的标识符：
名字的首字符不能是数字，中间不能出现空格，大小写敏感

#### 33个保留字

assert  elif  except  finally global  lambda None  nonlocal  raise  yield

其中，as 、with 、True 、Fa!se 、None 是Python3新增的关键字。

## 字符串

两个双引号""或者单引号''括起来；
两种序号体系：正向递增序号和反向递减序号：0~L-1和 -L~-1；
区间访问方式[N:M]格式，表示字符串中从N到M（不包含M）的子字符串，可以混合使用正向和反向。

### 字符串操作


#### 字符串格式化1 "%s"%name

1.3.py：圆面积-格式化
`
print("%s 大侠，学好Python，大展拳脚！"%name[0])
"%s"%name[1:]`

#### 字符串格式化2 "{:.2f}".format(area)


 1.2.py：圆面积-格式化



#### 字符串拼接：" {}{} ".format(strl , str2)
`
print(" 世界这么大.{}想去{}看看. ".format(strl , str2))`


### 打印

#### 打印函数用法 ??? 3.6节

>>>print("The answer is" , 2*2)
>>>print("{}" , x)
>>>print("x, end=)

{}表示一个槽位置



#### 打印后不换行  end= ... print(a,end=',')

 1.4.py
`>>> a=4
>>> print(a,',')
4 ,
>>> print(a,end=',')    //   end= ???
4,>>>`

#### eval("")
把字符串解析为Python代码并执行！
TempStr="102C"
(TempStr[0:-1])

eval("hello")
eval('"hello"')  
eval(`"hello"`)  # 这一句会报错，说明Python字符串的单引号是L右侧的按键，而不是左上角数字1左边的那个按键！

>>>value=eval(input("请输入要计算的数值："))
请输入要计算的数值：1024.256
>>>print（value*2）
2048.512

支持的运算： +-*/和**


### 列表list  6.2节


#### 提取串中某个字符 %name[0], %name[1:], TempStr[-1], TempStr[0:-1]
1.3.py：

TempConvert,py
TempStr[0:-1]不包括最后一个字符！

#### 判断是否in
`if TempStr[-1] in ['F' , 'f']:`



## 其它

### 赋值

同步赋值：
x,y=y,x


### 日期时间 datetime %x %X

1.6.py

```
from datetime import datetime
print(now)
2021-01-21 19:20:20.278945
>>> now.strftime("%x")
'01/21/21'
>>> now.strftime("%X")
'19:20:20'
```


### 键盘交互-input

input()
`strl = input(" 请输入一个人的名字: ")
str2 = input(" 请输入一个国家名字: ")`


### 分支语句 4.2节

if, elif, else

### 循环语句 4.4节
while

### 函数

def con(x):



### 思考与练习

> 两个连续的printO 函数输出内容一般会分行显示，即调用printO函数后会换行结束当前行，如何让两个printO函数的输出打印在一行内?  
print(XX, end=":")


> 获得系统的日期和时间使用什么Python 函数库?    // datetime


## 画图

#### import turtle 
 1.5.py
` import turtle   // ???
>>> turtle.pensize(2)
>>> turtle.circle(10)     `

2.1.py
turtle.fd(-)
.seth




### 思考与练习

> import 保留字用来引入函数库，绘制图形可以使用什么Python 函数库?  //  turtle



# 程序设计方法学 CH8

## 神器pyinstaller库--制作程序小包裹 ???


## 计算思维

## 自顶向下、自底向上

## 面向"计算生态"的教学理念

30年前-90年，刀耕火种--官方API
20年前-00年，开源运动--专业级代码复用
10年前-10年，大量领域成果涌现
今天， 需要胶水


Python致力于开源开放，有全球最大的编程计算生态--超过10 万个各类函数库，math库有44 个函数，
利用可重用资源快速构建应用--已是主流产品开发方式。
Python-胶水语言：可以用简单的接口封装调用其它语言的函数库--各类语言之间的接口！

漫长的学习，很难产出价值程序 vs. 快速实现--AlphaGo开源了！

内置库-标准库，第三方库：库library，模块module，类class，程序包package




## 模块编程-对象.方法() 或 库.函数() 8.5节

不再探究具体算法的内部细节，而是尽可能复用现有库，探究运用库的系统方法
搭积木

### OOP方法
对象   C 一辆汽车
属性     C.color  汽车的颜色
方法   C.forward()  前进

### import
两种方式
| 引用方式 | 函数调用方式 |优缺点 |
|:--:|:--:|:--:|
| import <库名>  |  <库名>.<函数名>（<函数参数>) | 引用较多库时不易混淆|
| from<库名>import<函数名, 函数名,...,函数名> <br>from<库名>import * | <函数名>（<函数参数>)  | 更简洁，但易冲突|
当函数名冲突时，会以最近的函数定义为准  ???

### vs. 模块化设计 ???

模块化设计--自顶向下  ???

2.1.py

### IPO程序 ???

数据输入的来源和方式：
文件，网络，随机数，内部参数
控制台??? 交互界面

图灵测试???

### range() ???

整数求和：
`n = input( "输入整数N: " )
sum = 0
for i in range(int(n)):
    sum += i + 1
print("1到N求和结果", sum)`

乘法表：
`for i in range(1, 10) :
    for j in range(1, i+1) :
        print("{}*{}={:2}" .format(j , i , i*j), end=' ')
print(' ')`

计算阶乘级数：


### 数据类型和变量
list, tuple

dict, set
dictionary (字典)、tuple (元组) 和list (列表)

字符串和编码

### 缩进






### 条件判断

### 循环



### 错误、调试和测试





## 常用库和工具

### CLI

### 3D

### PIL

### gnuplot

### GUI

### Game

### FP函数式编程



## CH6

6-4-jieba.py 中文


## CH7

> Traceback (most recent call last):
>   File "D:/OneDrive/LCL_Github/Teaching/SongTian/Sources/7-9.py", line 3, in <module>
>     for line in fo:
> UnicodeDecodeError: 'gbk' codec can't decode byte 0x82 in position 8: illegal multibyte sequence
6-4.py和6-5.py也用到UTF8编码，并没有采用“import io”  ???

7-9-price2016.csv 似乎是UTF8编码
解决同时涉及编码和读写设定的文件打开方式：
> import io
> fr = io.open("7-9-price2016.csv", mode="r", encoding="utf-8")

> ls = line.line.split(",")
> AttributeError: 'str' object has no attribute 'line'
7-11.py中，修改为“ ls = line.split(",")”。


7-13-price2016.html UTF8编码，浏览器中中文乱码？！ ???

7-15-json2csv.py 生成的UTF8编码的.csv，用excel打开，中文乱码？！ ???，用notepad打开没问题！

# 专题/模块


## CH8 词云等

`import wordcloud`
需要安装

> WARNING: The script wordcloud_cli.exe is installed in 'C:\Users\Lilian\AppData\Roaming\Python\Python36\Scripts' which is not on PATH.
> Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.
> Successfully installed wordcloud-1.8.1

from scipy.misc import imread 报错，改为"from matplotlib.pyplot import imread"


## CH9 ???

from PIL import Image
import numpy as np

import numpy as np  
import matplotlib.pyplot as plt

matplotlib需要安装，"pip3 install matplotlib"命令提示要先采用
"python.exe -m pip install --upgrade pip"更新pip

但是，Win10, Python 3.6.5下更新后，用"pip3 install matplotlib"命令依然报错：ERROR: Exception:
pip install matplotlib==3.3.1 也报错
pip install matplotlib==3.2试了两次，成功

#### 9.7
plt.thetagrids(angles*180/np.pi, radar_labels,frac = 1.2)  #  报错  AttributeError: 'Text' object has no property 'frac'??? #  lines, labels = thetagrids(angles, labels=None, fmt=’%d’, frac = 1.5)

因为使用的是库的最新版本，其方法内部是不需要使用到frac，去掉即可。
https://blog.csdn.net/CNAnonymous/article/details/86896101


##  CH 爬虫

import requests
from bs4 import BeautifulSoup
import re
import json

12-2-CrawUnivRanking.py

`u=allUniv[i]
IndexError: list index out of range`
估计是没有爬到数据？  ???



# 高级特性




## DevOps


## 版本控制






## 错误、调试和测试



# 程序清单

|章节|程序|
|--:|:--|
|  | 1-1-.py Hello <br>  1-2-.py 计算圆面积 <br>    1-3-.py 提取姓或名 <br>    1-4-.py 斐波那契数列 <br>   1-5-.py turtle画圆 <br>   1-6-.py 时间日期 <br>  1-7-.py 字符串连接 <br>  1-8-.py 整数求和 <br> 1-9-.py 乘法表 <br> 1-10-.py 阶乘的级数 <br> 1-11-.py (n+1)<<1 ??? <br>  1-12-.py 5选2组合数 <br>  1-13-.py 画五角星涂色 ???<br> 1-14-.py 画24角星涂色 ???<br> |
|  | 2-1-TempConvert.py温度转换<br>  2-2-.py<br>  2-3-.py<br>  2-4-DrawPython.py 蟒蛇绘制<br>  2-5-.py<br>  2-6-.py<br> 2-AutoTraceDraw.py turtle<br>  2-data.txt<br>  2-8-RoseDraw.py<br>  PythonDraw.py<br> 
| 3.基本数据类型 | 3-DayDayUp365-1.py 天天向上的力量<br>  3-2-.py<br>  3-3-.py<br>  3-4-.py<br>  3-5-.py<br>  3-6-Week.py 星期几<br>  3-7-Cypher.py 加密<br>  3-8-TextProgress Bar.py文本进度条<br>  3-9-.py<br>  3-10-.py<br>
| 4.控制结构 | 4-1-PM2.5.py <br>  4-2-.py<br>  4-3-.py<br>  4-4-CalBMI.py 身体质量指数BMI<br>  4-5-.py<br>  4-6-CalPi.py π的计算<br>  4-7-.py 整数平方<br>  4-8-Alph.py 按序号获取表中英文字母<br>  4-9-.py<br>
| 5.复用 | 5-1-.py Happy birthday<br>  5-2-DrawSevenSegDisplay.py七段数码管绘制<br>  5-3-.py<br>  5-4-recursion.py 递归<br>  5-5-reverse.py 字符串顺序反转<br>  5-6-DrawKoch.py 科赫分形曲线<br>  5-7-.py<br>
| 6.组合数据类型 | 6-1-CalStatistics.py 统计值<br>  6-2-CalHamlet.py文本词频统计<br>  6-3-.py<br>  6-4-jieba.py 中文<br>  6-5-.py<br>  6-7-.py Python之禅<br>
| 7.格式化 | 7-1-.py  7.1.txt ???<br>  7-2-.py 打开文件逐行读取显示<br>  7-3-.py 写入文件<br>  7-4-gif.py  分解gif<br>  7-5-split.py 变色<br>  7-6-Contour.py 轮廓<br>  7-7-ImageEnhance.py 对比度<br>  7-8-DrawCharImage.py 图像的字符画绘制<br>  7-9-.py 处理.csv<br>  7-10-.py<br>  7-11-.py<br>  7-12-.py<br>  7-13-csv2html.py<br>  7-14-csv2json.py<br>  7-15-json2csv.py<br>
| 8.方法论??? | 8-1-MatchAnalysis.py体育竞技分析<br>  8-2-BatchInstall.py  pip安装脚本<br>  8-GovRptWordCloudv1T1.py<br> 8-GovRptWordCloudv1T2.py<br> 8-GovRptWordCloudv1T3.py<br> 8-GovRptWordCloudv1T4.py<br> 8-GovRptWordCloudv2T1.py<br> 8-GovRptWordCloudv2T2.py<br> 8-GovRptWordCloudv2T3.py<br> 8-GovRptWordCloudv2T4.py<br>
| 9.可视化 | 9-1-HandDrawPic.py 图像的手绘效果<br> 9-2-.py 导入matplotlib<br> 9-3-.py科学坐标图，画出小图，但plots窗口没跳出<br> 9-4-.py 成功<br> 9-5-PlotDamping.py 阻尼<br> 9-6-DrawRadar.py 成功<br> 9-7-DrawHollandRadar.py 多级雷达图<br>
|10.爬虫  | 10-1-.py baidu<br> 10-2-CrawUnivRanking.py 大学排名 【没有爬到数据???, 报错】<br> 10-3-AutoKeywordSearch.py搜索关键词自动提交【成功，但没看到结果是怎样的】<br>