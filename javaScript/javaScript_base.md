![](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1533271326897&di=8701f06e3e10ab98a71d24c8a343d290&imgtype=0&src=http%3A%2F%2Fwww.inspinovation.cn%2Fimages%2Fupload%2F20170113%2F1484321980726299.jpg)

## javaScript 基础

- 输出

```
    console.log();

    alert();
```

- 函数的声明及赋值

```
    var a = 0;  //声明并赋值

    var a = 0, b = 1, c = 2;  //定义多个

```
 
#### js数据类型

- 基本数据类型
   - Number  数字
        + NaN：是一个特殊的值，即非数值(Not a Number)。数学运算无法得到数字时，就会返回NaN
            不代表任何值，也不等于任何值，甚至自己都不等于自己
            任何数据与它运算都返回NaN
            isNaN(a)：用来判断a到底是不是非数字,返回布尔值

    - String  字符串

    - Boolean   布尔

#### 引用数据类型

- Array  数组

- Object  对象


#### 特殊数据类型

- Null
    + Null 类型是一个只有一个值的数据类型，即特殊的值 null。它表示一个空对象引用(指针)，而 typeof 操作符检测 null 会返回 object

- Undefined 
    + Undefined类型只有一个值，即特殊的 undefined，在使用 var 声明变量，但没有对其初始化时，这个变量的值就是 undefined

    + 与not defined的区别(not defined:未声明)


#### 数据类型判断

- typeof

```
    typeof 'html5'; //=>string

    typeof 100; //=>number

    typeof true //=>boolean

    typeof null //=>object
```

#### 数据类型转换

- 基本数据类型转换：利用内置函数进行转换

    |    值(a)    | 转换为   | 字符串String(a) | 数字Number(a) | 布尔值Boolean(a) |
    | :--------:  | :-----: |     :----:      |   :------:   |    :------:      |
    | undefined   |   =>    |   "undefined"   |      NaN     |       false      |
    | null        |   =>    |   "null"        |      0       |      false       |
    | true        |    =>   |     "true"      |       1      |                  |
    | false       |    =>   |     "false"     |       0      |                  |
    | ""          |    =>   |                 |       0      |    false         |
    | "1.2        |    =>   |                 |       1.2    |       true       |
    | "one"       |    =>   |                 |     NaN      |        true      |
    | 0           |    =>   |     "0"         |              |        false     |
    | -0          |    =>   |     "0"         |              |   false          |
    | NaN         |    =>   |     "NaN"       |              |   false          |
    |  1          |    =>   |      "1"        |              |    true          |

    + 隐式转换
        + 如果运算不能进行下去，内部就会尝试进行数据类型的转换
支持隐式转换的运算：逻辑运算、关系运算、算术运算

#### 算术运算

- +, -, *, /, %:加,减,乘,除,取余(取模)

    - toFixed(num): 在数字后面调用，num为小数位，有四舍五入的功能，得到一个字符串

    - parseInt()：取整

    - parseFloat()：取小数


#### 赋值操作

- =
    - var num1=10;//表示把10赋值给num1变量

- +=：在原来的内容基础上追加内容
    - str += 'test' <==> str = str + 'test'

- -=
    - var n=10; n -= 2 <==> n = n - 2

- *=,/=,%=
    - 
    - 上同


#### 关系运算（返回布尔值）
- ==(等于), !=(不等于)
- <(小于)、>(大于)、<=(小于等于)、>=(大于等于)
- ===、恒等于/全等于，比较的时候要求值和类型都相等（不会进行类型隐式转换）
- !==、不全等于
- 关系运算符的比较规则: 
    - 1 数字和数字比较, 直接比较大小
    - 2 数字和字符串比较, 字符串转换为数字后再比较
    - 3 字符串和字符串比较, 进行字符的ASCII码值比较
