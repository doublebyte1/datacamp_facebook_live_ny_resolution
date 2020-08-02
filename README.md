## Identifying New Year's Resolutions with Google Trends

In session, you're going to check out Google trends data of keywords 'diet', 'gym' and 'finance' to see how they vary over time. Could there be more searches for these terms in January when we're all trying to turn over a new leaf? Let's find out! In this session, you'll code along to import google trends data into your Jupyter notebook and use `pandas` and a bunch of other packages from the Python data science stack to analyze and interpret these time series. You'll learn a bunch about time series analysis while getting your hands dirty with the world's new year's resolutions. You're not going to do much mathematics today but you'll source your data, visualize it and learn about trends and seasonality in time series data. The emphasis will be squarely on a visual exploration of the dataset in question.

### Code
The code in this repository is released under the [MIT license](LICENSE). Read more at the [Open Source Initiative](https://opensource.org/licenses/MIT).


Detect trends and seasonality

moving average: smooths out noise and seasonality
size of the window -> average of 12 months
what window size does it make sense using? size seasonality

on the moving average, the peak is not so high (it is smooth)

access columns of data frame [[]]

identify patterns and trends
seasonality - repetitive nature

seasonaility - you could remove the trend, but there may be different trends

use differencing instead

trend, the value is around 0. The peaks at January are far more noticeable

stationary: mean and variance dont change over time
For prediction, you would want to convert to stationary

The way of thinking of a peridiocality of 12 months, is that the ts is correlated with itself, every 12 months. Correlation of a ts with a shifted version of itself, is autocorrelation

lmplot (scatter plot for linear regression)

petals - there seems to be a slight negative correlation
they are positively correlated whithin species
causal inferences

Explore your dataset as much as possible and explore it in different ways

the season components of diet and gym are correlated, but the trend no.
This correlation is capturing both of them

plot the difference, and plot the correlation, because this will be the correlation of seasonal components

without the trend, they are highly correlated

AC - the ts is correlated with itself with a shoft of 12 months

spike: 12, 24, 36

correlation at 0

dotted lines: statistical significance of the correlation
The horizontal lines in the plot correspond to 95% and 99% confidence bands.

 If the autocorrelation coefficient is in the confidence interval, it is regarded as not statistically significant. Therefore, the user should focus on the values where the value of the ACF is outside the confidence interval.

The dashed line is 99% confidence band.