# Numpy 笔记

## Numpy 的基础数据结构

numpy.ndarray 

## ndarray 的 基础属性

ndim 表示数组维度（或轴）的个数。刚才创建的数组 arr_1_d 的轴的个数就是 1，arr_2_d 的轴的个数就是 2。

shape 表示数组的维度或形状， 是一个整数的元组，元组的长度等于 ndim。

​	可以使用 np.reshape(a,newshape,order)方法修改纬度，并且会生成一个新的ndarray对象。

​	Order它是指以什么样的顺序读写元素，其中有这样几个参数。

- ​	‘C’：默认参数，使用类似 C-like 语言（行优先）中的索引方式进行读写。(最常用的)
- ​	‘F’：使用类似 Fortran-like 语言（列优先）中的索引方式进行读写。
- ​	‘A’：原数组如果是按照‘C’的方式存储数组，则用‘C’的索引对数组进行 reshape，否则使用’F’的索引方式。

size 数组中的元素总数



dtype 数组中元素的类型，需要注意的是，在numpy中数组只允许是一种类型。

可以通过`astype()` 方法将类型进行修改。



## ndarray 支持的算术运算符操作

a-b

a*b

a@b

a<35



## ndarray 中常用的方法

![numpy_function](/Users/owenhan/documnets/Notebook/image/numpy函数.png)

### 创建一个新的 ndarray 对象 的方法

np.ones()

np.zeros()

np.arange([start],stop,[step],dtype)

np.linspace()



### 聚合类方法

np.sum()

np.max()

np.min()

np.argmin() 求最小值索引

np.argmax() 求最大值索引

np.argsort() 数组排序后返回原数组的索引

​	np.argsort 包括后面这几个关键参数：

- a 是要进行排序的原数组；
- axis 是要沿着哪一个轴进行排序，默认是 -1，也就是最后一个轴；
- kind 是采用什么算法进行排序，默认是快速排序，还有其他排序算法，具体你可以看看数据结构的排序算法。

np.cumsum() 每行累计求和

np.mean() 求均值



### 其他常用方法

np.concatenate((a1, a2, …), axis=0)  将多个数组按某一维度进行拼接。

np.

## 数组的轴

常用的一个参数axis ,参数值为数字 0 、1、 2 ....

例如：存在一个（3，2，3）的数组

当 axis=0时，会生成一个（2，3）的新数组

当 axis=1时，会生成一个（3，3）的新数组

当 axis=2时，会生成一个（3，2）的新数组

