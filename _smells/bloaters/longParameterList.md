---
layout: smell
group: Bloaters
title: Long Parameter List
image: longParameterList.png
---
Long Parameter Lists are methods that have many arguments. This could be a sign that the method is responsible for too many tasks, or that the input data is poorly organised.
## Example
~~~ python
def long(self, …):
    ⋮
~~~