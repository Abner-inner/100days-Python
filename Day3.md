# 100days-PythonDiary
2021.02.19

练习：
英制单位英寸与公制单位厘米互换
x=input('length= (in or cm)')
if x[-2:] == 'in':
    l=eval(x[:-2])
    print('%.2f in=%.2f cm'%(l,l*2.54))
elif x[-2:] == 'cm':
    l=eval(x[:-2])
    print('%.2f cm=%.2f in'%(l,l/2.54))
else:
    print('the units is error')

百分制成绩转换为等级制成绩
score=eval(input('score= '))
if score <60:
    print('E')
elif score <70:
    print('D')
elif score <80:
    print('C')
elif score <90:
    print('B')
else:
    print('A')

输入三条边长，如果能构成三角形就计算周长和面积
l=input('a,b,c 三边长').split(',')
a=eval(l[0])
b=eval(l[1])
c=eval(l[2])
p=(a+b+c)/2
if a>b and a>c:
    big=a
    s1=b
    s2=c
elif b>c:
    big=b
    s1=a
    s2=c
else:
    big=c
    s1=a
    s2=b
if big<s1+s2:
    print('C = %.2f ,S = %.2f'%(2*p,(p*(p-a)*(p-b)*(p-c))**(0.5)))
else:
    print('can not be a triangle')


多做多练以熟悉基本操作，加油加油干！
