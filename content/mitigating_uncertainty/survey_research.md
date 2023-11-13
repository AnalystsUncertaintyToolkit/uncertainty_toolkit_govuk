---
title: "Mitigating uncertainty in survey research"
draft: false
weight: 4
---

There are numerous different ways to reduce the risk of uncertainty posed by your data collection methods.

## Questionnaire testing

### Piloting
Testing a questionnaire with a small group of experts is a useful method for ensuring questions are appropriately worded and likely to be understood by the target audience. It is a useful test of face validity. That is, it tests whether the question, on the surface, taps into the concepts it’s intended to measure.

### Cognitive testing 
This is a form of qualitative research with prospective survey respondents to understand how they interpret and answer specific questions and what they think about when completing the survey. This helps to ensure results of the survey are properly understood by the researcher and that the questions make sense to the respondent and elicit the kind of information expected.

### Question testing
Item non-response occurs when a respondent completes a survey but fails to provide an answer on specific items. The amount of item non-response is considered a useful indicator of data quality. If particular questions are commonly left unanswered, it may indicate a problem (e.g. respondents may not understand what’s being asked, the question may be sensitive, the response categories are insufficient and so the respondent cannot adequately answer, etc.). 

Item non-response is a particular concern if it occurs systematically (i.e. particular types of respondents are less likely to answer a particular question). When conducting a survey, testing for item non-response helps to identify issues with particular questions and any systematic bias that might introduce.

## Question sequencing and randomisation

To minimise the priming effects arising from the order of questions, researchers should carefully decide the sequence of questions, as well as considering whether rotating the order of certain questions is appropriate. Furthermore, it’s common practice to randomise the order of response options where these are codes or statements, and invert the order of the scale for half the respondents for questions with a rating scale as the response options.

## Using scripting and logic in online surveys

To increase data accuracy, for online surveys you can use methods such as only showing particular questions to respondents as a result of their responses to previous questions and ensuring that several answer options cannot be chosen on questions where only one answer option should be chosen.

## The size of your sample

Larger samples will tend to be more representative (assuming you are conducting random sampling). Keep in mind that it’s unlikely that every sample will be perfectly similar to the population of interest. There will always be a little sampling error associated with any study, unless you sample every single member of your population.

## The likely response rates of your survey

You may need to contact a lot more people than you need to achieve a sample that is representative of your population under study and allows you to draw conclusions within the margin of error you are willing to accept.

## Your sampling frame (your possible participants) and recruitment procedures

Avoid only recruiting members of a certain subset of your population. Ideally you would randomly sample from your sample frame. Through this, you minimize any selection biases that might occur, such as volunteer bias.

Selection bias occurs when the subjects studied are not representative of the target population about which conclusions are to be drawn. However, selection bias is only problematic if the response probability is correlated with the variable you are measuring, i.e. the people who respond to the survey answer differently to your questions to the way in which those who did not respond would have done. Thus, addressing selection bias requires breaking the connection between non-response probability and outcome variables: adaptive response design.

## Implementing a stratification protocol, such as proportionate stratified sampling

Let’s say you do your research and find out your population under study are 80% women. You could then make sure that 80% of your sample consists of women, such as by quota sampling.

Alternatively, you might want to consider over-sampling: this is the selection of a large number of additional respondents that match certain criteria, to allow researchers to measure more precisely the changes in key populations.While this might not result in your overall sample representing the overall population under study (e.g. the general population), this may provide the most useful approach to allow you to draw conclusions from a small sub-group, such as a particular ethnic group.

## Using sample weights to correct for the over-representation or under-representation of key groups

You can weight down the responses from the over-represented group (which may have been purposefully oversampled) to make sure their views do not have a disproportionately large effect when conclusions are drawn based on responses from the whole sample, or weight up the responses from under-represented group to make sure they don’t have a disproportionately small effect.

A sample weight is a statistical measurement which is linked to the record of every survey respondent. The sample weight is calculated based on the probability of being selected for the survey for the respondent and can also account for other imbalances which arise in the sampling process, such as non-response adjustment. The value of a weight can be interpreted as a measure of the number of population members represented by that respondent.

For example, if 51% of a population are female, but a sample is only 40% female, then weighting is used to correct for this imbalance. There are a number of different types of weights.

### Design weights

We use design weights to account for the different probabilities of being sampled that different respondent types have. Let’s say we’re collecting data based on a list of addresses. People who live in a place where many families share the same address will have a lower chance of being surveyed than people who live at single-family addresses. Weighting our survey results ensures our results won’t be skewed by this discrepancy.

### Non-response weights

You can use non-response weights to correct for the fact that some types of people are less likely to be willing to participate in your survey than others. To illustrate, let’s imagine that young people in our district are less inclined to answer our survey questions. Weighting our results ensures that we account for this fact by placing more load on the responses from young people who do participate.

### Calibration/post-stratification weights

You can use calibration weights to make the characteristics of your sample closely match the characteristics of your population. This is commonly done using demographic data (like gender, age, income level) that is publicly available (from a Census, for example) as the target and adjusting the sample demographics to match that target.

Weights almost always increase the standard errors of estimates and introduce instability into your data. Some researchers like to “trim” the weights to not allow extremely high weights that can increase instability of estimates, but trimming the weights can often result in reducing the representativeness of the weighted data – it’s a trade-off between less instability or more accurate representativeness.
