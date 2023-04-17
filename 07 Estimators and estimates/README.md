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


