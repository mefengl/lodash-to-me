# lodash-to-me
 一边看Lodash文档，一边写下对每个接口应用场景的猜想

## Array

chunk

做多栏布局的时候，划分数据

compact

不用写if判断，方便的过滤掉数组中的假值

concat

合并多个flatten的数组或值

difference

比较同一用户关注列表的变化

differenceBy

单元函数的返回值作为比较的依据

differenceWith

comparator作为比较函数

drop

从左删除n个元素

dropRight

从右删除n个元素

dropRightWhile

从右删除满足条件的元素

dropWhile

从左删除满足条件的元素

fill

可以用于初始化数组的一部分

findIndex

自定义匹配函数

findLastIndex

从后往前的findIndex

first

不用担心IndexError的array[0]，LISP的car

flatten

只拆一层

flattenDeep

拆掉所有层

flattenDepth

指定拆层数

fromPairs

[['x', 1], ['y', 2]] => {'x': 1, 'y': 2}

head

first，不过4个字母

indexOf

匹配函数是==的findIndex

initial

形同pop，但是不用改变原数组

intersection

交集

intersectionBy

交集，单元函数的返回值作为比较的依据

intersectionWith

交集，comparator作为比较函数

join

JS有了它的join

last

不用担心IndexError的array[-1]

lastIndexOf

匹配函数是==的findLastIndex

nth

不用担心IndexError的array[n]

pull

批量删除指定元素

pullAll

pull 一个数组中 All 元素

pullAllBy

pullAll，单元函数的返回值作为比较的依据

pullAllWith

pullAll，comparator作为比较函数

pullAt

删除索引们对应的元素

remove

删除满足条件的元素

reverse

JS有了它的reverse

slice

JS有了它的切片

sortedIndex

查找插入位置

sortedIndexBy

查找插入位置，单元函数的返回值作为比较的依据

sortedIndexOf

在sorted数组中求indexOf

sortedLastIndex

在sorted数组中求lastIndexOf

sortedUniq

在sorted数组中求uniq

sortedUniqBy

sortedUniq，单元函数的返回值作为比较的依据

tail

不用担心IndexError的array[1:]，LISP的cdr

take

不用担心IndexError的array[:n]

takeRight

不用担心IndexError的array[-n:]

takeRightWhile

从右压仓

takeWhile

从左压仓

union

并集

unionBy

union，单元函数的返回值作为比较的依据

unionWith

union，comparator作为比较函数

uniq

去重

uniqBy

uniq，单元函数的返回值作为比较的依据

uniqWith

uniq，comparator作为比较函数

unzip

行列互换

unzipWith

unzip，提供合并函数

without

不原地修改的pull

xor

异或

xorBy

xor，单元函数的返回值作为比较的依据

xorWith

xor，comparator作为比较函数

zip

将参数中的数组合并成一个数组，然后行列互换

zipObject

将参数中的数组合并成一个数组，然后fromPairs

zipObjectDeep

智能的zipObject

zipWith

zip，提供合并函数
