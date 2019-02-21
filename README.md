# babel-addtion-plugin


babel插件走一个
===

babel介绍
---
 Babel 是一个通用的多功能的 JavaScript 编译器。此外它还拥有众多模块可用于不同形式的**静态分析**
- 静态分析是在不需要执行代码的前提下对代码进行分析的处理过程 （执行代码的同时进行代码分析即是动态分析）。 
- 静态分析的目的是多种多样的， 它可用于语法检查，编译，代码高亮，代码转换，优化，压缩等等场景。




Tree-Shaking啊啊啊
==

资料来源

[Tree-Shaking性能优化实践 - 原理篇](https://zhuanlan.zhihu.com/p/32554436)


Tree-Shaking介绍
---
- 通过工具"摇"我们的JS文件，将其中用不到的代码"摇"掉，是一个性能优化的范畴

Tree-Shaking原理
---
### es module
- 只能作为模块顶层的语句出现
- import 的模块名只能是字符串常量
- import binding 是 immutable的
### 基础
- ES6模块依赖关系是确定的，和运行时的状态无关，可以进行可靠的静态分析，这就是tree-shaking的基础
