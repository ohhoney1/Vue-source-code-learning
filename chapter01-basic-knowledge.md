
## Object.defineProperty

> 引用自[MDN`Object.defineProperty()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/defineProperty)。 可以定义一个对象的新属性，也可以修改一个对象属性，返回值都是当前对象。

### Syntax

`Object.defineProperty(obj, prop, descriptor)`

+ `obj` 目标对象
+ `prop` 要定义的或要更改的对象属性
+ `descriptor` 要定义的或要更改的对象属性的descriptor
+ 返回值 目标对象

### Description

分为`data descriptor` and `accessor descriptor`两种描述方式。键值keys如下：

+ `configurable`： 两种方式共有，默认为`false`。当为`true`时，该属性方可被更改或删除
+ `enumerble`： 两种方式共有，默认为`false`。当为`true`是，该属性可枚举，例如`for...in`或`Object.keys()`
+ `value`： （数据描述符），默认为`undefined`。该属性的值。
+ `writable`： （数据描述符），默认为`undefined`。当为`true`时，该属性可以进行赋值运算
+ `get`： （存储描述符），默认为`undefined`。该属性的getter方法，依赖于setter
+ `set`： （存储描述符），默认为`undefined`。该属性的setter方法，依赖于getter，接收参数且唯一，并赋值给该属性，以便后续操作

