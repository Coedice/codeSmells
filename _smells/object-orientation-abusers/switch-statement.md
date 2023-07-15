---
layout: smell
group: Object-Orientation Abusers
title: Switch Statement
image: switchStatement.png
---
A Switch Statement code smell occurs whenever a `switch` statement is used. If instead of an actual `switch` statement, an `if ... else if` statement is used, this is still a Switch Statement code smell.

`Switch` statements can be considered good design in a procedural programming paradigm, but in Object-oriented programming, `switch` statements are a sign that the inheritance hierarchy is bad, or under-used.

~~~ python
# Smelly code
class Vehicle:
    def __init__(name):
        self.name = name

if vehicle.name == "Car":
    print(4)
elif vehicle.name == "Motorbike":
    print(2)
elif vehicle.name == "Tricycle":
    print(3)
else:
    print("Unknown")

# Improved
class Vehicle:
    def __init__():
        self.tyres = None
    
    def get_tyres():
        return self.tyres

class Car:
    def __init__():
        super()
        self.tyres = 4

class Motorbike:
    def __init__():
        super()
        self.tyres = 2

class Tricycle:
    def __init__():
        super()
        self.tyres = 3

print(vehicle.get_tyres())
~~~
