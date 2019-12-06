# CommonJs 规范

## 概述

> Node 应用由模块组成，采用 CommonJs 模块规范

> 每一个文件就是一个模块，有自己的作用域，在一个文件里面定义的变量，函数，类，都是私有的，对其他文件不可见



## module 对象

> Node内部提供一个 Module 构建函数。 所有模块都是 Module 的实例
> 每个模块内部，都有一个 module 对象，代表当前模块， 它有以下属性

1. module.id 模块的识别符，通常是带有绝对路径的模块文件名。
2. module.filename 模块的文件名，带有绝对路径
3. module.loaded 返回一个布尔值，表示模块是否已经完成加载
4. module.parent 返回一个对象，表示调用该模块的模块。
5. moodule.children 返回一个数组，表示该模块要用到的其他模块
6. module.exports 表示模块对外输出的值。 



## ADM 规范与 Common 贵伐的兼容性

## require 命令

1. 基本用法

Node 使用 CommonJS 模块规范， 内置的 require 命硬用于加载模块文件

## 模块的加载机制

## 