## Topics
![Practical Examples](./imgs/practical_examples.png)

Finally it's time for the practical example we've been talking about in this lesson, we will see an actual database of a real estate company operating in California.

We're interested in the statistical properties of the data. That is why we have reordered the database and cherry picked variables than imported DS in a spreadsheet.

The labels of the columns have been made friendly even for those of you who have no experience with real estate.

Finally we have altered the names of the customers for confidentiality reasons.

The company is launching a marketing campaign but it wants to target its audience properly.

The management suspects after some shore analysis marketing results can be improved without the need of investing additional resources.

We are the data analysis who are going to crunch some number and identify which groups of people are most likely to buy our product.

Once we have done so we will instruct the marketing team to focus its efforts on these groups.

`The first thing we have to do when we analyze data is get acquainted with the table.` It illustrates the skills of real estate property for a specific company. Let's call it 365 data sites real estate California. Hopefully no one else thought of that name.

![Table](./imgs/table.png)
Second the table has two parts the left and right, on the left hand side, we have the `product information`, on the right hand side, we have `customer information`.

![Customer](./imgs/customer_info.png)
You can easily sport all `products` are listed but customer information is only available for some `products`.

![Sold buyer](./imgs/sold_buyer.png)
This is because we input information about a customer once the deal is done logically only `sold items` are associated with a buyer. This is because we input information about a customer once the deal is done, logically only `sold item` are associated with a buyer.

![Customer Detail](./imgs/customer_detail.png)
Let's see what a row looks like. This should clear up the logic of the table for your `Nora Lynch` with a customer id `C004` was 56 years old when she bought apartment 43 in building one, live there.

She paid `$377,313.56` for an area of `1160.36` square feet in June 2004, Nora is form California. Felt very satisfied with the deal and didn't get a mortgage for the purchase. She found out about our product through our website.

Now that's out of the way we need to dig deeper into these variables. We will identify types of data and levels of measurement for some of them. This is crucial steps as we cannot analyze the data, if we don't understand it's type.

Let's start from the first column ID. `ID` is a value we assign to each item that let's us differentiate between products. It may look `numerical` to you but it is `categorical` that's counter-intuitive the first time.

> ID may look numerical, but its categorical

So let's clarify it. What if we use the names like `John 1`, `John 2`, `John 3` and so on until John N. The meaning would not change `id` variable are like names we assign to different products. Howere it is much easier to use numbers as unlike names, we have an infinite number of numbers.

A simple way to check if a variable is numerical or categorical is to interpret its mean. The mean ID  `Mean ID:2975` number shows nothing. Now oppose this to the mean price `Mean Price:$280,637`. The mean price is a valuable piece of information.

> Ok the bottom line is ID is a categorical variable.

`What about it's level of measurement?` Well it is qualitative `nominal`.

The next variable that we will explain is `Age`. Age is rather interesting. The level of measurement is `quantitative ratio` A rule used for verifying ratios is asking the question. Is there a true `zero point`.

Well for age when you are born you are exactly `zero years old`. That's the true zero point. So we are safe.

However once intriguing is whether age is discrete or continuous it may be both, in this case we can only see age as the whole number, therefore it is `discrete`. However similar to weight of variable we discussed earlier in this course. `Age` is a continuous variable.

When I am recording this the Statue of Liberty is 131 years old but I may get more specific by saying, it is 131 years and 11 months old or it age is 131 92. If I had days minutes and seconds I'll get 131 nine thousand four hundred twelve, you get the point when dealing with age, you decide it's time depending on your work at hand. This is yet another way to represent age.

The next variable we have is age interval. This is yet another way to represent age. Once again it is continuous or discrete as we are talking about the same variable. This time through the level of measurement is ordinal instead of a ratio, the age groups represent different categories ordered but are not numerical.

This shows that the same variable can have different levels of measurement within the same database.

In most corporate analysis `price` is Central no matter the data set, it is always a numerical variable, that like age may be discrete or continuous depending on your needs.

If you are interested banks and corporations treat it as continuous and so will we. The level of measurement here is ratio.

The next variable we want to look to is `gender`. It is categorical type and its level of measurement if `nominal`.

```
Gender
Type of data: categorical -> Male or Female
Level of measurement: nominal 
```

It is similar to `yes` `no` questions discussed in a previous lesson. Such variables are called binary as there are only two possibilities. 

```
Variables that can only take two possible values are called binary:
Male, female;
Yes, no
```

Finally let's check out the `location`. We will discuss state in more detail and leave country for homework.

The `state variable` refers to sales in the USA only. Note that only if the country input is USA, would we have a value for state. State is a categorical variable like ID, we talked about earlier.

```
State is a categorical variable like ID
```

You can label the US states from 1 to 50 and use numbers instead.
![States](./imgs/states.png)

Either way the variable is `categorical` and it's level of measurement is `nominal`.






















## Keywords & Notes

## Summary