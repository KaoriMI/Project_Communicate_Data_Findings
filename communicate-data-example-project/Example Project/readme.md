# Diamonds Data Exploration

## Dataset

The data consists of information regarding 54,000 round-cut diamonds, including
price, carat, and other diamond qualities. The dataset can be found in the
repository for R's ggplot2 library [here](https://github.com/tidyverse/ggplot2/blob/master/data-raw/diamonds.csv),
with feature documentation available [here](http://ggplot2.tidyverse.org/reference/diamonds.html).


## Summary of Findings

In the exploration, I found that there was a strong relationship between the
price of a diamond and its carat weight, with modifying effects from the cut,
color, and clarity grades given to the diamond. The relationship is
approximately linear between price and carat when price is transformed to be on
a logarithmic scale and carat transformed to be on a cube-root scale. I found a
somewhat surprising result initially when the marginal trend for the cut, color,
and clarity variables indicated that higher diamond quality was associated with
lower price. However, higher diamond quality was also associated with smaller
diamonds. When I isolated diamonds of a single carat weight, there was a clear
positive relationship between higher diamond quality and higher diamond price.

Outside of the main variables of interest, I verified the relationship between
diamond carat weight and its x, y, and z dimensions. For the dataset given,
there was an interesting interaction in the categorical diamond quality
features. The lower clarity grades looked like they had slightly better
distribution of cut and color grades than diamonds with the higher clarity
grades.


## Key Insights for Presentation

For the presentation, I focus on just the influence of the four Cs of diamonds
and leave out most of the intermediate derivations. I start by introducing the
price variable, followed by the pattern in carat distribution, then plot the
transformed scatterplot.

Afterwards, I introduce each of the categorical variables one by one. To start,
I use the violin plots of price and carat across clarity. I'm only looking at
the clarity grade plot here since it's the clearest example of how the
categorical quality grades affect diamond pricing. The other two categorical
variables, cut and color, are covered afterwards, using point plots. I've made
sure to use different color palettes for each quality variable to make sure it
is clear that they're different between plots.


***
APR vs Prosper vs original loan
As the Prosper rating increase, the cloud of points moves towards bottom of the plot. Also, as the Prosper Rating increase, more higher loan amount appears, although ratings of 5 and 6 seems the peak and rating 7 has less high loan amount while borrower APR still go lower than 5 and 6.

APR vs Proper vs bank utili
As the Prosper rating increase, the cloud of points moves from right-top to left bottom. The higher Prosper ratings tends to have lower bankcard utilization.

APR vs Proper vs credit score range
As the Prosper rating increase, the cloud of points moves from leftt-top to middle bottom. The higher Prosper ratings tends to have lower credit score range.

APR vs Employment Status vs Loan Original Amount
Retired people seems borrow smaller amoutn of loan while APR is still widely spread. Cloud points doesn't move clearly and employment status doesn't give significant impact compared to the original loan amount.

APR vs Employment Status vs credit score range
The cloud points of not-employed and others are high, while other employment status cloud pointes are more spread around the middle from the top to lower right. Thus, employment status can give more impact than the credit score itself, especially if you are unemployed.

APR vs Income Range vs Loan Original Amount
As the income range increase, the more higher loan amount increase. Cloud points of vertical line doesn't significantly change between income range, while it gets shorter when loan amount gets higher. Thus, income range doesn't give significant impact compared to loan amount.


APR vs Income Range vs Loan Original Amount vs Employment Status
Self-employed and employed group shows similar pattern. Just employed group has more higher loan amount even when both are in the same income range. Employed group also has more lower APR rate in every income range. There are retired people with high income range, but APR doesn't show significant difference between each income range.
When you are employed, the influence of income to APR are clear, although interestingly, income range of $0 has much lawer APR. Other than that, the influence is not clear.

APR vs Income Range vs Loan Original Amount vs prosper ratingsMost of the lower have Prosper rating of more than 3 and income.
The income doesn't give much difference in APR, compared to the Prosper rating. As the prosper rating goes higher, there are more lower APR.
The cloud points moves from left to right as loan amount increase, and moves from top to bottoms as the Prosper ratings increase.
After separate plot
he larger error bars around $0 and Prosper rating of 1.0 are due to there bing fewer loans. Income range of $25,000+ shows a little bit unclear relationship with APR, while we see linear relationship either positive or negative. Except the Prosper rating of 1, no-income has higher APR rate.