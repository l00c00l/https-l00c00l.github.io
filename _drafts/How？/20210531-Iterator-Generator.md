

第二个是迭代器（Iterator），第三个是生成器（Generator）||  



素数实现,代码不是很懂
用户5307799436 created at June 2, 2020 10:53 PM, Last updated at June 2, 2020 10:53 PM
def num():

    n = 1

    while True:

        n += 1

        yield n

def not_division(n):

    return lambda x: x % n > 0  #这里的x为it,但it是一个generator

def prime():

    it = num()

    while True:

        nn = next(it)

        yield nn

        it = filter(not_division(nn),it)

for n in prime():

    if n<1000:

        print(n)

    else:

        break