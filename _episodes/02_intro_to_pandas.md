---
title: "Introduction and Installation of Pandas"

---

## What is Pandas?

Pandas is a Python library used for working with data sets. It has functions for analyzing, cleaning, exploring, and manipulating data.
Pandas allows us to analyze big data and make conclusions based on statistical theories.Pandas can clean messy data sets, and make them readable and relevant.

## Examples of questions answered by Pandas?

* Is there a correlation between two or more columns?
* What is average value?
* Max value?
* Min value?

## How to install Pandas?
Pandas can be installed by simply typing the command - __"pip install pandas"__ on your terminal on in jupyter notebook

## How to use Pandas?
To use pandas, we need to import it first. This can be done by typing the following line - "import pandas"

~~~
import pandas

stock_dict = {
  'Items': ["Sugar", "Salt", "Pepper"],
  'Qunatity(Kgs)': [10, 20, 5]
}

stock_df = pandas.DataFrame(stock_dict)

print(stock_df)
~~~
{: .language-python}
