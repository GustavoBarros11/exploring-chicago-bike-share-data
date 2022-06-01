# **Exploring Chicago Bike Share Data**
This is my implementation of the Explore Chicago Bike Share Project<br/>
From Udacity Machine Learning & AI Foundations Nanodegree<br/>
**Data Science Project**

![jpg](imgs/img1.jpg)

In this project, you will make use of Python to explore data related to bike share systems for Chicago. You will write code to import the data and answer interesting questions about it by computing descriptive statistics. You will also create some important functions and plot charts.

# Table of Contents
- [**Exploring Chicago Bike Share Data**](#exploring-chicago-bike-share-data)
- [Table of Contents](#table-of-contents)
- [Business Problem](#business-problem)
- [Business Questions](#business-questions)
- [Project Assumptions](#project-assumptions)
- [Data Dictionary](#data-dictionary)
- [Solution Planning](#solution-planning)
  - [Final Product](#final-product)
  - [Tech Stack](#tech-stack)
  - [Process and Methods](#process-and-methods)
- [Conclusion](#conclusion)
- [References](#references)
- [Next Steps](#next-steps)

# Business Problem
Over the past decade, bicycle-sharing systems have been growing in number and popularity in cities across the world. Bicycle-sharing systems allow users to rent bicycles on a very short-term basis for a price. This allows people to borrow a bike from point A and return it at point B, though they can also return it to the same location if they'd like to just go for a ride. Regardless, each bike can serve several users per day.

Thanks to the rise in information technologies, it is easy for a user of the system to access a dock within the system to unlock or return bicycles. These technologies also provide a wealth of data that can be used to explore how these bike-sharing systems are used.

In this project, you will use data provided by [Motivate](https://www.motivateco.com/), a bike share system provider for many major cities in the United States, to uncover bike share usage patterns. You will use the data from one of the largest cities of United States: Chicago.

# Business Questions
* Task 1: Print the first 20 samples(rows) from the database
* Task 2: Print the gender(column) of the first 20 samples
* Task 3: Create a function to get the columns as a list
* Task 4: Count how many of each gender do we have
* Task 5: Create a function to count the genders
* Task 6: Show the most popular gender
* Task 7: Plot a a chart using the previous data
* Task 8: Answer why summing the number of Males and Females doesn't match the number of samples
* Task 9: Find the minimum, maximum, mean and median duration of the trips
* Task 10: Get all the start stations of the dataset
* Task 11: Create a function count the occurrence of any given column (optional)

# Project Assumptions
* Some template code was provided.

# Data Dictionary
Data for the first six months of 2017 are provided. The data file contain six (6) columns.

Variable | Description
--- | ---
Start Time |  (e.g. 2017-01-01 00:07:57)
End Time |  (e.g. 2017-01-01 00:20:53)
Trip Duration |  (in seconds, e.g., 776)
Start Station |  (e.g. Broadway & Barry Ave)
End Station |  (e.g. Sedgwick St & North Ave)
User Type |  (Subscriber or Customer)
Gender | (Male or Female)
Birth Year |  (e.g., 1980)

# Solution Planning
## Final Product
Deliver a python script with the all TASKS completed passing all `assert` statements.

## Tech Stack
* Python
* Matplotlib

## Process and Methods
* Task 1: Print the first 20 samples(rows) from the database
    * Method: 
        - `for i in range(20): print("{}. {}".format(i, data_list[i]))`
* Task 2: Print the gender(column) of the first 20 samples
    * Method: 
        - `for i in range(20): print("{}. {}".format(i, data_list[i][-2]))`
* Task 3: Create a function to get the columns as a list
    * Method: 
        - Create function function that gets a multidimensional list and returns a particular column(list) specified by the index.
* Task 4: Count how many of each gender do we have
    * Method: 
        - Iterate over the list with a for loop and create a conditional clause to select each case and add 1 value to a counter of the respective value
* Task 5: Create a function to count the genders
    * Method: 
        - Put the above logic into a function
* Task 6: Show the most popular gender
    * Method: 
        - Print the largest value for the previou counters in respect to the genders
* Task 7: Plot a a chart using the previous data
    * Method: 
        - Use matplotlib to plot a bar chart of the frequency of each gender
* Task 8: Answer why summing the number of Males and Females doesn't match 
    * Method: the number of samples
        - Because there are missing values
* Task 9: Find the minimum, maximum, mean and median duration of the trips
    * Method: 
        - Use a for loop to iterate over and make the calculations
* Task 10: Get all the start stations of the dataset
    * Method: 
        - Implement: `user_types = set(column_to_list(data_list, 3))`
* Task 11: Create a function count the occurrence of any given column 
    * Method: (optional)
        - DOCSTRING: Function that counts the occurrence of any given column and returns the types and their quantities on the column.

# Conclusion
This was my first project in the data science world, it was a good start because it didn't involve leaving the ordinary python stack, but still introduced the usage of python for data science. It helped grasp how it is to import a dataset, explore and draw some conclusions about it.

# References
- [Udacity](https://www.udacity.com)

# Next Steps
- Create a notebook to make understanding this project easier
- Create some neat visualizations to gain more insight about the dataset
