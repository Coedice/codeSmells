---
layout: smell
group: Bloaters
title: Primitive Obsession
image: primitiveObsession.png
---
Primitive Obsessions are the overuse of primitives (eg. `1`, `3.14`, `"Hello"`, `False`), rather than classes that make use of those primitives.
~~~ python
# Primitive Obsession
dollars = 28.27
cents = int(dollars * 100 % 100)
print(cents)

# Improvement
class Money():
    def __init__(self, dollars):
        self.dollars = dollars
    
    def get_cents(self):
        return int(self.dollars * 100 % 100)

dollars = Money(28.27)
cents = dollars.get_cents()
print(cents)
~~~
The issue that this causes is that common functionality that uses this data must be coded in different places in the codebase, and is not tied to the data itself.

A Primitive Obsession is often a result of the programmer's desire not to create a small class, but having small classes is not itself a bad thing.

Primitive Obsessions are also often [Data Clumps](dataClump).