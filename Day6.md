# 100days-PythonDiary
##2021.02.22

###Day6

new knowledge
```__name__是Python中一个隐含的变量，它代表了模块的名字
只有被Python解释器直接执行的模块名字才是__main__```

练习
```实现计算最大公约数和最小公倍数的函数
def function(a,b):
	if a < b:
		c=a
		a=b
		b=c
	for i in range(1,b+1):
		if a%i==0 and b%i==0:
			gy=i
	gb=a*b/gy
	return gy,gb```

```实现判断一个数是不是回文数的函数
def huiwenshu(num):
	new_num=str(num)[-1,0]
	a=True if new_num==str(num) else a=False
	return a```

```实现判断一个数是不是素数的函数
def func(num):
	for i in range(2,num):
		if num%i==0:
			return False
	return True if num!=1 else False```

```写一个程序判断输入的正整数是不是回文素数
def func(num):
	return huiwenshu(num) and func(num)```
