---
layout: smell
group: Dispensables
title: Dead Code
image: deadCode.png
---
A Dead Code smell occurs when code is not used, be it a variable, method, class, or parameter.

This code smell is often created when code has become obsolete, and so is not instantiated, called, initialised, etc.

The offending code causes codebase clutter, and may cause confusion later on in development, slowing development.

To fix this code smell, such code should be deleted. Offending code can be easily found using most IDEs.
