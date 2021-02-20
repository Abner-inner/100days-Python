# 100days-PythonDiary
###2021.02.20

####练习

```输入一个正整数判断是不是素数
s=int(input('s= '))
count=0
for i in range(2,s):
    if s%i==0:
        count += 1
if count != 0:
    print('false')
else:
    print('true')
```

```输入两个正整数，计算它们的最大公约数和最小公倍数
a=int(input("a="))
b=int(input("b="))
if a<b:
    c=a
    a=b
    b=c
for i in range(1,b+1):
    if a%i==0 and b%i==0:
        big_gongyue = i
small_gongbei= a*b/big_gongyue
print("big_gongyue=%d"%big_gongyue)
print("small_gongbei=%d"%small_gongbei)
```

```打印一些三角形图案
row=int(input("row= "))
for i in range(row):
    for j in range(1,i+2):
        print('*',end='')
    print()

for i in range(row):
    for j in range(row):
        if j+1<row-i:
            print(" ",end="")
        else:
            print("*",end="")
    print()

for i in range(row):
    for j in range(2*row-1):
        if j+1<row-i or j+1>row+i:
            print(" ",end="")
        else:
            print("*",end='')
    print()
