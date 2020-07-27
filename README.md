# Regression-Analysis-House-Sales
## Objective: 
Perform a multiple regression analysis of houses sold in King County and optimize the base model to best represent the data present. Using cleaned data find what predictors have large impact on sales price. The data targets reoccurring home buyers looking to optimize their budget to get the highest quality house at the lowest cost
## Data Analysis:

### What condition house to buy?
![Imgur](https://i.imgur.com/M4X7BrA.png)

Between low-end house (condition 1&2) and high-end (condition 3,4, &5) subgroups there is little difference in average sale price. The jump from condition 2 to 3 is a $150,000 change. However, maintenance and overall satisfaction of the recurring buyer would justify buying up to higher-end house. Within the high-end subgroups condition 4 has the lowest price followed closely by condition 3, and would be the target as to not go too overbudget with condition 5

### Best building decade.
![Imgur](https://i.imgur.com/8I5iw88.png)

The above chart is a specific representation of only houses that meet the condition 4 criteria. Data overtime displays that the housing market is increasing, and new built houses will cost the most. With cost efficiency in mind houses built in the 1960 offer the cheapest price ideally without being culturally out of date.

### Optimal buying and selling periods.
![Imgur](https://i.imgur.com/qRD1Lkb.png)

January and February display the lowest average house price making it the best time period of buying houses while April is the counterpart having the best prices for selling houses. The subsequent months show an average sale price of $530,000 with not much deviation. The first four months of the year are having the most market volatility, possible working the buyer/seller favor if times correctly 

### Where to find the perfect house.
![Imgur](https://i.imgur.com/KKJOcuT.png)

When looking at houses Seattle and Bellevue have the highest prices with location to the city and waterfront availability driving up prices drastically. Cheaper alternatives are seen largely in southern King County. The graph dots size and color are representative of their cost and all depict a condition 4 house made in the 1960. If the buyer is looking for waterfront availability, Des Moines offer ideal locations for the price. With that if location is an issue, Renton closer to the larger cities like Seattle while still having competitive house prices.

## Muliple Regression
### Baseline Model 
![Imgur](https://i.imgur.com/QVwSD6p.png)

After an initial regression analysis, we get a baseline R2 0.673. With that there is a lot of data needed to be manipulated to achieve a better analysis. 

### Final Iteration
![Imgur](https://i.imgur.com/9O88oaB.png)

Iterations:
1. Remove outliers 
1. Create dummy variables 
1. Drop non signifiant P-values


The final model achieved a R2 of 0.710 improving by 0.037. While the change is not drastic a better fit of the data was achieved. The data was then split for training and testing:

* Train RMSE: 132093.1980972533
* Test RMSE: 127851.15655611489
 
There is only 3.2% difference between the two values indicating the model is not over or underfitted.

## Recommendations 
1. Search for house that are preferable condition 4 for highest values and lowest price of high-end houses
1. Look for houses built in the 1960’s
1. For buyers, close on a house in January or February. For Sellers, aim to sell it during the month of April
1. Search for houses in southern King County for lower house prices on average

## Future Research 
1. Resale value of house based on length of residency
1. Cost benefit analysis of common renovations projects
1. House listing time period based on the year built
