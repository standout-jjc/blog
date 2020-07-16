---
title: "Python第二弹  Python关键字和操作符"
toc: true
comments: true
date: 2020-07-16 20:45:16
categories:
  - "Programming Language"
tags:
  - Python
top_image:
photos:
---

## Python的关键字 ##

``` python

>>>import keyword
>>>keyword.kwlist
['False', 'None', 'True', 'and', 'as', 'assert', 'async', 'await', 'break', 'class', 'continue', 'def', 'del', 'elif', 'else', 'except', 'finally', 'for', 'from','global', 'if', 'import', 'in', 'is', 'lambda', 'nonlocal', 'not', 'or', 'pass', 'raise', 'return', 'try', 'while', 'with', 'yield']
```
## Python的操作符 ##

``` python

>>>import operator
>>> print(operator.abs.__doc__)
Same as abs(a).
>>> print(operator.imatmul.__doc__)
Same as a @= b.
>>> print(operator.lshift.__doc__)
Same as a << b.
>>> print(operator.add.__doc__)
Same as a + b.
>>> print(operator.imod.__doc__)
Same as a %= b.
>>> print(operator.lt.__doc__)
Same as a < b.
>>> print(operator.and_.__doc__)
Same as a & b.
>>> print(operator.imul.__doc__)
Same as a *= b.
>>> print(operator.matmul.__doc__)
Same as a @ b.
>>> print(operator.attrgetter.__doc__)
attrgetter(attr, ...) --> attrgetter object

Return a callable object that fetches the given attribute(s) from its operand.
After f = attrgetter('name'), the call f(r) returns r.name.
After g = attrgetter('name', 'date'), the call g(r) returns (r.name, r.date).
After h = attrgetter('name.first', 'name.last'), the call h(r) returns
(r.name.first, r.name.last).
>>> print(operator.index.__doc__)
Same as a.__index__()
>>> print(operator.methodcaller.__doc__)
methodcaller(name, ...) --> methodcaller object

Return a callable object that calls the given method on its operand.
After f = methodcaller('name'), the call f(r) returns r.name().
After g = methodcaller('name', 'date', foo=1), the call g(r) returns
r.name('date', foo=1).
>>> print(operator.concat.__doc__)
Same as a + b, for a and b sequences.
>>> print(operator.indexOf.__doc__)
Return the first index of b in a.
>>> print(operator.mod.__doc__)
Same as a % b.
>>> print(operator.contains.__doc__)
Same as b in a (note reversed operands).
>>> print(operator.inv.__doc__)
Same as ~a.
>>> print(operator.mul.__doc__)
Same as a * b.
>>> print(operator.countOf.__doc__)
Return the number of times b occurs in a.
>>> print(operator.invert.__doc__)
Same as ~a.
>>> print(operator.ne.__doc__)
Same as a != b.
>>> print(operator.delitem.__doc__)
Same as del a[b].
>>> print(operator.ior.__doc__)
Same as a |= b.
>>> print(operator.neg.__doc__)
Same as -a.
>>> print(operator.eq.__doc__)
Same as a == b.
>>> print(operator.ipow.__doc__)
Same as a **= b.
>>> print(operator.not_.__doc__)
Same as not a.
>>> print(operator.floordiv.__doc__)
Same as a // b.
>>> print(operator.irshift.__doc__)
Same as a >>= b.
>>> print(operator.or_.__doc__)
Same as a | b.
>>> print(operator.ge.__doc__)
Same as a >= b.
>>> print(operator.is_.__doc__)
Same as a is b.
>>> print(operator.pos.__doc__)
Same as +a.
>>> print(operator.getitem.__doc__)
Same as a[b].
>>> print(operator.is_not.__doc__)
Same as a is not b.
>>> print(operator.pow.__doc__)
Same as a ** b.
>>> print(operator.gt.__doc__)
Same as a > b.
>>> print(operator.isub.__doc__)
Same as a -= b.
>>> print(operator.rshift.__doc__)
Same as a >> b.
>>> print(operator.iadd.__doc__)
Same as a += b.
>>> print(operator.itemgetter.__doc__)
itemgetter(item, ...) --> itemgetter object

Return a callable object that fetches the given item(s) from its operand.
After f = itemgetter(2), the call f(r) returns r[2].
After g = itemgetter(2, 5, 3), the call g(r) returns (r[2], r[5], r[3])
>>> print(operator.setitem.__doc__)
Same as a[b] = c.
>>> print(operator.iand.__doc__)
Same as a &= b.
>>> print(operator.itruediv.__doc__)
Same as a /= b.
>>> print(operator.sub.__doc__)
Same as a - b.
>>> print(operator.iconcat.__doc__)
Same as a += b, for a and b sequences.
>>> print(operator.ixor.__doc__)
Same as a ^= b.
>>> print(operator.truediv.__doc__)
Same as a / b.
>>> print(operator.ifloordiv.__doc__)
Same as a //= b.
>>> print(operator.le.__doc__)
Same as a <= b.
>>> print(operator.truth.__doc__)
Return True if a is true, False otherwise.
>>> print(operator.ilshift.__doc__)
Same as a <<= b.
>>> print(operator.length_hint.__doc__)
Return an estimate of the number of items in obj.

This is useful for presizing containers when building from an iterable.

If the object supports len(), the result will be exact.
Otherwise, it may over- or under-estimate by an arbitrary amount.
The result will be an integer >= 0.
>>> print(operator.xor.__doc__)
Same as a ^ b.

```

