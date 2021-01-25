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


#### 1.2.py：圆面积-格式化

`"{:.2f}".format(area)`

#### 1.3.py：圆面积-格式化
`
print("%s 大侠，学好Python，大展拳脚！"%name[0])
"%s"%name[1:]`

#### 1.4.py
`>>> a=4
>>> print(a,',')
4 ,
>>> print(a,end=',')    //   end= ???
4,>>>`

#### 1.5.py
` import turtle   // ???
>>> turtle.pensize(2)
>>> turtle.circle(10)     `

#### 1.6.py

```
from datetime import datetime
print(now)
2021-01-21 19:20:20.278945
>>> now.strftime("%x")
'01/21/21'
>>> now.strftime("%X")
'19:20:20'
```

### 思考与练习

> 两个连续的printO 函数输出内容一般会分行显示，即调用printO函数后会换行结束当前行，如何让两个printO函数的输出打印在一行内?  
print(XX, end=":")

> import 保留字用来引入函数库，绘制图形可以使用什么Python 函数库?  //  turtle

> 获得系统的日期和时间使用什么Python 函数库?    // datetime

## IPO程序

数据输入的来源和方式：
文件，网络，随机数，内部参数
控制台??? 交互界面

图灵测试???

字符串拼接：
`strl = input(" 请输入一个人的名字: ")
str2 = input(" 请输入一个国家名字: ")
print(" 世界这么大.{}想去{}看看. ".format(strl , str2))`

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





