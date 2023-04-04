## Topics

## Introduction to Inferential Statistics

![Inferential Statistics](./imgs/inferential_statistics.png)
Now that we have covered the basics of `descriptive Statistics` it's time to move on to `inferential statistics`.

![Probability theory and Distribution](./imgs/pro_dist.png)
`Inferential Statistics` refers to methods that rely on `probability theory` and `distributions` to predict population values based on sample data.

![Key areas](./imgs/key_topics.png)
While this definition may not clear just yet starting from the next lesson we will define what a distribution is and we'll go through a couple of distribution you will likely use a work.

This will naturally lead us to `point estimates` and we will conclude the section with `confidence intervals`.

We will not only present these topics but will also develop a deep understanding of the statistical processes.

This will help you a great deal if you get into data science.

These insights will likely be your gateway to the fundamentals of quantitative research and data driven decision making.

> Read More
> [Course Notes](./imgs/027%20Course-notes-inferential-statistics.pdf)

## Keywords & Notes

## What is a distribution?

![Definition of Distribution](./imgs/distribution.png)

Before we can talk about `testing` we have to learn what a distribution is, and in this lesson we'll do just that.

In statistics when we use the term distribution we usually mean a probability distribution. Good examples are `normal distribution`, `the binomial distribution` and the `uniform distribution`.
![Distribution Example](./imgs/distribution_example.png)

> Let start with the definition

`Def:` A distribution is a function that shows the possible values for a variable and how often they occur.
![Definition Distribution](./imgs/def_dist.png)

> Rolling a die
> Think about a die, it has 6 sides numbered from 1 to 6. We roll a die. What is the `probability of getting 1`? is `1/6`. What is the `probability of getting 2`? is `2/6`.

The same for the rest.
![Rolling a die](./imgs/rolling_die.png)

Now, what is the `probability of getting 7`?, it is impossible to get a `7` when rolling a die. Therefore the probability is `zero`.

The distribution of an event consist not only of the input values that can be observed but is made up of all the possible values. So the distribution of the event rolling a die will be given by the following table.
![Probability Table](./imgs/probability.png)

The probability of getting 1 is `0.17` the probability of getting `2` is `0.17` and so on. You are sure that you have exhausted all possible values when the `sum of the probabilities is equal to 100% for all other values`.

The probability of all other values is zero.

Each probability distribution is associated with a graph describing the like hood of occurrence of every event.

The below graph, this type of distribution is called `uniform distribution`.
![Uniform Distribution](./imgs/uniform_distirubion.png)

It is crucial to understand that the distribution is defined by the underlying probabilities and not the graph. The graph is just a visual representation.

Now, think about rolling two dice. What are the possibilities, `(1,1),(2,1), (1,2)` and so on. Here's a table with all the possible combinations.
![Rolling two dice](./imgs/rolling_two_dice.png)

We are interested in the sum of two dice. So what's the probability of getting a sum of 1, the answer is `zero`, as this even is `impossible`.

`What is the probability of getting a sum of 2?`

There is only one combination that would give us the sum of two when both dice are equal to 1. So 1 out of 36 total outcomes or `0.03`.
![Sum of 2](./imgs/sum_2.png)

Similarily the `probability of getting a sum of 3?` is given by the number of combinations that give a sum of three divided by `36`. Therefore `2/6` is `0.06`.
![Sum of 3](./imgs/sum_3.png)

We continue this way until we have a full probability distribution.
![Full probability distribution](./imgs/full.png)

Let's see the graph associated with it.
[Graph](./imgs/graph.png)

So looking at it we understand that when we roll two dice the probability of getting `7` is the highest. We can also compare difference outcomes such as the probability of getting a `10` and the probability of getting a `5`. It's evident that it's less likely that we'll get a 10.

The examples that we saw here were of discrete variables. Next we wil focus on `continuous distribution` as they are more common in inferences.

In the next few lessons we'll examine some of the main type of continuous distributions starting with a `normal distribution`.

> Course notes
> [Course notes](./imgs/028%20Course-notes-inferential-statistics.pdf)

## The Normal Distribution

So far we learned that the distribution of a data set shows us the frequency at which possible values occur within an interval.
![Distribution frequency](./imgs/Dis_frequency.png)

We also said that there are dozens of distributions, experience statisticians can immediately distinguish a `binomial` from a `porcelain distribution` as well as a `uniform` from an `expoential` distribution in quick glimpse at a plot.
![Different Distributions](./imgs/distributions.png)

![Normal vs Student's T](./imgs/normal_t_distribution.png)
In this course though, we will rather focus on the `normal` and `student's T distributions` due to the following reasons.

1. They approximate a wide variety of random variables
2. Distribution of samples means with large sample size could be approximated to normal
3. All computable statistics are elegant
4. Decision based on normal distribution insights have a good track record.

Here is a visual representation of a `normal distribution`.
![Normal distribution](./imgs/normal_dist.png)

You have surely seen a normal distribution before as it is the most common one. The statistical term for it is `Gaussian distribution` but many people call it the `bell curve` as it is shaped like a bell.

It is `symmetrical` and its `mean, median and mode` are equal. If you remember the lesson about `skewness` you would recognize that it has no `skew`. It is perfectly centered around its mean. So it is denoted in this way.
![How it is denoted](./imgs/norma_distribution.png)

```
N~(mean,variance) - N stands for normal. The `tilde` sign denotes it is  a distribution and in brackets we have the mean and the variance of the distribution.
```

You can notice that the highest point is located at the `mean` because it coincides with the `mode`. The spread of the graph is determined by the `standard deviation`.
![The Spread of the graph](./imgs/n_sd.png)

Now let's try to understand the normal distribution a little bit better. Let's look at this approximately normal distribution histogram.
![Normal distribution](./imgs/normal_distribution_graph.png)

There is a concentration of the observations around the mean which makes sense as it is equal to the the mode.
![Normal distribution](./imgs/mean_nd.png)

Moreover it is symmetrical on both sides of the mean. We used 80 observations to create this histogram. It's mean is `743` and its standard deviation is 140.
![Standard deviation and mean](./imgs/mean_sd.png)

> What if the mean is smaller or bigger?
Let's zoom out a bit by adding the origin of the graph.
![Normal distribution, zoom out](./imgs/nd_zoom_out.png)

> Controlling for the standard deviation

The origin is the zero point. Adding it to any graph gives perspective. Keeping the `standard deviation fixed or in statistical jargon` controlling for the standard deviation, `a lower mean would result in the same shape of the distribution`, but on the left side of the plane. In the same way a `bigger mean would move the graph to the right`.

In our example this resulted in two new distributions, one with the mean of `470` and a standard deviation of `140` and one with a mean of `960` and a standard deviation of `140`.
![Controlling standard deviation](./imgs/controlling_sd.png)

> Controlling for the mean 
We change the standard deviation and see what happens this time, the graph is not moving but is rather `reshaping` a lower standard deviation result in `lower dispersion`. So more data in the middle and thinner tails.
![Controlling mean](./imgs/controling_mean.png)

On the other hand  `higher standard deviation` will cause the graph to fly with less points in the middle and more to the end or in statistics jargon `fatter tails`
![Higher standard deviation](./imgs/lower_sd.png)













## Summary
