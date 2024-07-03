# Pandas Challenge 1
## Module 4 Assignment work: This module involves analyzing a dataset from an e-commerce company.

***The Data:***
>The analysis was done on a sales order dataset that contained orders from 54,639 clients and heir order details. Fields include:
>* Customer identifiers: Full name , phone number, email and an internal id called client id
>* Product Categories and sub categories of the order
>* Order details- date of the order, unit cost, unit price nd quantity
>
***Files:***
>The following files are avaiable for your review:
> * the data is provided as a.csv and is avaiable in the resourcesz\ folder as client_dataset.csv
> *The code to run the analysis is stored in pandas_challenge_1.ipynb.

***Summary Stats:***
> The code hs been built to identify the following :
> * ***Part 1: Exploring the Data*** - initial review of the data provided showed no null values but quantity and weight were firls that were populated with the value '0'. These records were removed (142 entries) as a value is expected in these fields
>   
***Part 2: Data transformation*** 
> * A column caelld ***subtotal*** was created to hold the subtotal for each line using the unit_price and the qty ( unit_proce* qty) this is the field also used to comute Revenue 
> * A column called ***shipping price*** was comuted where a price of 7 per pound for orders over 50 pounds and 10 per pound for items 50 pounds or under.
> * A column called ***total_price*** was created using the subtotal and the shipping price along with a sales tax of 9.25%.

> * A column called ***total_cost*** was created using unit cost, qty, and shipping price ( it assumes the shipping cost is exactly what is charged to the client).

> * A column called ***total_profit*** was created of each line using line cost and line price.

***Confirmation***

>The calculations were confirmed by reviewing order numbers 
>Order ID 2742071 had a total price of $152,811.89 Order ID 2173913 had a total price of $162,388.71 Order ID 6128929 had a total price of $923,441.25
>
***Summary***
>The next section involves generating a formatted summary of totals for the top 5 clients( ran ordered by entries, for the following fields
>*total units purchased
>*total shipping price
>*total revenue*
>total profit.
>
>this section is followed by a write up of key observations
>
