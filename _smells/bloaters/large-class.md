---
layout: smell
group: Bloaters
title: Large Class
image: largeClass.png
---
Large Classes are classes that span too many lines. When a class gets too long, perhaps it is responsible for more tasks than it should be, or could be further generalised and additional classes that inherit from it can implement more specific features.

~~~ python
class LargeClass:
    # Many class variables

    def __init__(self):
        # Many instance variables

    # Many Methods
~~~
