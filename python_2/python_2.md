[TOC]

## python数据类型

- 整型： 整型就是我们说的整数，如 1,2,10等, python可以处理任意大小的整数

- 浮点数类型：浮点数就是小数,如3.1415

- 字符类型：字符串可以使用单引号( '  ' )和双引号( "  " )引起来的任意文本，

- 布尔类型： 布尔值只包含两种值:True和False，要注意手写字段的大写。

- 空值：空值是python里提供的特殊值，用None表示。

- 变量：变量可以是任意类型，变量的规则：英文的大小写、数字和_的组合，不能用数字开头，如 

  a = 10 则a表示的是数字类型

  b = True 则b表示的是布尔类型

- 列表类型： list是python内置的列表数据类型，list是有序的集合，可以随时添加和删除其中的元素， 如： className = ['english', 'math']

  常用的命令：

  - 列表的个数：len()方法

    ```python
    >>> classNames = ['english','math']
    >>> len(classNames)
    2
    ```

  - 通过索引获取list的元素：
  
    ```python
    >>> classNames[0]
    'english'
    ```
  
  - 访问最后第一个元素：
  
    ```python
    >>> classNames[-1]
    'math'
    ```
  
  - 追加元素：
  
    ```python
    >>>classNames.append('chinese')
    ```
  
  - 插入元素到指定位置：
  
    ```python
    >>> classNames.insert(1,'german')
    >>> classNames
    ['english', 'german', 'math', 'chinese']
    ```
  
  - 