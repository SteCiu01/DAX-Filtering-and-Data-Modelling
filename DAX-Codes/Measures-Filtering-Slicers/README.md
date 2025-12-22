# Measures Filtering Slicers

#### Situation

We have a matrix visual that displays data as below:

| Products | Total Returns | Associated Sales |
| ----- | ---- | ---- |
| Product A | 125 | 560 |
| Product B | blank | 154 |
| Product C | 265 | 1,240 |

However, we want to only see those products that had returns. 

To achieve it we need to set the level visual filter for Total Returns as "IS NOT BLANK".

However, if we have some slicers, for instance Product Category, Sub-products or Products, they most likely will carry "dead values". In fact 
