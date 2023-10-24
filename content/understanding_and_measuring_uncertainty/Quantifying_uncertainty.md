---
title: "Quantifying uncertainty in inputs"
draft: false
---

We have highlighted ways to think about the uncertainty coming from specific sources. We now bring this together into approaches that can be applied to understand the size and distribution of these uncertainties and how you might include this information in your analysis. In most cases, the approach to uncertainty quantification is limited by the data and time available to you, though you should also consider where the major sources of uncertainty are in your analysis and pay most attention to these.

In addition, the following approaches can be useful in understanding the size and distribution of the uncertainties in your analytical inputs.

## Distributions

### Discrete and continuous distributions

A probability distribution describes the probability of occurrences of different outcomes. Generally, there are two types of probability distribution; discrete distributions and continuous distributions.

### Confidence intervals

Consider whether you have information about the underlying distribution of the parameter. Often data from other sources will be provided with confidence intervals (or standard errors, etc) that can be used to quantify uncertainty. Where such information is not provided, you may be able to approximate these with knowledge of the sample size and design.

Distributions can also be created using what you know about error from previous models. Consider the performance of previous forecasts against outturn results. The distribution of previous errors can provide the uncertainty distribution for the current forecast. Additionally, you might be able to use one source to validate another or to help estimate the uncertainty in the original source.

### Expert judgement

If no quantitative data on the underlying population is available, you may be able to elicit this information from experts . For example, using the Delphi Method, a structured facilitation method, which relies on a panel of (ideally external) experts to build a combined judgement, for example, about a particular number. This method can be used to ask a panel of experts to estimate the range of uncertainty and use the aggregated responses to produce a distribution. Consider tools to overcome biases, e.g. Brier score. These measure the mean squared difference between the predicted and actual outcomes. The lower the Brier score is for a set of predictions, the better the predictions are calibrated, which has been shown to improve judgement

## Ranges

A range is similar to a probability distribution, in that it considers the possible outcomes but does not consider the probability of each outcome occurring. If there are data or resource limitations a range can be a simple way to illustrate the uncertainty in a parameter.

### Historical data

Historical data can be used to quantify a range. Consider how the parameter has changed over a suitable time period. The maximum and minimum values could provide a sensible range. When using historical data be aware that you will only be able to assess ‘business as usual’ uncertainty. If there are future shocks to the system this may fall outside your historic range.

### Literature review

For parameters that have been the subject of academic studies a literature review can be used to create a range. Consider why different studies may result in different outcomes, and which studies are the most suitable for what you are trying to measure.

### Expert steers

If no quantitative data is available, consider whether there are relevant policy/operational constraints that will limit your range. Judgement from experts can be also be used to create sensible ranges.

## Qualitative assessment of uncertainty

In some situations, it is not possible to create a probability distribution or a range. In such cases, make a qualitative assessment of uncertainty. This is still useful to analysts and customers to consider the magnitude of uncertainty.

### RAG rate your parameters

You can make qualitative assessments yourself, and by using expert judgement. A simple approach is to RAG rate the likelihood and impact of uncertainty in your parameters. This qualitative assessment should be considered when thinking about the analytical results. If data is categorised as highly uncertain and having a large impact on results, then final outputs will be subject to large uncertainty. Care in presentation is needed when using these more qualitative methods, however, as it’s potentially easier for decision makers to misunderstand the relevance of qualitative assessments of uncertainty for their decision compared to quantitative assessments. It is particularly important to explain the impact of uncertainty on the analytical result and the decision to be made when using these types of qualitative assessment.

### Break-even analysis

A further option to support decision makers is to use break-even analysis. This is useful to understand at which point a saving becomes a cost or possibly at which point you would take a different decision.

Some decision makers will be used to seeing a range around a central estimate. Break-even analysis works backwards – if we were to break-even what would the input be? This could help bring the policy alive and help assumption owners to really consider how realistic the assumption is.

Break-even analysis helps people understand how much the input has to change before you reach a break-even point so they can consider the probability of this occurring.





