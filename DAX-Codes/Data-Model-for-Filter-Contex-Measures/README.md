# Data Model for Filter Contex Measures

Using slicers based on some columns of a fact table can be generally acceptable if you don't have a specific Dim table, however there is to be careful when you want to use that same column also within a filter context measure.

Let's make an example to see the issue and the solution.

We have a Purchase Orders fact table:

| customer_id |  PO_nr   | days_old |
|------------|---------|----------|
| a          |  xhejsf  | 0        |
| a          |  heixkl  | 2        |
| a          |  lwsjgc  | 4        |
| a          |  ofhbcp  | 9        |
| a          |  ppgges  | 12       |
| b          |  kkbbhjk | 0        |
| b          |  hhjkkll | 1        |
| b          |  fffiio  | 2        |
| c          |  yyyhhh  | 0        |
| d          | cccvvv  | 0        |

We also have the Dim_Customers table:

| customer_id | Customer_name |
|------------|---------------|
| a          | cust_a        |
| b          | cust_b        |
| c          | cust_c        |
| d          | cust_d        |

