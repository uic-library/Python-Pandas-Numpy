---
title: "Important attributes in Numpy"
teaching: 0
exercises: 0
questions:
- "What are Variables?"
- "How to create a Variable?"
objectives:
- "To understand variables and the rules of naming variables"
---

## Shape of an Array

The shape of an array is the number of elements in each dimension.

~~~

import numpy as np

arr = np.array([[1, 2, 3, 4], [5, 6, 7, 8]])

print(arr.shape)
~~~
{: .language-python}


## Reshaping arrays
Reshaping means changing the shape of an array.

By reshaping we can add or remove dimensions or change number of elements in each dimension.

### Reshape From 1-D to 2-D
~~~
import numpy as np

arr = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12])

newarr = arr.reshape(4, 3)

print(newarr)
~~~
{: .language-python}

### Reshape From 1-D to 3-D
~~~
import numpy as np

arr = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12])

newarr = arr.reshape(2, 3, 2)

print(newarr)
~~~
{: .language-python}

> NOTE: We can Reshape Into any Shape, as long as the elements required for reshaping are equal in both shapes.

## Flattening the arrays
Flattening array means converting a multidimensional array into a 1D array.

We can use reshape(-1) to do this.
~~~
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6]])

newarr = arr.reshape(-1)

print(newarr)
~~~
{: .language-python}

## Joining NumPy Arrays
Joining means putting contents of two or more arrays in a single array.We pass a sequence of arrays that we want to join to the concatenate() function, along with the axis. If axis is not explicitly passed, it is taken as 0.
~~~
import numpy as np

arr1 = np.array([1, 2, 3])

arr2 = np.array([4, 5, 6])

arr = np.concatenate((arr1, arr2))

print(arr)

arr1 = np.array([[1, 2], [3, 4]])

arr2 = np.array([[5, 6], [7, 8]])

arr = np.concatenate((arr1, arr2), axis=1)
print(arr)
~~~
{: .language-python}

## Splitting NumPy Arrays
Splitting is reverse operation of Joining. We use array_split() for splitting arrays, we pass it the array we want to split and the number of splits.
~~~
import numpy as np

arr = np.array([1, 2, 3, 4, 5, 6])

newarr = np.array_split(arr, 3)

print(newarr)
~~~
{: .language-python}

## Searching Arrays
You can search an array for a certain value, and return the indexes that get a match.

To search an array, use the where() method.

~~~
import numpy as np

arr = np.array([1, 2, 3, 4, 5, 4, 4])

x = np.where(arr == 4)

print(x)
~~~
{: .language-python}

## Sorting Arrays
Sorting means putting elements in an ordered sequence.

Ordered sequence is any sequence that has an order corresponding to elements, like numeric or alphabetical, ascending or descending.

The NumPy ndarray object has a function called sort(), that will sort a specified array.

~~~
import numpy as np

arr = np.array([3, 2, 0, 1])

print(np.sort(arr))
~~~
{: .language-python}
