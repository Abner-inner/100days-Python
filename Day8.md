# Day8
### 2021.3.7

## 面向对象编程基础

使用class定义类<br>

驼峰命名法
=
小驼峰：littleHump
大驼峰：BigHump

```用initial为对象绑定属性
```

```私有属性private：给属性命名时以两个下划线做开头，如student.__name即为私有属性，否则为公开的（public）
   命名惯例，以单下划线表示受保护属性，但只是表示，本质仍是公开属性
```

## 重点：定义函数内部变量无法保留改变，但是可以改变外部对象的属性，通过改变属性影响外部变量

将一系列函数封装成类，只保留简介的外部接口