Deep copy VS Shallow copy
-------------------------

**Shallow**

![shallow copy](https://upload.wikimedia.org/wikipedia/en/thumb/e/e1/Shallow_copy_done.svg/120px-Shallow_copy_done.svg.png "Shallow copy")
![shallow copy](https://upload.wikimedia.org/wikipedia/en/thumb/3/3e/Shallow_copy_in_progress.svg/120px-Shallow_copy_in_progress.svg.png "Shallow copy")
![shallow copy](https://upload.wikimedia.org/wikipedia/en/thumb/e/e1/Shallow_copy_done.svg/120px-Shallow_copy_done.svg.png "Shallow copy")

The variables A and B refer to different areas of memory, when B is assigned to A the two variables refer to the same area of memory. Later modifications to the contents of either are instantly reflected in the contents of other, as they share contents.

**Deep**

![deep copy](https://upload.wikimedia.org/wikipedia/en/thumb/5/5f/Deep_copy_in_progress.svg/120px-Deep_copy_in_progress.svg.png "Deep Copy")
![deep copy](https://upload.wikimedia.org/wikipedia/en/thumb/5/5f/Deep_copy_in_progress.svg/120px-Deep_copy_in_progress.svg.png "Deep Copy")
![deep copy](https://upload.wikimedia.org/wikipedia/en/thumb/0/00/Deep_copy_done.svg/120px-Deep_copy_done.svg.png "Deep Copy")

The variables A and B refer to different areas of memory, when B is assigned to A the values in the memory area which A points to are copied into the memory area to which B points. Later modifications to the contents of either remain unique to A or B; the contents are not shared.
