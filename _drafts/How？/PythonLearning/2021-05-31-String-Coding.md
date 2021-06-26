

 UTF-16 LE BE 对比 ||


### IDE编码
打印 koi8-r 编码的字符串有可能会在你的屏幕上显示为乱码，因为你的 Python IDE 将这些字符作为 iso-8859-1 的编码进行解析，而不是 koi8-r 编码。但是，至少它们 能打印。（并且，如果你仔细看，当在一个不支持 unicode 的文本编辑器中打开最初的【setdefaltencoding 决定了print，函数能打印什么样的字符。不染的话需要在print函数里面指定编码
如果要打印的内容和打印函数的编码，不一致，比如你用汉语的编码打印俄语，那就会报错。
是如果你打印的内容，你打印的语言，不被你的编程环境IDE，支持的话，那就虽然打印不报错，但是打印出来的是乱码

sitecustomize.py 是一个特殊的脚本；Python 会在启动的时候导入它，所以在其中 的任何代码都将自动运行。就像注解中提到的那样，它可以放在任何地方（只要 import 能够找到它），但是通常它位于 Python 的 lib 目录的 site-packages 目录中。恩，setdefaultencoding 函数设置默认编码。Python 会在任何需要自动将 unicode 字符串强制转换为正规字符串的地方，使用这个编码模式。

## 打印字符串时，Python 试图将字符串转换为你的默认编码
sitecustomize.py 是一个特殊的脚本；Python 会在启动的时候导入它，所以在其中 的任何代码都将自动运行。就像注解中提到的那样，它可以放在任何地方（只要 import 能够找到它），但是通常它位于 Python 的 lib 目录的 site-packages 目录中。恩，setdefaultencoding 函数设置默认编码。Python 会在任何需要自动将 unicode 字符串强制转换为正规字符串的地方，使用这个编码模式。
s = u >>> print
'La Pe\xf1a'
s
Traceback (innermost last):
File "<interactive input>", line 1, in ?
UnicodeError: ASCII encoding error: ordinal not in range(128)
>>>
print
s.encode(
'latin-1'
)
La Peña
python utf8 unicode examples
ANSI UTF-16LE UTF-16BE UTF-8  带有BOM的UTF-8
检测为 GB2312  UTF-16 UTF-16 UTF-8  UTF-8-SIG
"C:\Program Files (x86)\Python36-32\python.exe" D:/OneDrive/LCL_Github/Teaching/SongTian/Sources/st03_8_str_coding_emoji_unicode.py
b'\xbc\xd3\xd3\xcd\xa3\xa1\xcd\xa8\xd0\xc520\xbc\xb6\xcd\xac\xd1\xa7\xa3\xac\xc5\xac\xc1\xa6\xb3\xc9\xce\xaapython\xb8\xdf\xca\xd6\xa3\xa1'
{'encoding': 'GB2312', 'confidence': 0.99, 'language': 'Chinese'}
文件内容为：
加油！通信20级同学，努力成为python高手！
b'\xff\xfe\xa0R\xb9l\xb9l\x01\xff\x1a\x90\xe1O2\x000\x00\xa7~\x0cTf[\x0c\xff\xaaR\x9bR\x10b:Np\x00y\x00t\x00h\x00o\x00n\x00\xd8\x9aKb\x01\xff'
{'encoding': 'UTF-16', 'confidence': 1.0, 'language': ''}
文件内容为：
加油油！通信20级同学，努力成为python高手！
b'\xfe\xffR\xa0l\xb9l\xb9l\xb9\xff\x01\x90\x1aO\xe1\x002\x000~\xa7T\x0c[f\xff\x0cR\xaaR\x9bb\x10N:\x00p\x00y\x00t\x00h\x00o\x00n\x9a\xd8bK\xff\x01'
{'encoding': 'UTF-16', 'confidence': 1.0, 'language': ''}
文件内容为：
加油油油！通信20级同学，努力成为python高手！
b'\xe5\x8a\xa0\xe6\xb2\xb9\xe6\xb2\xb9\xe6\xb2\xb9\xe6\xb2\xb9\xef\xbc\x81\xe9\x80\x9a\xe4\xbf\xa120\xe7\xba\xa7\xe5\x90\x8c\xe5\xad\xa6\xef\xbc\x8c\xe5\x8a\xaa\xe5\x8a\x9b\xe6\x88\x90\xe4\xb8\xbapython\xe9\xab\x98\xe6\x89\x8b\xef\xbc\x81'
{'encoding': 'utf-8', 'confidence': 0.99, 'language': ''}
文件内容为：
加油油油油！通信20级同学，努力成为python高手！
b'\xef\xbb\xbf\xe5\x8a\xa0\xe6\xb2\xb9\xe6\xb2\xb9\xe6\xb2\xb9\xe6\xb2\xb9\xe6\xb2\xb9\xef\xbc\x81\xe9\x80\x9a\xe4\xbf\xa120\xe7\xba\xa7\xe5\x90\x8c\xe5\xad\xa6\xef\xbc\x8c\xe5\x8a\xaa\xe5\x8a\x9b\xe6\x88\x90\xe4\xb8\xbapython\xe9\xab\x98\xe6\x89\x8b\xef\xbc\x81'
{'encoding': 'UTF-8-SIG', 'confidence': 1.0, 'language': ''}
文件内容为：
加油油油油油！通信20级同学，努力成为python高手！

========unicode:
b'\\u52a0\\u6cb9\\uff01\\u901a\\u4fe120\\u7ea7\\u540c\\u5b66\\uff0c\\u52aa\\u529b\\u6210\\u4e3apython\\u9ad8\\u624b\\uff01'
b'\\u52a0\\u6cb9\\u6cb9\\uff01\\u901a\\u4fe120\\u7ea7\\u540c\\u5b66\\uff0c\\u52aa\\u529b\\u6210\\u4e3apython\\u9ad8\\u624b\\uff01'
b'\\u52a0\\u6cb9\\u6cb9\\u6cb9\\uff01\\u901a\\u4fe120\\u7ea7\\u540c\\u5b66\\uff0c\\u52aa\\u529b\\u6210\\u4e3apython\\u9ad8\\u624b\\uff01'
b'\\u52a0\\u6cb9\\u6cb9\\u6cb9\\u6cb9\\uff01\\u901a\\u4fe120\\u7ea7\\u540c\\u5b66\\uff0c\\u52aa\\u529b\\u6210\\u4e3apython\\u9ad8\\u624b\\uff01'
b'\\u52a0\\u6cb9\\u6cb9\\u6cb9\\u6cb9\\u6cb9\\uff01\\u901a\\u4fe120\\u7ea7\\u540c\\u5b66\\uff0c\\u52aa\\u529b\\u6210\\u4e3apython\\u9ad8\\u624b\\uff01'

python unicode 及解码编码方式   https://blog.csdn.net/Eclipsesy/article/details/78843461
http://www.ruanyifeng.com/blog/2007/10/ascii_unicode_and_utf-8.html   https://blog.csdn.net/ran337287/article/details/56298949
http://xahlee.info/python/unicode.html
 read and write unicode (UTF-8) files in Python?
import io
with io.open(filename,'r',encoding='utf8') as f:
    text = f.read()
# process Unicode text
with io.open(filename,'w',encoding='utf8') as f:
    f.write(text)
https://stackoverflow.com/questions/15750079/utf-8-ascii-unicode-examples-python




