# 列表

[TOC]

## 列表是什么

列表是一系列按特定顺序排序的元素组成.你可以创建包含字母表内的所有字母,也可以将各种东西加入列表中,其中元素之间没有任何关系,鉴于列表通常包含多个元素,给列表制定一个复数的名称是个不错的主意.

##　使用和访问列表

列表是有序集合，因此要访问列表的任何元素，只需要告诉ｐｙｔｈｏｎ该元素的位置和索引即可．在ｐｙｔｈｏｎ中，第一个列表元素的索引是**0**,而访问最后一个元素，其索引也可以表示为**-1**

```python
#　创建一个列表并且打印它
bicyles = ['trek','cannondale','redlien']
print(bicyles)
# 访问列表的元素
print(bicyles[0])#　第一个元素
print(bicyles[-1])# 最后一个元素
```



## 修改,添加和删除列表元素

### 修改列表元素

修改列表元素的语法与访问列表元素的语法类似,要修改列表元素,可指定列表名和要修改的元素索引.

```python
motorcycles = ['honda','yamaha','suzuki']
print(motorcycles)

motorcycles[0] = 'asdsd'
print(motorcycles)
# 输出
['honda','yamaha','suzuki']
['asdsd','yamaha','suzuki']
```

### 添加列表元素

1. 在列表末尾添加元素

   ```python
   motorcycles = ['honda','yamaha','suzuki']
   print(motoceycles)
   # 使用.append()内置方法在列表末尾添加元素
   motorcycles.append("jkl")
   print(motoceycles)
   ['honda','yamaha','suzuki']
   ['asdsd','yamaha','suzuki','jkl']
   ```

2. 在列表中插入元素

   ```python
   motorcycles = ['honda','yamaha','suzuki']
   motorcycles.insert(0,'ducati')
   # 这种操作将指定索引后的所有元素向后移一个索引
   ```

### 从列表删除元素

你经常需要从列表中删除一个或多个元素.

1. 使用del语句删除元素

```python
motorcycles = ['honda','yamaha','suzuki']
print(motorcycles)
# 使用ｄｅｌ语句删除指定索引位置的元素
del motorcycles[0]
print(motorcycles)
```

2. 使用pop方法删除元素

```python
motorcycles = ['honda','yamaha','suzuki']

popped_motocrycles = motorctcles.pop()
print(motocrycles)
print(popped_motocrycles)
# 输出
['honda','yamaha','suzuki']
suzuki
```

### 组织列表

1. 使用方法sort()对列表进行永久性排序

   ```python
   cars = ['bmw','audi','toyota','subaru']
   cars.sort()
   
   ```

   

## 遍历列表

在处理列表时，经常需要对列表的每个元素执行相同的操作，可以通过for循环来遍历迭代列表元素.

```python
magicians = ['alice','david','carolina']
for magician in magicians:
    print(magician)
# 输出
alice
david
carolina
```

创建数值列表

使用函数**range()**,Python range()函数让你能够轻松生成一系列数字

```python
for valve in range(1,6):
    print valve
for valve in range(1,6,2)
	print valve
print(sum(range(1,101)))
# 输出
1
2
3
4
5
1
3
5
5050
```

## **列表解析**

前面介绍的生成列表squares的方式包含三四行代码,而列表解析让你只需要编写一行代码就能生成这样的列表,**列表解析**将for循环和创建新元素的代码合并成一行,并自动附加新元素

下面的实例使用列表解析创建一个平方数列表:

```python
squares = [valve**2 for valve in range(1,100)]
#　列表解析的格式是
# 列表名称　＝　[要执行的操作　for循环]
```



## 使用列表的一部分

### 切片

要创建切片,可指定要使用的第一个元素,和最后一个元素的索引

```python
players = ['charles','martina','michael','florence']
print(players[0:3])
# 输出
['charles','martina','michael']
```

