## Topic
Now that we've covered the necessary theory it is time for some testing. We are going to explore two types of tests drawn from a single population and drawn from multiple populations.

![single_multiple](./img/single_mltiple.png)

This is very similar to confidence intervals for a single populationa and confidence intervals for two population that we convered previously


In the next few sessions, we will run tests for a single mean with both known variance and unknown variance.

Let's start with the test in chich the `variance is known`.



## Keywords & Notes

## Single population

For this tests, we will use our good old data scientist salary example. Here's the data set one more time, by now, I hope you are able to calcuate the sample mean. It is `$100,200`. The population variance is known and it's standard deviation is equal to `$15,000`. Moreover the sample size is 30.

However you swa that aaccording to `Glassdoor` the popular salary information website, the mean data scientists salary is `$113,000`. The sample that is availabel on `glassdoor` is based on `self-reported` numbers and you would like to see if it's value is correct.

We needed a two sided test as we were interested in known both if the salary is significantly less than that or significantly more than that.

The null hypothesis is the `population mean salary is $113,000`. We denote as, see below.

![Data scienties](./img/data_scientists.png)

The alternative hypothesis is that the population mean is different than `$113,000`

![hypothesis](./img/hypothesis.png)

`Testing is done by standardizing the variable at  hand and comparing it to the z which follows a standard normal distribution`


We standardize a variable by substracting the mean and dividing by the standard deviation.

`A variable is standardized by substracting the mean and diving by the standard deviation`.

Since it is a sample we use the `standard error`. Thus the formula for standardization becomes captial Z is equal to the sample mean minus the value of interest from the null hypothesis divided by standard error.


![standardizing](./img/standardizing.png)

In this way we obtain a distribution with a mean of zero. Any standard deviation of one the upper case z should not be mistaken with the lowercase Z.


`The uppercase Z is the standardized variable associated witht he test and will be called the Z score`. The lower case z is the one from the table we talked about before and henceforth will be reffered to as the critical value.


![z_score](./img/z_score.png)

> How does the test work

Think about this, the lowercase z is normally distributed with a mean of 0 and standard deviaiton of 1. The upper case Z is normally distributed with a mean of X bar mins mue and standard deviation.

![z_Z](./img/z_Z.png)

`Standardization lets us compare the means`, the closer the difference of x bar minus mue 0 to zero the closer the z score itself to zero, this implies a higher chance to accept the `null hypothesis`.

> Let's go back to the example.

So what is the value of our standardized variable replug in the numbers that we have from the begining of the lesson. What we get is a z score of minus 4.67

![Z-score](./img/Z_score_value.png)


> Now we will compare the z score to the cirital value

Now we will compare the absolute value of minus 4.67 with a Z of alpha divided by 2 where alpha is the significance level.

Note that we use the absolute value as it is much easier to always compare positive capital Z with positive lower z's. Mowerver some Z tables don't includes negative values.

![z_table](./img/z_tables.png)

You should be aware that the two statements minus 4.67 is lower than the negative critical value, is the same as 4.67 hihger than the positive critical value.

![table](./img/table.png)

Thus our decision rule becomes absolute value of the `z score` should be higher than the absolute value of the crital value.

![decision](./img/decision.png)

 Using `5%` significance, our alpha is 0.05. Since it is a two sided test we check the bale for Z of 0.05 the corresponding value is 1.96.

 ![table2](./img/table2.png)

 The last thing we need to compare our standardized variable to is the crital value.

 If the z score is higher than 1.96 we would reject the null hypothesis, if it is lower we will accept it.

 `4.67` is higher than `1.96`. Therefore we reject the null hypothesis.

 ![reject](./img/reject.png)

 The answer is that at 5% significance level we have rejected the null hypothesis or at `5% significance level we have rejected the null hypothesis`.

 Or "There is no statistical evidence that the mean salary is $113,000.

 ![reject_statements](./img/reject_statements.png)

 There are many other ways to express this and you will probably hear more about this later in the course.
 
 What if we had a difference level using 1% significance, we have an alpha of 0.01. So Z of alpha divided by 2 is 2.58. Once again our z score is 4.67 is higher than 2.58 so we would reject the null hypothesis, even at the 1% significance

 ![one percent](./img/one_percent.png)

 But how much further can we go before we cannot reject the null hypotheis anymore, 0.5% of 0.1%?

 There is a a special technique that allows us to see what the signifcance of all is after which we will be unable to reject null hypothesis. We will see it in our next section.

 ## Exercise
![exercise](./img/exercise_1.png)

## Solution
![Solution](./img/solution_1.png)