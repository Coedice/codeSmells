---
layout: smell
group: Bloaters
title: Primitive Obsession
image: primitiveObsession.png
---
Primitive Obsession is the overuse of primitives, rather than classes that make use of those primitives. When this data is used or manipulated, this must be done in another class' method.
## Example
    # Primitive Obsession
    dollars = 28.27
    cents = int(dollars * 100 % 100)
    print(cents)

    # Improvement
    class Money():
        def __init__(self, dollars):
            self.dollars = dollars
        
        def get_cents(self):
            return int(self.dollars * 100 % 100)

    dollars = Money(28.27)
    cents = dollars.get_cents()
    print(cents)
        