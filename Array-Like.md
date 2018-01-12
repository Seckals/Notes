# Array-Like
参考链接：http://2ality.com/2013/05/quirk-array-like-objects.html

## 什么是Array-Like对象呢？。
An array-like object
- has: indexed access to elements and the property length that tells us how many elements the object has.
- does not have: array methods such as push, forEach and indexOf.

## 哪些又是Array-Like对象呢？
- the result of the DOM method document.getElementsByClassName() (many DOM methods return array-like objects)
- the special variable arguments

## Array-Like 转 Array
1. 比较简单的方法就是新建一个新数组，循环往新的数组中添加，替换原Array-Like对象
2. Array.prototype.slice.call(nodes) 
