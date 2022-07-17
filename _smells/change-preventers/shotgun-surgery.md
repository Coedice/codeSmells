---
layout: smell
group: Change Preventers
title: Shotgun Surgery
image: shotgunSurgery.png
---
Shotgun Surgery smells occur when a single change requires edits in many classes.

The consequence of this is that you can easily cause errors whenever a change is made that outside classes do not expect, limiting how quickly you can make changes to the code.

The aim should be that code changes and classes have a one-to-one relationship (each change affects only one class). Shotgun Surgery smells are one-to-many (one change affects many classes).

Shotgun Surgery is the opposite of [Divergent Change](divergent-change).