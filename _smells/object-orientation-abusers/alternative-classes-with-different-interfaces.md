---
layout: smell
group: Object-Orientation Abusers
title: Alternative Classes with Different Interfaces
image: alternativeClassesWithDifferentInterfaces.png
---
When closely related classes lack a common interface, this is an Alternative Classes with Different Interfaces smell.

Reducing this will increase the legibility and understandability of the code. To do this, you could rename public methods and modify code parameters to be the same, create a superclass above both classes, and remove any [Dead Code](../dispensables/dead-code) smells.