---
layout: smell
group: Change Preventers
title: Parallel Inheritance Hierarchies
image: parallelInheritanceHierarchies.png
---
Parallel Inheritance Hierarchy smells occur when subclasses of class A must be linked to subclasses of class B.
~~~ python
# Parent classes
class Dinosaur:
    # Dinosaur code

class Egg:
    # Egg code

# Child classes with Parallel Inheritance Hierarchy smell
class Velociraptor(Dinosaur):
    # Velociraptor code

class VelociraptorEgg(Egg)
    # VelociraptorEgg code
~~~
There are three main issues caused by Parallel Inheritance Hierarchy smells: If you want to add a new class, you will need to create two every time, changes in one class may require changes in the other, and it is generally harder to maintain the code and avoid bugs.

There are different ways to remove this code smell, and which one you choose will depend on your exact case. One way is to only have one hierarchy with implements details for both the dinosaur, and its egg. Another way is to reduce one of the hierarchies into a single class, such as an Egg class that contains objects that are subclasses of Dinosaur.