#Data_Analysis_Project


Overview


In this project I made use of Python to handle a large dataset to gather different type of information
this is a image of the dataset:


![image](https://github.com/user-attachments/assets/29cbd5a8-a069-4d2e-8027-8f5421b8252a)


-Data collection and storage


The provided data set shows a transactional data regarding an online business.
The data set also shows the purchased product information where there is a unique ID that is used for each product followed by their sub-category, category and name.
It also contains order details that has as primary key an order ID that can repeat because a customer can purchase multiple products followed by the order date, ship date, ship mode.
Then finally there is the row ID that doesn’t come up multiple times compared to the other ID`s, it represents each transaction that is contained in each row within the dataset, followed by the sales, quantity, discount and profit variables that are used to show detail of the transaction.
The data types within the dataset are integers for numeric variables like for example the Row ID, float for decimal variables such as the sales, Discount, Profit and string for word-based variables such as Region, Country, Order ID etc..
Also other than the type some of the variables within the dataset follow a specific input format like for example the date variables follow a date format “00/00/0000” and another example is for the post codes where each one of them contain 5 numbers by following a “00000” format another example is for the customer ID that follows a format that combines integer and string such as “AA-0000-000000” , the variables follow a specific format for accuracy that is going to help to easily understand the dataset.
Some descriptive statistics include:


*The minimum number of quantity for each transaction is 1 and the max is 14


*The max profit is 18451.27


*The average profit is 8.69


*2121 total transactions


-Data cleaning


Data cleaning is a crucial step when it comes to datasets that takes place before the data analysis and it involves removing duplicate data, missing data, making sure that the data is up to date and making sure that there isn’t invalid data.
It is important to make sure that the dataset doesn’t have any of the defects listed above so that when it comes to the data analysis the results are going to be consistent and accurate.
In the real world it is crucial for organisations to clean their data because if they don’t it will negatively affect them, since they won’t be able to come up with accurate results that they can use to keep track and improve their organisation.


*Chosen approach and justification(codes screenshots and justification)
Code used to identify number of missing values:


![image](https://github.com/user-attachments/assets/7d959dc1-cf96-47db-b3cf-9281cdfb7d9b)


Justification:


Simple code that basically looks for cells within the dataset to see if they are null, if that’s the case they get grouped within the column name that is empty, this process takes place for each of the columns names.
Then after the .sum() just sums the total of missing values for each of cells with each columns and then prints a table like the one in the screenshot to show the number of missing values within each column inside the dataset.


Code used to replace the missing values with the mean


![image](https://github.com/user-attachments/assets/48a5b87d-bce5-40b4-8699-400d89ce14ee)


Justification:


I used the above code to replace the missing values within the Sales and Discount columns with the mean to keep the dataset integrity compared to if I would have chosen to delete the rows that contained the missing values, this to help the analysis performed on the dataset to produce accurate results.
For safety I created a copy of the dataset, the output of the code shows the missing values after this code gets applied that is then 0 because the missing values have been replaced with the mean.


*Screenshot of data after cleaning


![image](https://github.com/user-attachments/assets/d4f6befe-c686-405a-a477-9e8b1d5f6cc2)


I kept using the imputed version of the original dataset.


-Data analysis and visualisation

Visualisation 1 (Comparing the sales and profits of different states)


Screenshot code
![image](https://github.com/user-attachments/assets/009c4d9b-fd04-4ef8-9279-cd1f9b90352c)


Visualisation of the result


![image](https://github.com/user-attachments/assets/e6b7bab5-7039-476a-b0d5-7077c703e1f3)


Interpretation


The visualisation shows both the sales and Profit of all of the states that are mentioned within the dataset.
I created two separate visualisations for each subject to make it easy to read and interpret.
The visualisation uses a x and y axis template where the x label is occupied by the states and the y label is occupied by rounded numeric values that it is used to determine the amount of sales and profit for each state that it can be used to know the states that are doing fine and the one’s that aren`t.
A difference between the two in terms of visualisation is that the Profit visualisation bar chart contains also negative numbers that’s why the visualisation starts sort of in the middle of the page to show both the positive and negative trends.
Key info gathered from the visualisation:


*The state with the highest Sales is California 


*The state with the lowest Sales is Montana 


*The state with the highest Profit is California 


*The state with the lowest profit is Texas


Visualisation 2 (Investigation of the distributon of different ship modes)


Screenshot code


![image](https://github.com/user-attachments/assets/5b712a16-2fa8-4445-89d5-50abaa7d5d55)


Visualisation of the result


![image](https://github.com/user-attachments/assets/01907c08-aae0-4fe6-bae5-d5a016f3c90a)


Interpretation


The visualisation shows the frequency of each shipping method that is available within the dataset.
I made use of a histogram for the visualisation where it makes use of a x and y template for easy interpretation, the x label is occupied by the Shipment modes, and the y label is occupied by count that is used to measure the frequency of each of the shipment modes.
Some info that can be gathered from this visualization are:


*The most used shipment method is Standard class


*The least used shipment method is Same day


*It shows that the customers are not concerned about the speed of the delivery


*It shows that the customers prefer no to spend much on delivery 


Viusalisation 3 (Predominant sub-category in terms of sales)


Screenshot code


![image](https://github.com/user-attachments/assets/3a624fda-eea0-4ff0-b62a-992753b4f7b5)


Visualisation of the result


![image](https://github.com/user-attachments/assets/7969704d-2ca1-4e9d-8b09-dbbfb7737ccd)


Interpretation


The visualisation shows the number of times or frequency of the amount of times a the sub-categories within the dataset are involved in a transaction.
The visualization shows the result through a horizontal bar chart where the y label is occupied by the Sub-categories, and the x label is occupied by the Sales frequency.
The beauty of this visualisation is that it simplifies the thousand of data into this easy to interpret visualisation.
Key info gathered from this visualisation:


*The sub-category with the most sales are chairs


*The sub-category with the least sales are furnishings
