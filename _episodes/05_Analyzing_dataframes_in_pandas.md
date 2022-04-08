---
title: "Working with Dataframes using functions in Pandas"

---

## View the Data?

The head and tail methods are used to access few rows in the data frame. The head() method returns rows from the beginning of the dataframe. 
The tail() returns rows from the ending of the data frame. The default number of rows returned is 5 rows. We can change the number of rows returned by passing the reuired number to the function as an argumet.

~~~
data = {
  "quantity_available": [5, 10, 15, 20, 25, 30, 35, 12, 10, 10, 25, 15],
  "quantity_needed_for_full_inventory": [50, 40, 45, 60, 60, 80, 100, 50, 25, 50, 50, 30],
  "Name_of_item":['Sugar','Salt','Pepper','Butter','Flour','Baking Powder','eggs','Blue Cheese', 'Panko', 'Maple Syrup', 'Strawberry Preserve', 'Honey']
}

#load data into a DataFrame object:
df = pd.DataFrame(data)

print(df.head())
print(df.tail())

print(df.head(10))
print(df.tail(10))

~~~
{: .language-python}


## Info()

Pandas library provides a methos called info(), which works on data frame objects. This function is used to et information regarding the data frame.

~~~
print(df.info())
~~~
{: .language-python}


### interpreting the result

The first two lines - i.e RangeIndex and Data columns tells us the number of rows(RangeIndex) and numbr of columns(Data columns)

Next, there is a table displayed. 
The "Column" column contains the names of the columns. 

The "Non-Null Count" tells us the number of columns that are not null(contains a value).

The "Dtype" column describes the data type of the values in the column.


