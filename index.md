  # this is a biggest one
  ## this is a small one than above that one
  ##### this is fifth degree one



  ## 👋  a practise


![网页形式](https://wallpapercave.com/wp/wp8757558.png "f1")

```
import math
r = int(input())
PI=math.pi
area = (r**2) * PI
print('%.7f' % area)  #保留七位小数

#序列和1
def he():
    n = int(input())
    return n * (1 + n) / 2  # 等差数列时间短 直接使用a+b会超时

s = int(he())
print(s)

#序列和2
def func(n):
    if n is None:  # 如果没有传入参数n，则从输入中获取,如果像序列和1那样直接从输入中获取值
        n = int(input())
    if n == 1:
        return 1
    return func(n - 1) + n
#或者像这样子，在外部先把n的值传入
#n = int(input())  # 获取用户输入
#a = func(n)  # 传递n给func函数
a = int(func())#直接调用func()
print(a)



#字符串对比
"""
给定两个仅由大写字母或小写字母组成的字符串(长度介于1到10之间)，它们之间的关系是以下4中情况之一：
　　1：两个字符串长度不等。比如 Beijing 和 Hebei
　　2：两个字符串不仅长度相等，而且相应位置上的字符完全一致(区分大小写)，比如 Beijing 和 Beijing
　　3：两个字符串长度相等，相应位置上的字符仅在不区分大小写的前提下才能达到完全一致（也就是说，它并不满足情况2）。比如 beijing 和 BEIjing
　　4：两个字符串长度相等，但是即使是不区分大小写也不能使这两个字符串一致。比如 Beijing 和 Nanjing
　　编程判断输入的两个字符串之间的关系属于这四类中的哪一类，给出所属的类的编号。
"""

def zifu(str1, str2):
    if len(str1) != len(str2):
        return 1
    else:
        if str1 == str2:
            return 2
        elif str1.lower() != str2.lower():   #str1.lower是将字符串全部转换为小写
            return 4
        return 3
if __name__ == '__main__':  #字面上，这是一个if判断，而__name__是一个内置的特殊变量，当我们
    str1 = input()          #希望将一个python模块（就是写好的py文件）导入其他python模块时，
    str2 = input()          #就只会执行if __name__ == "__main__":的语句
    print(zifu(str1, str2))

```


- [x] Turn on GitHub Pages
- [ ] Outline my portfolio
- [x] Introduce myself to the world
