---
title: "Indexing and slicing Arrays"
teaching: 0
exercises: 0
questions:
- "What are Variables?"
- "How to create a Variable?"
objectives:
- "To understand variables and the rules of naming variables"
---

## Access Array Elements

Array indexing is the same as accessing an array element.You can access an array element by referring to its index number.The indexes in NumPy arrays start with 0, meaning that the first element has index 0, and the second has index 1 etc.

~~~
import numpy as np

arr = np.array([1, 2, 3, 4])

print(arr[0])
~~~
{: .language-python}


## Access 2-D Arrays

To access elements from 2-D arrays we can use comma separated integers representing the dimension and the index of the element.

~~~

import numpy as np

arr = np.array([[1,2,3,4,5], [6,7,8,9,10]])

print('2nd element on 1st row: ', arr[0, 1])
~~~
{: .language-python}

In python, we can also change the values assigned to the variables, without any restrictions.

~~~
no_of_ingredients = "Recipe for pancakes"    # x is now of type string
name = 5                       # name is now of type int
print(x)
print(name)
~~~
{: .language-python}

## Slicing arrays

Slicing in python means taking elements from one given index to another given index.

We pass slice instead of index like this: [start:end].

We can also define the step, like this: [start:end:step].

~~~
import numpy as np

arr = np.array([1, 2, 3, 4, 5, 6, 7])

arr2 = np.array([[1, 2, 3, 4, 5], [6, 7, 8, 9, 10]])
print(arr[1:5]) # Slice elements from index 1 to index 5
print(arr[4:]) # Slice elements from index 4 to the end of the array
print(arr[:4]) # Slice elements from the beginning to index 4 (not included)
print(arr[-3:-1]) # Slice from the index 3 from the end to index 1 from the end
print(arr[1:5:2]) # Return every other element from index 1 to index 5
print(arr2[1, 1:4]) # From the second element, slice elements from index 1 to index 4 (not included)
print(arr2[0:2, 1:4]) # From both elements, slice index 1 to index 4 (not included)
~~~
{: .language-python}


