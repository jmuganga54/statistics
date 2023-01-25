## Topic
It is time for us to dive into the  heart of `descriptive statistics`, `measurements of central tendency` and `variability`.

## Keywords & notes
### Measures of Central tendency
This lesson we'll introduce you to the three measures of central tendency. Don't be scared by the terminology we are talking about `mean`, `median` and `mode` event if you are familiar with these terms.
![measure of central tendency](./imgs/central_tendency.png)

The first measure we will study is the `mean`, also known as `simple average`. It is dentoted by the Greek latter `mue` for population and `x bar` for a sample.
![mean denoted](./imgs/mean.png)

These notion will come in handy in the next section.

We can find the mean of dataset by adding up all of it components and then diving them by the number of components contained in the data set.
![mean find](./imgs/find_mean.png)

The mean is the most common measure of `central tendency` but it has a huge downside. `It is easily affected by outliers`.

Let's compare these two data sets.
![data set](./imgs/data_set.png)

These are the price of pizza at 11 different locations in New York City and 10 different locations in LA. Let's calculate the means of the two data sets using the formula. 
![mean calculated](./imgs/mean_calculated.png)

For the mean in NYC, we get `$11` whereas for LA just `$5.5` on average pizza. 

>On average, pizza in MY can't be twice as expensive as in LA, right? Correct

The problem is that in our sample we have included one posh place in New York where they charge `$66` for pizza, and this doubled the mean, what we should take away from this example is that `the mean is not enough to make definite conclusions!`

So how can we protect ourselves from this issue. You guessed it, we can calculate the second measure, `the median`, the median is basically the `middle number` in an `ordered dataset`.

Let's see how it works in our example

In order to calculate the median we have to order our dataset in ascending order, `the median of the dataset is the number at position n plus 1, divide by two in the ordered list whee n is the number of observations`

![median formula](./imgs/median_formula.png)

Therefor the median for NYC is at the 6 position or `6` much closer to the observed price than the mean of `$11`.

What about LA, we have just 10 observation in LA. According to our formula the mean is at position `5.5`. In case like this the mean is simple average of the numbers, at position 5 and 6. Therefore the median of LA prices is `5.5` dollars.
![median_city](./imgs/median_city.png)

We have seen that the median is not affected by `extreme prices which is good` when we have posh New York restaurants in a street pizza sample, but we still don't get the full picture of the majority of restaurants, low cost or average

![mode](./imgs/mode.png)
We must introduce another measure `the mode`.The `mode` is the value that occurs most often`. It can be used for numerical and categorical data but we will stick to our numerical example.

After counting the frequencies of each value we find that the mode of `New York Pizza` prices is `$3`, now that's interesting. The most common price of pizza in NYC is just `$3` but the mean and median lead us to believe it was much more expensive.


Let's do the same fnd find the mode of LA pizza prices, from `each price appears only once`. How do we define the mode then. Well, we say that `there is no mode`, but can I say that there are 10 modes you may ask?.

Sure you can but it will be meaningless with 10 observation and an experienced statistician would never do that.

In general you often have multiple modes usually two or three modes are tolerable. But more than that would defeat the purpose of finding a mode.

> There is one last question that we haven't answered which measure is best?

The NYC and LA, example shows us that measures of central tendency should be used together rather than independently. `There is not best... but using only one is definitely the worst`

Now you know about the mean, median and mode, in our next video we will use that knowledge to talk about `skewness`

#### Mean, Median and Mode | Challenge
![measure of central tendency](./imgs/measure_central_challenge.png)

> Solution to the challenge
![solution challenge](./imgs/solution_challenge.png)

```
Execel formulas
MEAN - =AVERAGE(B11:B21)
MEDIAN - =MEDIAN(B11:B21)
MODE - =MODE.SNGL(B11:B21)
```

### Measuring Skewness
After exploring the measures of `central tendency`, let's move on to the measure of `asymmetry`. The most commonly used tool to measure asymmetry is `skewness`.

![Skewness](./imgs/skewness_formula.png)
This is the formula to calculate it, almost always you will use `software that performs the calculations` for you. 

So in this lesson we will not get into the computation but rather the meaning of `skewness`. 

![skewness](./imgs/skewness_indicates.png)
So `skewness` indicates whether the observations in a dataset are concentrated on one side, `skewness` can be confusing at the beginning. 

So an example is in place. Remember frequency distribution tables from previous lectures. Here we have three datasets and their respective frequency distributions. We have also calculates the means, medians and modes.

> Positive Skew / Right skew

![Positive skew](./imgs/right_skew.png)
The first dataset has a mean of `2.79` and median of `2.00`, hence the `mean > median`. We say that this is a positive or `right skew`. From the graph, you can clearly see that the data points are concentrated on the left side. Note the direction of the skew is counter-intuitive.

It does not depend on which side the line is leading to but rather to which side it's `tail` is leading. So `right skewness` means that the outliers are to the right.

It is interesting to see the measures of central tendency incorporated in the graph when we have `right skewness the mean is bigger than the median` and the `mode is the value with the highest visual representation`
![Positive skewness](./imgs/positive_skew.png)

> Zero or no skew
![zero skew](./imgs/zero_skew.png)
In the second graph, we have plotted a data set that `has an equal mean, median and mode`, the frequency of occurrence is completely symmetrical and we call this a `zero or no skew`.

Most often you'll hear people say that the `distribution is symmetrical` 

> Negative skew
![Negative Skew](./imgs/negative_skew.png)
For the third dataset, we have a mean of `4.9` a median of `5` and a mode of `6`, as the `means is lower than the median`, we say that there is a `negative or left skew`. Once again the highest point is defined `by the mode`.

Why is it called a `left skew` again? Because the `outliers` are to the `left`

So why is skewness important. Skewness tells us a lot about where the data is situated. As we mentioned in our previous lesson, the mean, median and mode should be used together to get a good understanding of the dataset, `measure of asymmetry` are the link between the `central tendency` measures and `probability theory` which ultimately allows us to get a more complete understanding of the data we are working with.

#### Skewness | Challenge
![Skewness](./imgs/skewness_challenge.png)

> Solution to the challenge
![solution challenge](./imgs/skewness_solution.png)

### Measure of Variability 
There are many ways to quantify variability. However we will focus on the most common ones, `variance`, `standard deviation` and `coefficient of variation`.

In the field of statistics we will typically use different formulas when working out the population data and sample data.

When you have the whole `population` each data point is known, so you are 100% sure of the measure you are calculating, when you take a `sample of this population`, and you compute a `sample statistic, it is interpreted as an approximation of the population parameter`.

Moreover if you extract 10 different samples from the same population you will get 10 different measures. Statisticians have solved the problem by adjusting the algebraic formulas for many statistics to reflect. Therefore we will explore both population and sample formulas as they are both used.

You must be asking yourself why there are unique formulas for the mean, median and mode.

![mean evaluated](./imgs/mean_evaluated.png)
`Mean`, well actually the sample mean is the average of the sample data points. While the population mean is the average of the population data points. Technically there are two different formulas but they are compute in the same way.

Ok now after this short clarification it's time to get on a `variance` measure of the `dispersion`

### VARIANCE
`Variance` measure the dispersion of a set of data points around their mean value.

![Variance](./imgs/variance.png)

`Population variance` denoted by Sigma squared is equal to the sum of square difference between the observed values and the population mean divided by the total number of observations.

![population variance](./imgs/population_variance.png)

`Sample variance` is denoted by `s squared` and is equal to the sum of squared differences between observed sample values and the sample mean divided by the number of sample observation minus one.

![sample variance](./imgs/sample%20variance.png)

All right when you are getting acquainted with statistics it is hard to grasp everything right away.

Therefore let's stop for a second to examine the formula for the population and try to clarify it's meaning

![population variance](./imgs/population_variance.png)


The main part of the formula is its numerator. So that's what we want to comprehend. The sum of the differences between the observation and the mean squared.

![variance explained](./imgs/variance_explained.png)
So the closer the number of the mean the lower the result we will obtain. And the further away from the mean it lies the larger the difference. 

Easy, but why do we elevate the second degree. Squaring the differences has two main purpose. First by squaring the numbers we always get non-negative computations. Without going deep into the mathematics of it is intuitive that dispersion cannot be negative.

`Dispersion` is about distance and distance cannot be `negative`. If on the other hand we calculate the difference and do not elevate to the second degree we would obtain both positive and negative values, that when summed would cancel out leaving us with no information about the dispersion.


Second `squaring amplifies the effect of large differences`, for example if the mean is 0 and you have an observation of 100 the squared spread is 10000

![squaring variance](./imgs/squaring_variance.png)

> Example
We have a population of 5 observations, `1,2,3,4,5`, Let's find it's variants. We start by calculating the means.

![calculating mean](./imgs/calculating_mean.png)

Then we just apply the formula of findin the variance of a population.

![calcuating the variance](./imgs/population_variance_calculated.png)

So the population variance of the data set is `2` but what about `sample variance`. This would only be suitable if we were told that these five observation were a sample drawn from a population, so let image that is the case.

![sample variance](./imgs/sample_variance_calculated.png)

Denominator is going to be 4 instead of 5, giving us a sample variance of `2.5` to conclude the variance topic we should interpret the result.

![result](./imgs/result.png)

`Why is sample variance bigger than the population variance` in the first case, we knew the population that is we had al the data and we calculated the variance, in the second case, we were told that `1,2,3,4,5` was a simple drawn form a bigger population, 



## Summary