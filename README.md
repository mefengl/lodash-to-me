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

## Collection

countBy

计数，单元函数的返回值作为计数的依据

every

所有元素满足条件

filter

不原地修改的remove

find

找到第一个满足predicate的元素

findLast

find，但最后一个

flatMap

map，然后flatten

flatMapDeep

map，然后flattenDeep

flatMapDepth

map，然后flattenDepth

forEach

可以用在字典上的forEach

forEachRight

反向遍历

groupBy

分组，单元函数的返回值作为分组依据，返回字典，key是分组依据，value是分组的元素数组

includes

是否包含

invokeMap

LISP中的mapcar

keyBy

提取数组中某值作为数组的key，可以是单元函数

map

不原地修改的invokeMap

orderBy

sortBy，但是接受的是一一对应的函数数组和排序方向数组

partition

根据predicate的真假结果分成两个数组

reduce

JS有了它的reduce

reduceRight

reduce，但是反向

reject

类似filter，但是假值留下

sample

单个采样

sampleSize

指定数量采样

shuffle

JS有了它的shuffle

size

JS有了它的len

some

至少有一个

sortBy

排序，单元函数的返回值作为排序依据

## Date

now

得到timestamp

## Function

after

生成一个调用n次后才会执行的函数，可以用在模型训练中的500次循环输出一次的场景

ary

控制函数获取的参数个数，并不知道有什么用

before

生成一个调用n次前才会执行的函数，可以用在闹钟的贪睡功能

bind

想不到使用的场景，this的问题箭头函数可以解决

bindKey

绑定key，key对应的值可以更改，从而实现更改绑定的函数

curry

柯里化

curryRight

curry，但是参数右对齐

debounce

防抖，可以用在搜索框的输入

defer

延迟执行，setTimeout(func, 1ms)

delay

defer，但是可以指定延迟时间（那和setTimeout有什么区别？

flip

参数反转

memoize

记忆函数，似乎是通过指针判断是否已经计算过

negate

「函数」取反

once

只承认第一次调用的参数，将函数转为单例

overArgs

参数转换，然后分配给多个函数

partial

柯里化？

partialRight

partial，但是参数右对齐

rearg

参数重排

rest

参数转换，将剩余参数转为数组

spread

参数转换，将数组转为参数

throttle

节流，可以用在滚动加载，和debounce的区别是，throttle能保证每隔一段时间执行

unary

ary，但是ary(func, 1)

wrap

给函数包装一层，不知道有什么用

## Lang

castArray

转Array

clone

JS有了它的copy

cloneDeep

clone，但是深拷贝

cloneDeepWith

cloneDeep，但是可以指定拷贝规则

cloneWith

clone，但是可以指定拷贝规则

conformsTo

every，但可以方便分属性确认

eq

NaN == NaN 的比较

gt

>

gte

>=

isArguments

判断是否是arguments对象？

isArray

判断是否是数组

isArrayBuffer

判断是否是ArrayBuffer

isArrayLike

判断是否是类数组，比如HTMLCollection

isArrayLikeObject

isArrayLike，但是元素是对象

isBoolean

判断是否是bool

isBuffer

判断是否是Buffer

isDate

判断是否是Date

isElement

判断是否是DOM元素

isEmpty

human understandable empty

isEqual

eq，但是比较内在结构

isEqualWith

isEqual，但是可以指定比较规则

isError

判断是否是Error

isFinite

判断是否不是Infinity

isFunction

判断是否是function

isInteger

判断是否是integer

isLength

判断一个数是否可能是数组的length

isMap

判断是否是Map

isMatch

部分eq

isMatchWith

isMatch，但是可以指定比较规则

isNaN

判断是否是NaN

isNative

判断是否是native函数

isNil

判断是否是null或者undefined

isNull

判断是否是null

isNumber

判断是否是number，包括NaN，Infinity

isObject

判断是否是object

isObjectLike

isObject，但是typeof objectLike == 'object'

isPlainObject

判断是否为一代对象

isRegExp

判断是否是RegExp

isSafeInteger

判断是否是IEEE-754双精度整数

isSet

判断是否是Set

isString

判断是否是string

isSymbol

判断是否是symbol

isTypedArray

判断是否是TypedArray，比如Uint8Array

isUndefined

判断是否是undefined

isWeakMap

判断是否是WeakMap

isWeakSet

判断是否是WeakSet

lt

<

lte

<=

toArray

是object，就转为array

toFinite

转为finite

toInteger

转为integer

toLength

转为可能的length

toNumber

转为number

toPlainObject

转为一代对象

toSafeInteger

转为IEEE-754双精度整数

toString

转为string

## Math

add

\+

ceil

向上取整，可以指定小数点前后位数

divide

/

floor

向下取整，可以指定小数点前后位数

max

JS有了它的max

maxBy

max，但是可以指定映射方式

mean

JS有了它的mean

meanBy

mean，但是可以指定映射方式

min

JS有了它的min

minBy

min，但是可以指定映射方式

multiply

\*

round

四舍五入，可以指定小数点前后位数

subtract

\-

sum

JS有了它的sum

sumBy

sum，但是可以指定映射方式

## Number

clamp

toSafeInteger，但是可以指定上下限

inRange

clamp，但是返回是否在范围内

random

JS有了它的random，random(int)是randint，random(int, int)是randrange，random(int, true)是randfloat

## Object

assign

*不知道有什么用

assignIn

*assign，但是会把原型链上的属性也拷贝

assignInWith

*assignIn，但是可以指定拷贝规则

assignWith

*assign，但是可以指定拷贝规则

at

*通过path数组获取对象的值

create

*指定继承属性

defaults

指定默认值

defaultsDeep

defaults，但是不止一层

findKey

find，但是返回key

findLastKey

findKey，但是从后往前

forIn

可以用在字典上的forIn

forInRight

forIn，但是从后往前

forOwn

*遍历定义时的属性

forOwnRight

forOwn，但是从后往前

functions

forOwn，但是返回函数属性的名字

functionsIn

functions，但是非定义时的函数属性的名字也会返回

get

at，但是只提取一个

has

at，但是只判断是否存在

hasIn

has，但是会检查原型链上的属性

invert

键值互换

invertBy

invert，但是可以指定values_to_key的映射方式

invoke

在对象的部分属性上调用函数

keys

返回数组的key数组

keysIn

keys，但是会检查原型链上的属性

mapKeys

map，但是只映射key

mapValues

map，但是只映射value

merge

像Git merge 一样合并对象

mergeWith

merge，但是可以指定合并规则

omit

不要指定的属性，和pick相反

omitBy

omit，但是可以指定过滤方式，比如_.isNumber

pick

只要指定的属性，和omit相反

pickBy

pick，但是可以指定过滤方式，比如_.isNumber

result

*get，但可以调用函数

set

指定路径赋值

setWith

set，但是可以指定赋值规则

toPairs

键值对转为数组

toPairsIn

toPairs，但是会检查原型链上的属性

transform

*reduce 的替代

unset

指定路径恢复出厂设置

update

set，但是可以指定updater

updateWith

setWith，但是可以指定updater

values

返回字典的value数组

valuesIn

values，但是会检查原型链上的属性

## Seq

_

类似jQuery的$，转化后就可以链式调用

chain

_，但是需要调用value取值

tap

*tap into

thru

*pass thru

prototype[Symbol.iterator]

*I don't know

prototype.at

*wrapper version of _.at

prototype.chain

*wrapper version of _.chain

prototype.commit

执行链式调用

prototype.next

*返回下一个值

prototype.plant

*同chain，但是新的初始值

prototype.reverse

*wrapeer version of _.reverse

prototype.value

返回解析值

## String

camelCase

驼峰命名

capitalize

首字母大写

deburr

去除重音符号

endsWith

是否以指定字符串结尾

escape

为HTML转义

escapeRegExp

为正则表达式转义

kebabCase

短横线命名

lowerCase

小写命名

lowerFirst

首字母小写

pad

左右填充至指定长度

padEnd

右填充至指定长度

padStart

左填充至指定长度

parseInt

转成整数

repeat

重复指定次数

replace

替换

snakeCase

下划线命名

split

分割

startCase

首字母大写命名

startsWith

是否以指定字符串开头

template

*有了模版字符串，这个就没啥用了

toLower

全小写

toUpper

全大写

trim

去除首尾填充

trimEnd

去除尾部填充

trimStart

去除首部填充

truncate

限制字符串长度，自动添加省略号，可以用在标题上

unescape

反escape

upperCase

全大写命名

upperFirst

首字母大写

words

分割成单词

## Util

attempt

不用catch的try，可以用在querySelector，但似乎jQuery已经有了

bindAll

绑定对象的方法们到对象上

cond

类似switch，但条件是函数

conforms

类似_.matches，但条件是函数

matchesProperty

创建一个函数，判断对象的指定属性是否符合条件，可以用于_.filter，_.find

method

*I don't know

methodOf

*oppoiste of _.method

mixin

给对象添加方法，可以用于扩展lodash

noConflict

恢复_的原始值

noop

undefined 制造机

nthArg

返回第n个参数的函数

over

批量执行函数，返回结果数组

overEvery

over + every

overSome

over + some

property

有path，等待object去取值的函数

propertyOf

有object，等待path去取值的函数

range

JS有了它的range

rangeRight

JS有了它的reversed(range)

runInContext

*创建一个新的lodash实例

stubArray

[]

stubFalse

false

stubObject

{}

stubString

""

stubTrue

true

times

执行n次，比如结合stubArray，创建n个空数组

toPath

从字符串path转成path数组

uniqueId

添加唯一id

## Properties

*I don't know

## Methods

*I don't know
