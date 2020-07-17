---
title: "Python第一弹  Python语言的特性和设计理念"
toc: true
comments: true
date: 2020-07-16 20:45:16
categories:
  - "Programming Language"
tags:
  - "Programming Language"
  - Python
top_image:
photos:
---

## Python的特性 ##

> Python是支持多范式编程，比如面向对象编程、结构化编程、函数式编程和面向切面编程(包括元编程和元对象).

> Python是完全面向对象的语言，函数，模块，数值，字符串都是对象，并且完全支持继承，重载，派生，多重继承，增强代码的易用性。同时支持重载运算符，范性设计。但是只对函数式编程提供了有限的支持。

> Python的设计哲学是`优雅`，`明确`,`简单`。

> Python开发者的哲学是“用一种方法，最好只有一种方法来做一件事情”。

Python的语法和那些拥有个人风格的其他的语言很不一样。Python开发者拒绝花哨的语法，选择没有或很少歧义的语法。Python拥有动态类型系统和垃圾回收功能。Python本身被设计为可扩展的。并非所有的特性和功能都集成到语言核心。Python提供了丰富的API和工具，以便程序员能够轻松地使用C、C++、Cython来编写扩展模块。Python编译器本身也可以被集成到其它需要脚本语言的程序内。因此，有很多人把Python作为一种“胶水语言”使用。


``` python
>>>import this
The Zen of Python, by Tim Peters

Beautiful is better than ugly.
Explicit is better than implicit.
Simple is better than complex.
Complex is better than complicated.
Flat is better than nested.
Sparse is better than dense.
Readability counts.
Special cases aren't special enough to break the rules.
Although practicality beats purity.
Errors should never pass silently.
Unless explicitly silenced.
In the face of ambiguity, refuse the temptation to guess.
There should be one-- and preferably only one --obvious way to do it.
Although that way may not be obvious at first unless you're Dutch.
Now is better than never.
Although never is often better than *right* now.
If the implementation is hard to explain, it's a bad idea.
If the implementation is easy to explain, it may be a good idea.
Namespaces are one honking great idea -- let's do more of those!

# 优美优于丑陋。
# 明了优于隐晦。
# 简单优于复杂。
# 复杂优于凌乱。
# 扁平优于嵌套。
# 稀疏优于稠密。
# 可读性很重要。
# 即使特例的实用性比纯粹性更优，也不可违背原则。
# 错误绝不能悄悄忽略，除非它明确需要如此。
# 面对不确定性，不要妄加猜测。
# 任何问题应有一种，且最好只有一种显而易见的解决方法。
# 尽管这并不容易，因为你不是Python之父。
# 做优于不做，然而不假思索还不如不做。
# 很难解释的，必然是坏方法。
# 很好解释的，可能是好方法。
# 命名空间是个绝妙的理念，我们应好好利用它。
```
