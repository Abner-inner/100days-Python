# 100days-PythonDiary
### 2021.02.21

## Day5

```interesting game  "CRAPS赌博游戏"

from random import randint

money = 1000
while money > 0:
    print('你的总资产为:', money)
    needs_go_on = False
    while True:
        debt = int(input('请下注: '))
        if 0 < debt <= money:
            break
    first = randint(1, 6) + randint(1, 6)
    print('玩家摇出了%d点' % first)
    if first == 7 or first == 11:
        print('玩家胜!')
        money += debt
    elif first == 2 or first == 3 or first == 12:
        print('庄家胜!')
        money -= debt
    else:
        needs_go_on = True
    while needs_go_on:
        needs_go_on = False
        current = randint(1, 6) + randint(1, 6)
        print('玩家摇出了%d点' % current)
        if current == 7:
            print('庄家胜')
            money -= debt
        elif current == first:
            print('玩家胜')
            money += debt
        else:
            needs_go_on = True
print('你破产了, 游戏结束!')
```

### 练习
```生成斐波那契数列的前20个数
num=int(input('numble='))
a=1
b=1
print("1")
print("1")
for i in range(num-2):
    x=a+b
    a=b
    b=x
    print(x)```

```找出10000以内的完美数
x=0
lim=int(input("lim="))
for i in range(1,lim+1):
    for j in range(1,i)：
        if i%j==0:
            x += j
    if i==x:
        print(i)
    x=0```

```输出100以内所有的素数
count=0
lim=int(input('limit='))
for i in range(2,lim+1):
    for j in range(2,i):
        if i%j==0:
            count+=1
    if count==0:
        print(i)
    count=0```
    
    写程序是一件我非常喜欢的事情，在写程序的过程中需要逻辑思维的运转，而测试时总会发现数不尽的bug，这些bug就是写程序中我们所没有注意到的部分，纠错的过程本质上让自己对程序的实际运行过程有了一个更加细致的了解
    也说明业精于勤，需要不断的回顾，回溯源头，遍历每一个细节，只有对每一个细节完全掌握了，才能去教电脑怎么做
    也是体现施动者必定需要对每一个细节都把握的非常准确，不能含糊，否则就会形成沟通的障碍
