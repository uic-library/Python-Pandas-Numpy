---
title: "Pandas Series"
teaching: 0
exercises: 0
questions:
- "What are Variables?"
- "How to create a Variable?"
objectives:
- "To understand variables and the rules of naming variables"
---

## What is a Series?

It is a one-dimensional array holding data of any type. It is similar to a column in a table.

~~~

import pandas as pd

quantity = [10, 20, 30]

quantity_series = pd.Series(quantity)

print(quantity_series)
~~~
{: .language-python}


## Labels

By default the values are labeled with their index number. These labels can then be used to access the elements. 
For example: The first element of the series is accessed by quantity_series[0].

## Custom Labels

We can index the elemts in the series with our own labels.

~~~


quantity = [10, 20, 30]

quantity_series = pd.Series(quantity, index = ["Sugar", "Salt", "Pepper"])

print(quantity_series["Sugar"])
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

## Key/Value Objects in a Series
Objects that follow key:value format(Dictionaries) can also be used to create series. The key becomes the index and the value becomes the column element.

~~~

pantry={'eggs':10,'butter(tbsp)':20,'sugar(oz)':30,'salt(oz)':40}

pantry_series = pd.Series(pantry)
print(pantry_series)
pantry_series_slice = pd.Series(pantry, index = ['eggs', 'butter(tbsp)'])
print(pantry_series_slice)
~~~
{: .language-python}

