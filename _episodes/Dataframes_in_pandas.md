---
title: "Dataframes in Pandas"
teaching: 0
exercises: 0
questions:
- "What are Variables?"
- "How to create a Variable?"
objectives:
- "To understand variables and the rules of naming variables"
---

## What are Dataframes?

A  DataFrame is a 2 dimensional data structure. It is similar to a 2 dimensional array.

~~~
import pandas as pd

data = {
  "quantity_available": [420, 380, 390],
  "quantity_needed_for_full_inventory": [50, 40, 45]
}

#load data into a DataFrame object:
df = pd.DataFrame(data)

print(df) 
~~~


## Accessing a row element

Pandas uses the .loc attribute to return one or more specified row(s).

> NOTE: If you use loc to retrieve a single row, the result is a series. If we retrieve multiple rows, the result is a dataframe.

~~~
print(df.loc[0]) # returns single row
print(df.loc[[0, 1]]) # returns multiple rows in a dataframe
~~~
{: .language-python}

## Named Indexes

We can create custom labels by using the index argument while creating a data frame.

~~~
data = {
  "quantity_available": [420, 380, 390],
  "quantity_needed_for_full_inventory": [50, 40, 45]
}

#load data into a DataFrame object:
df_labeled = pd.DataFrame(data, index = ['Sugar', 'Salt', 'Pepper'])

print(df_labeled) 
~~~
{: .language-python}

## Accessing Rows Through Named Indexes

The loc attribute can be used to access rows with the custom labels.

~~~
print(df_labeled.loc['Sugar'])
print(df_labeled.loc[['Sugar','Salt']])
~~~


