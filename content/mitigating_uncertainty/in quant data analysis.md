---
title: "Mitigating uncertainty in quantitative data analysis"
draft: false
weight:
---

## Missing data
To decide what method is appropriate to use to deal with missing data, you need to understand why the data is missing.

If the data is missing across all observations, for example due to test design, failure in the observations or failure in recording observations, the data can be classified as missing completely at random (MCAR). This is because the reasons for its absence are external and not related to the value of the observation. It is typically safe to remove MCAR data because the results will be unbiased. The statistical test(s) you are performing may not be as powerful, but the results will be reliable.

Listwise deletion involves deleting all data for an observation that has one or more missing values. The analysis is run only on observations that have a complete set of data. If the number of observations with missing data is small, it may be the most efficient method to handle missing data. However, if listwise deletion would result in throwing away a lot of your data, pairwise deletion may be more appropriate. Here, cases with missing data are used when analysing variables where they don’t have missing values. For example, if you are missing data on a participant’s gender then this participant would be excluded from any analysis using the gender variable but would be included in any analyses for which the participant has complete data. However, the resulting statistics may vary because they are based on different data sets.

If the data is missing systematically, imputation can be more appropriate. The imputation method develops reasonable guesses for missing data. A common technique used when the number of missing cases is small is to impute the mean or median. For datasets with a large amount of missing data, multiple imputation is often used. Here, instead of substituting a single value for each missing data point, multiple imputed data sets are created where the missing values are exchanged for values that encompass the natural variability and uncertainty of the observed values. Each set is then analysed using the standard analytical procedures, and the multiple analysis results are combined to produce an overall result.

The website [How to Deal with Missing Data](https://www.mastersindatascience.org/learning/how-to-deal-with-missing-data/#:~:text=%2520How%2520to%2520Deal%2520with%2520Missing%2520Data%2520,a%2520large%2520amount%2520of%2520missing%2520data.%2520More%2520) provides a useful overview of methods to deal with missing data.

## Type I errors (or a false positives)

The probability of making a type I error (or a false positive) is represented by your significance level (or alpha level): a 0.05 significance level indicates that you are willing to accept a 5% probability that your results occurred by chance.

If you need to be very confident that your results are not going to be a false positive (concluding there is a significant difference when it has actually occurred by chance), you can decrease your significance level, for example to 0.01. Because this change increases the amount of evidence required to conclude a difference is significant, it makes your test less sensitive to detecting differences, but decreases the chance of committing a Type I error (or a false positive) occurring from 5% to 1%.

However, using a lower value for alpha means that you will be less likely to detect a true difference if one really exists, which increases the risk of a type II error occurring.

## Type II errors

A type II error is when you conclude there is no significant difference when one does in fact exist. You can reduce the risk of a type II error by ensuring your sample size is large enough to detect a difference when one truly exists.

## Synthesis

Combining findings from a range of studies, known as synthesis, allows you to draw conclusions from a body of evidence.

Synthesis methods include systematic review and meta-analyses. These methods include reviewing study characteristics and quality and, where relevant, combine data in a statistical synthesis of study findings. 

Evidence synthesis (i.e. systematic reviews and meta-analyses) sit at the top of the ‘evidence pyramid’. This means they are considered the evidence source with the least uncertainty and highest rigour as their design minimises bias and maximises your ability to ascertain causality. However, the types of evidence at the top of the pyramid may not be available or feasible for your research topic of interest, in which case you will need to move down the evidence pyramid (note that this is not a comprehensive list of potential evidence sources):

![](../docs/images/evidence_pyramid.png)