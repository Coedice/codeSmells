---
layout: smell
group: Dispensables
title: Duplicate Code
image: duplicateCode.png
---
A Duplicate Code smell represents code in multiple places that is the same or very similar.

If the functionality of some code is shared, there is a good chance that the purpose is also shared, and so the functionality should be implemented in one place and then reused where it is required.

To combine the duplicated code, a superclass may be appropriate, or an additional third class may be the best solution. Where functionality is similar but not the same, generalising the code may be necessary in the new unified code.

Having the same or similar code in multiple places can also lead to [Shotgun Surgery](../change-preventers/shotgun-surgery).