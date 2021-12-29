---
layout: smell
group: Bloaters
title: Long Parameter List
image: longParameterList.png
---
Long Parameter Lists are methods that have many arguments (parameters). This could be a sign that the method is responsible for too many tasks, or that the input data is poorly organised.
~~~ python
def long_parameter_list(self, arg_1, arg_2, arg_3, arg_4, arg_5, arg_6):
    pass
~~~