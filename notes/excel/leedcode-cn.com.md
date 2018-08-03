
[Leedcode](https://leetcode-cn.com/)踩过的坑
------------------------

## 基础

+ 除法
    ```
    # 地板除: // （返回不大于x的整数)
    -5//3 == -2
    # 真除法: / （无论任何类型都会保持浮点数形式)
    4/2 == 2.0
    ```

+ 异或
    ```
    3^3 == 0
    ```

## 数组 [list](https://www.cnblogs.com/adampei-bobo/p/6640581.html)

+ 转 set集合 过滤重复元素
    ```
    list1=[1,2,3,4,4]
    s=set(list1)
    # 使用add(key)添加元素，重复的元素自动过滤
    s.add(5)
    # 通过remove(key)方法可以删除元素
    s.remove(1)
    # 交集，使用&操作符
    s3=s1&s2
    # 并集，使用|操作符
    s4=s1|s2
    ```

+ slicing 与 slice assignment 区别
    ```
    a = [1, 2, 3]
    b = a[:]  
    # 切片 slicing 是浅拷贝，不影响原序列,分配新内存； 
    c[:] = a  
    # 切片赋值 slice assignment 是针对原序列进行操作，改变切片区域的序列。

    ```

+ .copy() 与 copy.deepcopy() 区别 
    ```
    l2 = l1.copy()  
    # id内存地址不一样，创建了两个空间, 第一层都是独立的的,从第二层开始都是是公用的，改一个都会变。
    import copy  # 先引入模块
    l2 = copy.deepcopy(l1)
    # 复制一份，完全没有变化，不会受l1的影响。l1改变，l2不会跟着改变。
    ```

+ List .sort()方法
    ```
    list.sort(cmp=None, key=None, reverse=False)
    # cmp -- 可选参数, 如果指定了该参数会使用该参数的方法进行排序。
    # key -- 主要是用来进行比较的元素，只有一个参数，具体的函数的参数就是取自于可迭代对象中，指定可迭代对象中的一个元素来进行排序。
    # reverse -- 排序规则，reverse = True 降序， reverse = False 升序（默认）。
    ```

+ 






