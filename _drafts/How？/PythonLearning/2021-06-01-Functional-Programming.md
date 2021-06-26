

* **编程范式**：命令式编程，函数式编程-中小规模软件，OO编程 ！

# lambda函数-匿名函数 5.1,6.6节 ??

```
<函数名> = lambda <参数列表> : <表达式>
```

```
def <函数名>(<参数列表>) :
    <函数体>
    return <返回值列表>
```
定义中，形参；调用时，实参

Can a function have no parameters?
The lesson brief states that “Functions can have zero, one or more parameters”.

All functions in Python can be passed as an argument to another function (that just happens to be the sole purpose of lambda functions)
![](vx_images/5034309196561.png)
![](vx_images/2395907208694.png)

### 哈姆雷特词频统计 [没用到dict，而是用到list类型]

def getText():
    txt = open("hamlet.txt", "r").read()
    txt = txt.lower()
    for ch in '!"#$%&()*+,-./:;<=>?@[\\]^_‘{|}~':
        txt = txt.replace(ch, " ")
    return txt
 
hamletTxt = getText()
words  = hamletTxt.split()
counts = {}
for word in words:           
    counts[word] = counts.get(word,0) + 1
items = list(counts.items())
items.sort(key=lambda x:x[1], reverse=True)   # 高阶函数+匿名函数
for i in range(10):
    word, count = items[i]
    print ("{:<10},{:>5}".format(word, count))



# 函数式编程

https://www.liaoxuefeng.com/wiki/1016959663602400/1017328525009056

虽然也可以归结到面向过程的程序设计，但其思想更接近数学计算。【】

函数式编程就是一种抽象程度很高的编程范式，纯粹的函数式编程语言编写的函数没有变量，因此，任意一个函数，只要输入是确定的，输出就是确定的，这种纯函数我们称之为没有副作用。而允许使用变量的程序设计语言，由于函数内部的变量状态不确定，同样的输入，可能得到不同的输出，因此，这种函数是有副作用的。

函数式编程的一个特点就是，允许把函数本身作为参数传入另一个函数，还允许返回一个函数！

Python对函数式编程提供部分支持。由于Python允许使用变量，因此，Python不是纯函数式编程语言。


讨论 / JavaScript / 看完感觉Function这东西和python的functools一毛一样
 

RubyonRailPython
#1 Created at 2018/8/15 22:25
突然有种语言的确是共通的奇妙感

## 一个函数就可以接收另一个函数作为参数，这种函数就称之为高阶函数。

#### 一个最简单的高阶函数：

def add(x, y, f):
    return f(x) + f(y)


#### 随便写的加减乘除，大概就这个意思吧？

def plus(x, y):
    return x + y
def minus(x, y):
    return x - y
def multi(x, y):
    return x * y
def divide(x, y):
    if y!=0:
        return x / y
    else:
        return x*float("inf")
def calculate(x,y,f):
    return f(x,y)
#计算  2*(3+4)-5/6 = 13.16666
>>> print(calculate(calculate(2,calculate(3,4,plus),multi),calculate(5,6,divide),minus))
...
>>> 13.166666666666666


【】这个传入函数 有点简单工厂模式??? 的感觉啊