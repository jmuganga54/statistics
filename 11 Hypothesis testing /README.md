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

## What is the p-value and why is sit one of the most useful tool for statisticians?

Now we know how to test hypothesis and how to reject them. Actually we reject the hypothesis at various levels of significance but we couldn't find a level of significance for which we could no longer do it.

![we_know](./img/we_know.png)

This is the right moment to introduce a measure called the `P-value`. This is the most common way to test hypothesis instead of testing at pre-assigned levels of significance. We can find the smallest level of significance at which we can still reject the null hypothesis given the observed sample statistics.

![pvalue](./img/pvalue.png)

So how we do that. Recall the test with the data scientists salary. We had a standard error of `2739`, known population standard deviation of 15,000, normally distribute population and a sample size of 30, the corresponding z score was minus 4.67.
![example](./img/example.png)

We reject the null at 0.05 and 0.01. But we wanted to know how much lower we could go. We can check the Z table for plus 4.67 which gives us the same result as minus 4.67. 

![cant_find](./img/cant_find.png)


In most Z table, you would not find this value as it is so large. Thus we round up to the close's value available and get 0.0001.

![cant_find](./img/approximate.png)

> But how do we actually test the hypothesis?

Well after choosing a significance level of alpha you compare the P-value to it. `You should reject the null hypothesis if the pvalue is lower than the significance level.`

![reject_pvalue](./img/pvalue.png)

Therefore we can safelty say that such a result is extremely significant by any measure of significance.

![exmple_pvalue](./img/example_pvalue.png)


Let's see another example, if our z score was 2.12 we should reject the null hypothesis at 5% but not reject it at 1% significance. 

![another_example](./img/another_example.png)


Now it becomes more interesting at this point, we can actually look at the table and then find the pvalue. We look for the value that corresponds with 2.12 and find that it is 0.983 the pvalue for a one sided test is (1- number we see on the table). So the corresponding pvalue is equal to `0.017`. The pvalue for a two sided test is (1 - the number we see in the bale) multiplied by 2. Therefore the pvalue would be 0.034, this is also the answer to our question.

![table_value](./img/table_value.png)
![pvalue conditions](./img/pvalues_condition.png)

> Wehere and how are pvalues used

![where_pvalue](./img/where_pvalue.png)

Most statistical software packages run tests and then provide us with a series of results, one of them is p-value. It is then up to the researcher to decide whether the variable is statistically significance or not. Generally software is designed to calcuate the p-value to the third digit after separator.

The point is when you start conducting your own research you would love to be able to see the three zerors after the dot. The closer to 0 your pvalue is the more significant is the result you've obtained.

The final consideration is taht the pvalue is an extremely powerful measure as it works for all distributions, no matter if we are dealing with the normal Student's t, binomial or uniform distribution.

Whatever the test the `p-value` rationale hold if the `p-value` is lower than the level of significance you reject the null hypothesis. Having said that you would normally use the p-value in the presence of a digital medium.

Throughout this couse I recommend that you use online `p-value` calculators to support your studies and double check your answers.

![online](./img/online.png)