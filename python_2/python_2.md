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
  
  - 删除list末尾的元素：
  
    ```python
    >>> classNames.pop()
    'chinese'
    ```
  
  - 删除指定位置的元素：
  
    ```python
    >>> classNames.pop(0)
    'english'
    ```
  
  - 替换元素：
  
    ```python
    >>> classNames[0] = 'chinese'
    ```
  
  - list里面元素类型可以不相同
  
  - list元素也可以是另一个list
  
  - tuple：有序列表，tuple一旦初始化不能修改，和list非常类似
  
    - 定义一个空的tuple， t = ()
    - 当tuple中有一个数的时候，可以自己定义 t = (1,)来消除歧义
  
  - 条件判断：
  
    - if判断
  
      - 语法结构： 
  
        ```python
        >>> if a > 18:
        		print('yes')
            elif a < 15:
                print('yes')
            else:
                print('no')
        ```
  
        当if 的条件为True时进去到分支中，否则的话进入到elif分支，最后进入到else分支
  
  - 循环：
  
    python循环判断有两种方式：
  
    - 1.for ... in 循环：
  
      ```python
      >>> a = ['1','2','3','4','5']
      >>> for x in a:
      	print(x)
      
      	
      1
      2
      3
      4
      5
      ```
  
    - 2.while循环：
  
      ```python
      >>> sum = 0
      >>> n = 0
      >>> while n < 5:
      	sum = sum + n
      	n = n + 1
      
      	
      >>> sum
      10
      ```
  
  - dict字典类型：
  
    使用的是key -value类型存储，格式为 {key: value}
  
    ```python
    >>> d = {'sum':10}
    >>> d['sum']
    10
    ```
  
  - dict常用方法：
  
    - get（）
  
      ```python
      >>> d.get('num')
      >>> d.get('num', 1)
      1
      ```
  
      当get方法没有获取到数据的时候，返回的是None，也可以指定默认值，当没有查询到数据时返回默认值
  
  - set类型：
  
    set和dict类型，是一组key的集合，不能包含重复的数据。
  
    - 初始化方式： 
  
      ```python
      >>> s = set([1,2,3])
      >>> s
      {1, 2, 3}
      ```
  
    - set的常用方法：
  
      - add：add(key)
  
        ```python
        >>> s.add(4)
        >>> s
        {1, 2, 3, 4}
        >>> s.add(4)
        >>> s
        {1, 2, 3, 4}
        ```
  
        当添加了重复数据的时候会自动过滤掉
  
      - remove：remove(key)
  
        ```python
        >>> s.remove(1)
        >>> s
        {2, 3, 4}
        ```
  
        删除set中指定的值