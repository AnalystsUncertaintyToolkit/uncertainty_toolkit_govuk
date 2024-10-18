---
title: "2. Jointly agreeing how uncertainty should be used"
date: 2023-02-27T17:25:32Z
draft: false
weight: 1
---


Decision-makers need information about uncertainty in the impacts of their decisions. This section looks at the steps to ensure that analysts and decision-makers agree on the question being asked, how analytical outputs will be used in the decision-making process, and how to appropriately incorporate uncertainty into the analysis.

## Understanding the problem

### Clarify what the real question is

It is important to ensure that the question is correctly framed to address the problem. For example, are we really interested in ‘how much money is this new policy likely to save?’, or should we be asking ‘how certain can we that this policy would save more than £x?’.

As well as clearly defining the question, we should also ensure that any important detailed questions to support the analysis are appropriately thought through. For example, are we interested in uncertainty on a calendar year or financial year basis?

### Identify the important details

You may also want to jointly identify sources of uncertainty that are so deep that little or nothing can be said quantitatively about their impact on the outcome. An example might be the impact of a natural disaster on a particular policy. Deep uncertainties can have major implications for decision making, and may call for a descriptive approach to the analysis and presentation of options.

Once the key questions have been agreed, analysts and decision-makers should discuss how the outputs will be used. Understanding the role of the analysis in the decision-making process will help to inform which uncertainty techniques are appropriate and proportionate.

## How will the outputs be used?

### Discuss the role for the analysis

Will the decision be based purely on the results of the analysis, or is it just one of a wider set of considerations informing the decision? The more influential the analysis is, the more important it is to build in robust uncertainty analysis.

### Are there dependent models drawing on the analysis?

If the output is to be fed into ‘downstream’ models, then it is important to understand the requirements of those models. For example, if scenarios are used to illustrate uncertainty in your model, then these may not be suitable inputs for a Monte Carlo simulation in a dependent model.

## To summarise

Now that we know what the question is and the context in which the analysis will be used, we should agree how to build appropriate uncertainty into the analysis. It is a good idea to ask the decision maker what it is conceptually that they would like to be able to say. This is important as it frames how the uncertainty analysis will be conducted.

## Work with the decision maker to inform their decision at the right time

### Explain how the uncertainty can be used to better inform decisions

We can help the decision-maker to understand how information about the uncertainty present in the analysis supports a better informed and more robust decision. It’s important to make it clear that not all sources of uncertainty will be quantifiable and/or supported by robust evidence, and we should jointly prioritise the key sources of uncertainty that need to be included in the model.

### Avoid misleading results or spurious accuracy by choosing the appropriate presentation

We can assess the impact of uncertainty using many different techniques. Not all will be appropriate for a given piece of analysis. A poor choice of technique may even give misleading results. For example, if there are many sources of uncertainty, the use of 95% confidence intervals to describe just one limited part of this uncertainty may be misleading, and modelling a range of described scenarios may be more appropriate. Appropriate presentation, such as rounding, is equally important to avoid spurious accuracy and implying better precision than is actually the case. These aspects are covered further in the [presenting]({{< ref "/presenting_uncertainty">}}) and [communicating]({{< ref "/communicating_uncertainty">}}) uncertainty chapters.

### Discuss how the uncertainty will inform the decision-maker’s judgement

Discuss with the decision-maker what level of uncertainty is acceptable. Do they want to know how wrong the forecast would need to be in order to change or rethink the policy? Or are they simply interested in an output “range”? If so, what does that “range” actually mean?

Examples can be very helpful when discussing the analysis with the decision maker. An answer to the question of the net benefits of a policy may be £3m, with uncertainty analysis giving a broad range of £0.5-5.5m. You could discuss with the decision maker how they want to be able to frame the analysis, for example:
- “A range of £0.5-5.5m”
- “The estimated benefits are £3m, with analysis showing a 90% likelihood that benefits will be between £1-5m”
- “Analysis shows that there is an 80% likelihood that the net benefits will be greater than £2m”
- “The policy needs to have x amount of takeup in order to break even”

Operational decision makers may not want to see a range of results, but instead want to plan to a certain level of confidence, such as 65% or 95% rather than 50%. For example, when planning the number of schools, prison places or GPs we’ll need over the next 5 years, it may be more appropriate to plan to a higher level of confidence than 50%.

Financial decision makers may be interested in understanding the likelihood of receiving a certain level of income, or that risks and opportunities will materialise. For example, HMRC might want to know the likelihood of receiving a certain level from tax receipts. Here, the analysis would need to go hand in hand with financial risk management to mitigate the risks materialising or crystallise the opportunities.