### 对象

对象由：标识、类型、value组成

本质：一个内存块，拥有特定的值，支持特定类型的相关操作。

1. 标识用于唯一标识对象，通常对应于对象在计算机内存中的地址。使用内置函数id(obj)可返回对象obj的标识。
2. 类型用于表示对象存储的 “数据” 的类型。类型可以限制对象的取值范围以及可执行的操作。可以使用type(obj)获得对象的所属类型。
3. 值表示对象所属的数据的信息。使用print(obj)可以直接打印出值。

### 引用

在Python中，变量是对象的引用。因为，变量存储的是对象的地址。变量通过地址引用了 “对象”。

变量位于栈内存，对象位于堆内存。

1. Python是动态类型语言：不需要显式的声明类型。根据变量引用的对象，解释器自动确定数据类型。
2. Python是强类型语言：每个对象都有数据类型，只支持该类型支持的操作。

### 标识符

用于变量、函数、类、模块的名称。

1. 区分大小写
2. 由字母、数字、下划线组成。不能由数字开头。
3. 不能使用关键字。
4. 以双下划线开头和结尾的名称通常有特殊含义，尽量避免这种写法。

规范：模块、包名和函数名为蛇形命名，类名为驼峰且首字母大写，常量名都为大写。

### 删除变量和垃圾回收机制

可以通过 del 语句删除不再使用的变量

```python
a = 123
del a
```

如果对象没有变量引用，就会被垃圾回收器回收，清空内存空间。

### 链式赋值

```python
x = y = 123
```

### 系列解包赋值

```python
a,b,c = 4,5,6
#变量交换
a,b = b,a
```

### 常量

Python不支持常量，即没有语法规则限制一个常量的值，我们只能约定常量的命名规则，以及在程序的逻辑上不对常量的值做出修改。

### 运算符

1. / ：浮点数除法
2. //：整数除法
3. **：幂

### 三种进制

1. 二进制：0b或0B
2. 八进制：0o或0O
3. 十六进制：0x或0X

### 类型转换

1. 整数转换：int(3.14)、float(1)
2. 自动转型：整数和浮点数混合运算时，表达式结果自动转型成浮点数。
3. 整数四舍五入：round(value)

（所有的转换和运算都不会改变原有的值，而是产生新的值）