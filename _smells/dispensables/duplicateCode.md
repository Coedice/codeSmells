---
layout: smell
group: Dispensables
title: Duplicate Code
image: duplicateCode.png
---
Data clumps are sets of related primitives that always appear together. Data clubs should instead be encapsulated in a class.
## Example
~~~ python
x_coordinate = 4
y_coordinate = -7
z_coordinate = 43

print(distance(x_coordinate, y_coordinate, z_coordinate))
~~~