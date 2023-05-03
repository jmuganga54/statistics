## Topics

## Keywords and Notes

## Estimators and estimates
Lets's continue by introducing the concept of an `estimator` of a population parameter, it is an approximation depending solely on sample information a specific value is called an `estimate`
![Estimate](./imgs/estimate.png)

There are two types of estimates, `point estimates` and `confidence interval estimates`.

`Point estimate` is a single number while `a confidence interval` naturally is an interval the two are closely related. In fact the `point estimate` is located exactly in the middle of the `confidence interval`. However `confidence intervals` provide much more information and are preferred when making inferences.
![Point Estimate vs Confidence intervals](./imgs/point_interval.png)

All right have we seen estimates so far? Sure we have, the `sample mean X bar` is a point estimates of the `population mean mue`. Moreover the `sample variance as squared` was an estimates of `population variance sigma squared`.
![Point estimates](./imgs/point_estimates.png)

There may be many estimators for the same variable. However they all have two properties, `Bias and efficiency`, we will not prove them as the mathematics associated is out of the score of this course.
![Properties](./imgs/properties.png)

However you should have an idea about the concepts estimators are like judges. 
![Judges](./imgs/judges.png)

We are always looking for the most efficient `unbiased estimator`, an unbiased estimator has an expected value equal to the population parameter.
![Bias](./imgs/bias.png)

Let's think of a biased estimator to explain that point. What if somebody told you that you will have to find the average height of Americans by taking a sample, finding its mean and then adding one foot to that result. So the formula is X bar plus 1 foot. 
![Biased Estimator](./imgs/biased_estimator.png)

Well I hope you won't trust them. They gave you an estimator but a biased one. It makes much more sense that the average height of Americans is approximated just by the sample mean. We say that the bias of this estimator is `1 foot`.
![Why bias](./imgs/why_bias.png)

Let's move on to efficiency. The most efficient estimators are the ones with the least variability of outcomes from the estimates we know so far we haven't seen estimators with problematic variants, so it is hard to exemplify.
![Efficiency](./imgs/efficiency.png)

It is enough to know that the most efficient means the `unbiased estimator with the smallest variance`


## Confidence Intervals
In previous lesson we learned about `point estimators`. But as you can guess they are not very reliable.

Imagine visiting 5 percent of the restaurants in London and saying that the average meal is worth 22.50 pounds. You many be close but chances are that the true values is it really 22.50 but somewhere around it its much safer to say that the average meal in London is somewhere between 20 and 25 pounds.

In this way you have create a confidence interval around your point estimate  of 22.50 pounds, Confidence Interval: [20pounds, 25pounds]
![Confidence Interval](./imgs/confidence_interval.png)

`Confidence Interval` is a much more accurate representation of reality. However there is still some uncertainty left which we measure in levels of confidence.

So getting back to our example you may say that you are `95% confident that the population parameters lies between 20 and 25 pounds.
![95% sure](./imgs/sure_confiedence.png)

Keep in mind that you can never be 100% confident unless you go through the entire population, and there is of course a 5% chance that the actual population parameter is outside of the 20 - 25 pounds range.
[5% chance](./imgs/not_sure.png)

We'll observer that if the sample we have considered deviate significantly from the entire population.

There is one more ingredient needed. The `level of confidence` it is denoted by `one minus alpha` and is called the confidence level of the interval.
![Confidence level](./imgs/confidence_level.png)

Alpha is a value between `0 and 1`.

For example if we want to be 95 percent confident that the parameter is inside the interval Alpha is 5% If we want a higher confidence level say 99% Alpha will be 1%.
![Confidence level](./imgs/levels.png)

The formula for all confidence interval is from the point estimate minus the reliability factor times  the standard error to the pont estimate plus reliability factor times standard error.
![Formula Confidence Interval](./imgs/formulat_ci.png)

## Population Variance Known, Z-Score
A `confidence Interval` is the range within which you expect the population parameter to be and its estimation, is based on the data we have in our sample.
![Confidence Interval](./imgs/confidence_int.png)

There are two main situations when we can calculate the confidence intervals for a population when `population variance known` and `population variance unknown`, depending on which situation we are in we would use different calculation method.
![When Confidence Interval](./imgs/when_confidence_interval.png)

In this lesson we will explore the confidence intervals for a `population mean` with a `known variance`.
 ![Confidence Interval](./imgs/confidence_interNormal.png)

An important assumption and in this calculation is that the population is normally distributed even if is not, you should use a large sample and let the `Central Limit Theorem` do the normalization magic for you.

`Remember if you work with a sample which is large enough you can assume normality of sample means`.

Let's say you want to become a data scientist and you are interested in the salary you're going to get. You are also aware that `population standard deviation` of the data science salaries is equal to `$15,000`. Furthermore you know the salaries are normally distributed and your sample consists of `30 salary's`

The formula for the confidence interval with a `known variance` is given below.
![Formula](./imgs/formula_ci_pvknow.png)

> X bar is population mean which we have already be given `$100,200`, population std is given already `$15,000`. Number of sample (n) is 30

Let calculate `Standard error` 
![Standard Error](./imgs/standard_error_calc.png)

What have left is the so called `reliability factor` Z of alpha divided by two, Z is the statistic that we've described earlier. `The standardized variable` that has a standard normal distribution. Alpha is the same alpha we had when we defined our confidence level. So for a `confidence level of 95%`, alpha would be equal to `5%`. Similarily for a confidence level of `99%`, alpha would be equal to 1%. It all fall into place.
![Alpha](./imgs/alpha.png)

Keep in mind that a `95%` confidence interval means that you are sure that in `95%` of the cases, the true population parameter would fall into the specified interval.

The Z of Alpha comes from the so-called `standard normal distribution` table it is best to forsee it and then comment on it.  

Let's say we want to find the values for the `95%`, confidence interval Alpha is `0.05`. Therefore we are looking for Z of Alpha divided by two  which will be `0.05/2 = 0.025`. This will match the value of `1-0.025 = 0.975`, the corresponding Z comes from the sum of the `row and column table headers` associated with the cell. 
![Reliability factor](./imgs/reilability_factor.png)

A commonly used term for the `Z` is `critical value`. So we have found the critical value for this confidence interval. Now we can easily



