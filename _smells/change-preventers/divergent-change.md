---
layout: smell
group: Change Preventers
title: Divergent Change
image: divergentChange.png
---
Divergent Change smells occur when a single class needs to be edited many times when changes are made outside the class.
~~~ python
class Fish:
    def __init__(self, id, aquarium):
        self.name = aquarium.get_fish_name(id)  # Overly reliant on aquarium's method
~~~
The consequence of this is that you can easily cause errors whenever a change is made that the class does not expect, limiting how quickly you can make changes to the code.

The aim should be that changes and classes should have a one-to-one relationship (each change affects only one class). Divergent Change smells are many-to-one (many changes affect one class).

In principle, a class should be self-sufficient. It should not need outside code to work in a particular way.

Divergent Change is the opposite of [Shotgun Surgery](shotgun-surgery).