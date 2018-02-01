# BFC
参考链接：https://zhuanlan.zhihu.com/p/25321647

### 什么是BFC？
英文原意:Block Formatting Context
中文意思：块级格式化上下文。具有BFC特性的元素可以看做一个隔离容器，容器里面的元素不会在布局上影响外面的元素。

### 触发BFC的条件？
- 1.body根元素
- 2.浮动元素：float 除none以外的值(脱离文档流)
- 3.绝对定位： position(absolute,fixed)(脱离文档流)
- 4.display为inline-block(脱离文档流)，flex(标准文档流)
- 5.overflow除了visible以外的值(hidden,auto,scroll)

### BFC的特性？
1.同一个BFC下外边距会发生重叠
2.BFC可以包含浮动元素(清除浮动)
3.BFC 可以阻止元素被浮动元素覆盖
