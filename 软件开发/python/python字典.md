# python字典


## 概念

字典是另一种可变容器模型，且可存储任意类型对象。

字典的每个键值(key=>value)对用冒号(:)分割，每个对之间用**(,)**分割，整个字典包括在花括号**{}**中,格式如下所示

> d = {key1:value1,key2:value2}

键必须是唯一的，但值则不必。

值可以取任何数据类型，但键必须是不可变的，如字符串，数字和元组。

## 访问字典里的值

把相应的键放入到方括号中，如下示例：

> ```python
> dict = {'name':'runoob','age':7,"class":"first"}
> 
> print(dict['name'])
> print(dict['age']
> ```
>
> 

## 修改字典

向字典添加新内容的方法是增加新的键/值对，修改或删除已有键/值对如下：

> ```python
> dict = {'name':'runoob','age':7,"class":"first"}
> 
> dict['age']=0 #修改更新了age键的值
> dict['school']='菜鸟教程' #添加了信息
> 
> ```
>
> 

## 删除字典元素

能删除单一的元素也能清空字典，清空只需一项操作

> ````python
> dict = {'name':'runoob','age':7,"class":"first"}
> 
> del dict['name']/
> dict.clear()
> del dict
> ````

## 字典内置函数&方法

python字典包含了以下内置函数：

| 序号 | 函数及描述                                               | 示例                                                         |
| ---- | -------------------------------------------------------- | ------------------------------------------------------------ |
| 1    | len(dict)计算字典元素个数，即键的总数                    | dict = {'name':'runoob','age':7,"class":"first"}    len(dict)=3 |
| 2    | str(dict)输出字典，以可打印的字符串表示                  | dict = {'name':'runoob','age':7,"class":"first"}         str(dict) |
| 3    | type(dict)返回输入的变量类型，如果变量是字典返回字典类型 | dict = {'name':'runoob','age':7,"class":"first"}         type(dict) |

python字典包含了以下方法

| 序号 | 方法及描述                              |
| ---- | --------------------------------------- |
| 1    | radiansdict.clear()删除字典内所有元素   |
| 2    | radiansdict.copy()返回一个字典的浅复制  |
| 3    | radiansdict.fromkeys()创建一个新字典，  |
| 4    | radiansdict.get(key,default=None)       |
| 5    | radiansdict.items()                     |
| 6    | key in dict                             |
| 7    | radiansdict.keys()                      |
| 8    | radiansdict.update(dict2)               |
| 9    | radiansdict.values()                    |
| 10   | pop(key,[default])                      |
| 11   | popitem()                               |
| 12   | radiansdict.setdefault(key,defaut=None) |

