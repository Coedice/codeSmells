---
layout: smell
group: Change Preventers
title: Parallel Inheritance Hierarchies
image: parallelInheritanceHierarchies.png
---
Long Methods are methods that span too many lines. When a method gets too long, perhaps it is responsible for more tasks than it should be.
## Example
    def longMethod(self):
        # Do first thing
        ⋮
        
        # Do second thing
        ⋮
        
        # Do third thing
        ⋮