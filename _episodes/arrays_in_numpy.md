---
title: "arrays_in_numpy"
teaching: 0
exercises: 0
questions:
- "What are Variables?"
- "How to create a Variable?"
objectives:
- "To understand variables and the rules of naming variables"
---

## Create a NumPy ndarray Object
We can create a NumPy ndarray object by using the array() function.

~~~
import numpy as np

arr = np.array([1, 2, 3, 4, 5])

print(arr)

print(type(arr))
~~~
{: .language-python}

## How to create a Variable?

A variable is created the moment you assign a value to it.

~~~

name = "Recipe for pancakes"
no_of_ingredients = 5
print(no_of_ingredients)
print(name)
~~~
{: .language-python}


## Dimensions in Arrays

A dimension in arrays is the level of array depth (nested arrays).

### 0-D Arrays
0-D arrays, or Scalars, are the elements in an array. Each value in an array is a 0-D array.
~~~
import numpy as np

arr = np.array(42)

print(arr)
~~~
{: .language-python}

### 1-D Arrays
An array that has 0-D arrays as its elements is called uni-dimensional or 1-D array.

~~~
import numpy as np

arr = np.array([1, 2, 3, 4, 5])

print(arr)
~~~
{: .language-python}

### 2-D Arrays
An array that has 1-D arrays as its elements is called a 2-D array.These are often used to represent matrix or 2nd order tensors.
 ~~~
 import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6]])

print(arr)
 ~~~
{: .language-python}

### 3-D arrays
An array that has 2-D arrays (matrices) as its elements is called 3-D array.These are often used to represent a 3rd order tensor.
~~~
import numpy as np

arr = np.array([[[1, 2, 3], [4, 5, 6]], [[1, 2, 3], [4, 5, 6]]])

print(arr)
~~~
{: .language-python}

## Higher Dimensional Arrays

We can create higher dimension arrays by using the ndmin argument.

~~~
import numpy as np

arr = np.array([1, 2, 3, 4], ndmin=5)

print(arr)
print('number of dimensions :', arr.ndim)
~~~
{: .language-python}

## Find the dimension of the Array

To find the number of dimensions of an array, we can print the ndim attribute of that array.

~~~
print(arr.ndim)
~~~
{: .language-python}
