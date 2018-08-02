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

    |    值(a)    | 转换为   |  字符串String(a)  | 数字Number(a)| 布尔值Boolean(a) |
    | :--------:  | :-----:  | :----:  |  :------: |  :------: |
    | undefined   | =>   |   "undefined"     |      NaN       |       false       |
    | null        |   =>   |   "null"   |      0        |        false           |
    | true        |    =>   |  "true"  |       1       |               |