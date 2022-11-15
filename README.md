# SIMULATING RESTAURANT FOOD SUPPLY

## Introduction
It often gets challenging for restaurants to estimate the food supply for the week in order to avoid any shortage of food or wastage of food. In order to tackle this problem, here we are trying to create a simulated environment of a restaurant with 2 processes: Waiter and Customer, interacting with the environment via Events like Taking orders from customers, Giving orders to the cooks, Serving food to customers 

## Motivation:
To approximate how much food a restaurant needs to prepare for the next day, given the number of customers visiting each day and the average time to serve a customer.

## Flow of the Project
### Simulate Waiters
Model a waiter (a process) who serves in a restaurant (an environment). Some basic things that waiters do are:
- Taking orders from customers
- Giving orders to the cooks
- Serving food to customers

### Simulate Customers
We will follow the same process as simulating waiters. However, since there is a limited number of customers that can be served in the restaurant, we will also model the restaurant with a limited capacity. Here, we have limited the number of customers to 2, which means that new customers can get into the restaurant only when there are fewer than 2 customers in the restaurant.

### Simulate Food Quantity with Customers
We will simulate a restaurant that:
- Only takes take-out orders
- There is only one staff member
The customers are waiting in line to order food on the menu. The more items a customer orders, the longer the customer needs to wait.

The attributes of this restaurant are:
- *staff* : a resource with the capacity 1 (the staff can only serve one customer at a time)
- *foods* : options of food the restaurant offers
- *available* : number of items per option of food
- *run_out* : events when each option of food runs out
- *when_run_out* : the time when each option of food runs out
- *rejected_customers* : number of customers who leave the line because their food option runs out

### Creating a Customer
We also want to create a customer who is waiting in line. A customer will:
- Leave if there is not enough food left
- Order food if there is enough food left
If there is no food left after the customer orders a particular kind of food, we will declare that the chosen food has run out.

## Screenshots
(of any restaurant diagram with processes happening - may be in animated form to better explain what we're doing)

## Credits
This project is presented by @shreya-saini-07, @Mitansh-Khurana and @manisha-singh22 in reference to a simulation project contributed by khuyentran1401
