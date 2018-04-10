# 18409
upper


利用map()函数，把用户输入的不规范的英文名字，变为首字母大写，其他小写的规范名字。输入：['adam', 'LISA', 'barT']，输出：['Adam', 'Lisa', 'Bart']：


# -*- coding: utf-8 -*-  
def normalize(name):  
    name=name[0].upper()+name[1:].lower()  
    return name  
L1 = ['adam', 'LISA', 'barT']  
L2 = list(map(normalize, L1))  
print(L2)  


# 1.利用map()函数，把用户输入的不规范的英文名字，变为首字母大写，其他小写的规范名字。输入：['adam', 'LISA', 'barT']，输出：['Adam', 'Lisa', 'Bart']：
def formating(name):
    return name.title()
     
L = list(map(formating,['adam', 'LISA', 'barT']))
print("练习1的答案:",L) # == > 练习1的答案: ['Adam', 'Lisa', 'Bart']


# 2.Python提供的sum()函数可以接受一个list并求和，请编写一个prod()函数，可以接受一个list并利用reduce()求积：
def prod(L1=[]):
    def fn(x,y):
        return x * y
    return reduce(fn,L1)
P = prod([1,2,3,4,5,6,7,8])
print("练习2乘积的答案:",P) # == > 练习2乘积的答案: 40320


