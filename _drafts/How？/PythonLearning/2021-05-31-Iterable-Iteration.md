迭代
https://www.liaoxuefeng.com/wiki/897692888725344/923029668363040
在Python中，迭代是通过for ... in来完成的，而很多语言比如C或者Java，迭代list是通过下标完成的，比如Java代码：
Python的for循环抽象程度要高于Java的for循环，因为Python的for循环不仅可以用在list或tuple上，还可以作用在其他可迭代对象上。【】!!!

list这种数据类型虽然有下标，但很多其他数据类型是没有下标的，但是，只要是可迭代对象，无论有无下标，都可以迭代，比如dict就可以迭代：

可迭代类型-可迭代对象（Iterable），List, set, dictionary, doubles, strings, … all of these objects are iterable  https://izziswift.com/making-a-python-user-defined-class-sortable-hashable/  ||    【各种例子！】


[遍历-Javascript也有这个概念！]
遍历Array可以采用下标循环，遍历Map和Set就无法使用下标。为了统一集合类型，ES6标准引入了新的iterable类型，Array、Map和Set都属于iterable类型。
具有iterable类型的集合可以通过新的for ... of循环来遍历。 https://www.liaoxuefeng.com/wiki/1022910821149312/1023024358748480