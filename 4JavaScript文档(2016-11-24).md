﻿# JavaScript文档(2016/11/24)

标签（空格分隔）： 前端 js

---

> 这里会有连着三天的文档内容，是书上的35页~59页的内容。我会把这三天的内容都写在这片文档里。内容也会比较粗略一点，这部分还是平时注意起来有用吧。空余的时间，这两天需要做出一个web端图片剪裁的demo,也会接触到一些新的东西。

---

> 所谓代码的可维护性，值得是不管团队规模多大，大家都能在一个文档集合上展开合作，知道该如何对待吗进行添加、修改或者删除且同时保证最终结果的一致性。

---

### **结构化的JavaScript文档**
> 最好将说明和示例直接放在源文件本身的块级注释中，这样可以最大可能的保持文档和代码的一致性。

- 下面就是一些能够从源代码中提取特殊格式的文档的工具
    - [JSDoc][1]
    - [dox][2]
    - [YUIDoc][3]

### **YUIDoc文档格式**
- **YUIDoc**只读取文件中的**块级注释**
```javascript
/**
*这一行将被读取
*/

/**
*一个用于定义各种类型住宅（accommodation）的类
*
*@class Accommodation
*@constructor
*/

/**
*表示住宅当前是否上锁
*
*@property
*/

/**
*为住宅解锁
*
*@method unlock
*/
```
- [官方语法指南][4]
    
### **使用YUIDoc创建一个文档网站**
- 下载使用**YUIDoc**,它是基于nodejs的
```javascript
//下载
npm install -g yuidocjs

//执行,扫描当前目录和所有子目录
yuidoc .

//只扫描当前目录
yuidoc -n .
```
### **Markdown,更具表达性**
- [文档][5]
    - 直接百度就可以找到常用的语法，足够使用了


  [1]: http://usejsdoc.org/
  [2]: https://github.com/tj/dox
  [3]: http://yui.github.io/yuidoc/
  [4]: http://yui.github.io/yuidoc/syntax
  [5]: http://daringfireball.net/projects/markdown