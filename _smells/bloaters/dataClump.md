---
layout: smell
group: Bloaters
title: Data Clump
image: dataClump.png
---
Data clumps are sets of related primitives (eg. `1`, `3.14`, `"Hello"`, `False`) that always appear together. Data Clumps can be avoided by with encapsulating them together in a class.
~~~ python
x_coordinate = 4
y_coordinate = -7
z_coordinate = 43

print(distance(x_coordinate, y_coordinate, z_coordinate))
~~~
The problem with Data Clumps, is that it is not easy to centrally control their behaviour. In the above example, if we wanted to restrict `y` coordinates to positive numbers only, we may need to edit the code in many places, leading to [Shotgun Surgery](../changePreventers/shotgunSurgery).

Data Clumps are also often [Primitive Obsessions](primitiveObsession).