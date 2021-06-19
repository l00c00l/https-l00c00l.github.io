

try-except-else-finally   
# continue     ^    SyntaxError: 'continue' not supported inside 'finally' clause

-finally对应语句块4一定执行
-else对应语句块3在不发生异常时执行
try:
<语句块1>
except :
<语句块2>
else :
<语句块3>
finally :
<语句块4>
-当循环没有被break语句退出时，执行else语句块 -else语句块作为"正常"完成循环的奖励
for<变量> in<遍历结构> :
<语句块1>
else:
<语句块2>
while<条件> :
<语句块1>
else:
<语句块2>

09-else+for-while-except.py  else 与其它结构的综合 例子  
上面的两个例子，都可以通过改写循环条件或者修改循环逻辑，去掉break和continue语句。20210502