### list

~Python内置的一种数据类型是列表：list。list是一种有序的集合，可以随时添加和删除其中的元素。

~用索引来访问list中每一个位置的元素，记得索引是从0开始的：

~list里面的元素的数据类型也可以不同

~当索引超出了范围时，Python会报一个`IndexError`错误，所以，要确保索引不要越界，记得最后一个元素的索引是`len(classmates) - 1`。如果要取最后一个元素，除了计算索引位置外，还可以用`-1`做索引，直接获取最后一个元素：

`len append insert pop del remove sort(永久) sorted（临时）reverse=True相反顺序排序  list.reverse()`

list=\[1,2,3\]  list.sort\(\) sorted\(list\)` `

数值列表统计计算：min max sum 

a=list\(range\(1,6,2\)\)

列表解析list=\[value\*2 for value in range\(11\)\]

### tuple

另一种有序列表叫元组：tuple。tuple和list非常类似，但是tuple一旦初始化就不能修改，比如同样是列出同学的名字：

tuple=\(1,2,3\)

"可变的”tuple

### dict

Python内置了字典：dict的支持，dict全称dictionary，在其他语言中也称为map，使用键-值（key-value）存储，具有极快的查找速度。要避免key不存在的错误，有两种办法，一是通过

`in`

判断key是否存在二是通过dict提供的

`get()`

方法，如果key不存在，可以返回

`None`

，或者自己指定的value：

要删除一个key，用

`pop(key)`

方法，对应的value也会从dict中删除：请务必注意，dict内部存放的顺序和key放入的顺序是没有关系的。

和list比较，dict有以下几个特点：这个通过key计算位置的算法称为哈希算法（Hash）。

1. 查找和插入的速度极快，不会随着key的增加而变慢；
2. 需要占用大量的内存，内存浪费多。

而list相反：

1. 查找和插入的时间随着元素的增加而增加；
2. 占用空间小，浪费内存很少。

所以，dict是用空间来换取时间的一种方法。

```
dict={'a':1,'b':2}
```

### set

set和dict类似，也是一组key的集合，但不存储value。由于key不能重复，所以，在set中，没有重复的key。

要创建一个set，需要提供一个list作为输入集合：

```
s=set([1,2,3])
add remove
```

set可以看成数学意义上的无序和无重复元素的集合，因此，两个set可以做数学意义上的交集、并集等操作:s1$s2 s1\|s2

