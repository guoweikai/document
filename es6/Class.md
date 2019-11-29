# Class 的基本语法

> 1. 简介
> 2. 静态方法
> 3. 实例属性的新方法
> 4. 静态属性
> 5. 私有方法和属性
> 6.  new.target 属性

## 简介

*** 

### constructor 方法

> constructor 方法是类的默认方法，通过 new 命令生成对象实例时，自动调用该方法
一个类必须有 constructor 方法， 如果没有显式定义,一个空的 constructor 方法会被默认添加。

```
class Point {

}
//等同于

class Point {
  constructor (){}
}

```
> 上面代码中,定义了一个空的类 Point, JS 引擎会自动为它添加一个空的 constructor 方法.

>constructor 方法默认返回实例对象(即this),完全可以指定返回另外一个对象

> constructor 函数返回一个全新的对象,结果导致实例对象不是 Foo 类的实例

> 类必须使用 new 调用,否则会报错,这是它跟普通构造函数的一个主要区别,后者不用 new 也可以执行 

### 类的实例

>与 ES5 一样,实例的属性除非显式定义在其本身,否则都是定义在原型上(即定义在 class)

