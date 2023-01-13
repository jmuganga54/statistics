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
## Summary