# PA-3_ECE2112P

# Programming-Assignment-3

## In the given Programming Assignment we were tasked to create a code using pandas

# In the first part of the assignment we were tasked to:
### - Load the corresponding .csv file into a data frame named cars using pandas.
### - Display the the first five and last five rows of the resulting cars. 

# #3.1 Load the correspoding .cvs file into a data frame named cars using pandas.

In order to do this task first is to input:

## [1] import pandas as pd

So that we would be able to use the different syntaxes that it offers.

Then using the code:

## cars = pd.read_csv('cars.csv')

This would put the .csv file into a data frame in order to extracts its elements.

# #3.1 Display the first five and last five rows of the resulting pandas. 

In order to perform the task we would need to utilize the code:

## .head() and .tail()

Using the code *cars.head(10)* I was able to extract the first 10 rows of the given data frame.

Then using the code *cars.tail(10) I was able to extract, starting from the last row, the 10 last rows of the given data frame.

## What I learned

### I learned that if I want to extract the data of a .csv file then I would need to use the code .read_csv("name of the .csv"). And in order for me to extract either the first couple or last couple of rows, I would need to use the code .head("number of rows from the first row") and .tail("number of rows from the last row") in order to output the specific amount of rows that I want. 

# In the second part of the assignment we were tasked to:
## - Display the first five rows  with odd numbered columns in the given data frame cars
## - Display the row that contains the 'Model' of 'Mazda RX4'
## - Determine how many cylinders ('cyl') does the car model 'CamaroZ28' have
## - Determine how many cylinders ('cyl') and what gear type ('gear') do the car models 'Mazda RX4 Wag', 'Ford Pantera L', and 'Honda Civic' have.

# #3.2 Display the first five rows with odd numbered columns in the given data frame 'cars'

In order to do this task I used the code:

## .iloc()

So that I would be able to input the specific indexes that I want to output. Simply inputing the code:

## cars.iloc[[0,1,2,3,4],[1,3,5,7,9,11]]
