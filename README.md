# PA-3_ECE2112P

# Programming-Assignment-3

## In the given Programming Assignment we were tasked to create a code using pandas

# In the first part of the assignment we were tasked to:
### - Load the corresponding .csv file into a data frame named cars using pandas.
### - Display the the first five and last five rows of the resulting cars. 

# #3.1 Load the correspoding .cvs file into a data frame named cars using pandas.

In order to do this task first is to input:

`import pandas as pd`

So that we would be able to use the different syntaxes that it offers.

Then using the code:

`pd.read_csv('cars.csv')`

This would put the .csv file into a data frame in order to extracts its elements.

# #3.1 Display the first five and last five rows of the resulting pandas. 

In order to perform the task we would need to utilize the code:

`.head() and .tail()`

Using the code `cars.head(10)` I was able to extract the first 10 rows of the given data frame.

Then using the code `cars.tail(10)` I was able to extract, starting from the last row, the 10 last rows of the given data frame.

## What I learned

I learned that if I want to extract the data of a .csv file then I would need to use the code .read_csv("name of the .csv"). And in order for me to extract either the first couple or last couple of rows, I would need to use the code .head("number of rows from the first row") and .tail("number of rows from the last row") in order to output the specific amount of rows that I want. 

# In the second part of the assignment we were tasked to:
## - Display the first five rows  with odd numbered columns in the given data frame cars
## - Display the row that contains the 'Model' of 'Mazda RX4'
## - Determine how many cylinders ('cyl') does the car model 'CamaroZ28' have
## - Determine how many cylinders ('cyl') and what gear type ('gear') do the car models 'Mazda RX4 Wag', 'Ford Pantera L', and 'Honda Civic' have.

# #3.2a Display the first five rows with odd numbered columns in the given data frame 'cars'

In order to do this task I used the code:

## .iloc()

So that I would be able to input the specific indexes that I want to output. Simply inputing the code:

`cars.iloc[:5,1::2]`

This would output display the first five rows with odd numbered columns as the indexing works like `[row,column,increment]` it is coded to start from the first row to the fifth, then it would start from the 1st index column, with an increment of 2 so that it would only output the odd numbered columns.

# 3.2b Display the row that contains the ‘Model’ of ‘Mazda RX4’.

For this code I used:

`cars.loc[cars['Model']=='Mazda RX4']`

In which it would try to locate the 'Model' Mazda RX4 and ouput its row.

# 3.2c How many cylinders (‘cyl’) does the car model ‘Camaro Z28’ have?

Using the code:
`print('The model Camaro Z28 has this many cylinders: ')
print(cars.loc[cars['Model']=='Camaro Z28']['cyl'].values[0])`
I was able to output the number of cylinders the car Camaro Z28 has which was 8

# 3.2d Determine how many cylinders (‘cyl’) and what gear type (‘gear’) do the car models ‘Mazda RX4 Wag’, ‘Ford Pantera L’ and ‘Honda Civic’ have.
For this problem I used the code:
`print('The total amount of cylinders and gears for each car are: ')
print(cars[cars['Model'].isin(['Mazda RX4 Wag', 'Ford Pantera L', 'Honda Civic'])][['Model','cyl','gear']])`

Using the `.isin` code I was able too locate the three cars that I want to get my information from. Then followed by the specific information that I want outputed.

# What I learned

Using pandas makes it so that we can use different data frames to compile and collect our data. Through active and thourough use of this function we would be able to properly compact and locate specific parts of our data that might be hard to find manually. By practicing with pandas, I learned how to manipulate and explore data more effectively—whether by filtering, sorting, or combining different datasets. Through this task I was also able to utilize key functions like `.loc` in order to find the data that I need from the data frame. This task has helped me understand the importanc of proper data management and using the built ini functions of phython to extract these data that would be hard to find.




