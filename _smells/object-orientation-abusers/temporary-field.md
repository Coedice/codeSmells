---
layout: smell
group: Object-Orientation Abusers
title: Temporary Field
image: temporaryField.png
---
A Temporary Field smell occurs when a variable that should be defined within a method's scope is instead defined in the class' scope.

This violates the information hiding principle, since all the methods in the class will have access to this variable, when only one method needs it.

Another issue this smell causes, is the unreliability of instance variables, since this instance variable would only be updated when the method is run, but we expect instance variables to reliably track information about our objects at all times.
