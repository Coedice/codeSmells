---
layout: smell
group: Bloaters
title: Long Method
image: longMethod.png
---
Long Methods are methods that span too many lines. When a method gets too long, perhaps it is responsible for more tasks than it should be.
## Example
{% highlight python linenos %}
def long(self):
    # Do first thing
    ⋮
    
    # Do second thing
    ⋮
    
    # Do third thing
    ⋮
{% endhighlight %}