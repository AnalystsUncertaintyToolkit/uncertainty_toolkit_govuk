---
title: "5.2 Common techniques for assessing uncertainty in analytical outputs"
draft: false
---

Now that we have explored how to assess uncertainties in individual analytical inputs, we turn to commonly used techniques for analysing overall  uncertainty in analytical outputs, moving from approaches to use when we have a good numerical understanding of input uncertainties, through to approaches which can be used when we know less about how input uncertainties are quantified.


{{< accordionset >}}

{{< accordion title="Monte Carlo Techniques" >}}

If all significant sources of uncertainty can be quantified, along with the correlations between them, then probabilistic methods can provide a picture of the range of possible outcomes and the likelihood of each.

#### Outline

The basic process for a Monte Carlo simulation is to:
1. Define a distribution for each input showing the uncertainty in each. These can be simple distributions based on estimation (e.g. uniform, triangular) or more complex distributions based on data (e.g. normal, beta).
2. Define the correlations between these inputs
3. Randomly generate a value from each input distribution (accounting for correlations)
4. Calculate the outputs of the model deterministically
5. Repeat steps 3) and 4) many (i.e. thousands of) times
6. Analyse the distribution of the resulting outputs

#### Advantages

* Produces a full probability profile of the range of possible outcomes and the likelihood of each – the gold standard in uncertainty analysis
* Enables analysis of complex interactions between uncertainties within a model
* Produces a visual representation of the range of possible outcomes, that may aid customer understanding
* Can be used to assess the impact of  removing or reducing a source of uncertainty

#### Disadvantages

* Highly dependent on the accuracy of the distributions used
* May require more resource than other techniques to build
* Correlations can be difficult to define mathematically, and can give misleading results if not properly accounted for
* Can be computationally expensive
* Outputs may not be reproducible if insufficient iterations are used (effectively introducing further uncertainty to the model)


#### Examples

* Can help assess overall uncertainty when you have uncertainty around many aspects of your model
* Assess uncertainty around a fund forecast
* Estimate the uncertainty around assumptions used in policy costings
* An example of how MoJ use Monte Carlo analysis to assess uncertainty is provided [here](https://github.com/AnalystsUncertaintyToolkit/UncertaintyWeb/blob/master/Monte%20Carlo%20template/Monte%20Carlo%20Template.xlsm)

{{< /accordion >}}


{{< accordion title = "Convolution" >}}

If there are a small number of uncertainty sources, then it may be possible to combine them mathematically, which can be quicker than using probabilistic methods

#### Outline

In principle uncertainty distributions can be combined to give an exact distribution for the resulting overall uncertainty (known as convolution).

Consider rolling two dice - the value of each follows a discrete uniform distribution from 1 to 6. If we wanted to know the sum of the two dice, we can combine these uniform distributions to show that the resulting probability profile follows a triangular distribution from 2 to 12.

This avoids the randomness of probabilistic approaches. However this method tends to get very complicated once more than a few uncertainties are involved, and probabilistic methods may be easier.

#### Advantages

* Deterministic, so outputs are reproducible and quick to generate
* Works with any input probability distributions (don't need to assume normality)

#### Disadvantages

* Can be difficult to do with more than 2 or 3 sources of uncertainty
* Generally only feasible if the distributions are combined using simple mathematical operations (addition, subtraction, multiplication)
* Assumes that each uncertainty is independent (or correlations must be accounted for)

#### Example

Any situation where you're combining two probability distributions using simple mathematical operations (addition, subtraction, multiplication)

{{< /accordion >}}


{{< accordion title="Summing Uncorrelated Uncertainties in Quadrature" >}}

If multiple components need to be summed, and the uncertainty in each can be assumed to be normal and uncorrelated, then summing in quadrature is a useful shortcut for estimating the total uncertainty

#### Outline

If the model is simply summing a number of output components (e.g. a number of different funding forecasts), and the uncertainty is known in each, then the uncertainty in the sum of those values can be given by the square root of the sum of the individual uncertainties squared (assuming that all errors are independent and normally distributed).

#### Advantages

* Very simple to calculate
* Can include uncertainties from all sources

#### Disadvantages

* Only applicable for models where uncertainties can simply be summed - more complex interactions will need to use other techniques
* Only valid if the individual uncertainty distributions are independent and normally distributed

#### Examples

Useful for financial forecasting, where individual budgets and their uncertainty has been assessed, and these must be summed to give the overall budget. In this situation assuming independence between budget over/underspends is often reasonable.

Also useful for quickly estimating the uncertainty when changing the timeframe of a forecast e.g. if you have a forecast by month (with quantified uncertainty), then this is quick way of estimating the uncertainty in the annual totals – assuming there is no correlation between the uncertainty from one month to the next.

{{< /accordion >}}


{{< accordion title="Using Past Variance to Estimate Future Uncertainty" >}}

If a forecast has been produced repeatedly over many years, it may be possible to use the accuracy of all the previous forecasts to estimate the uncertainty in the new forecast.

#### Outline

Start by looking at the variance of all of the previous forecasts after one time period, and create a distribution of these variances. This distribution can be used to estimate the uncertainty of the new forecast after one time period.

Repeat for the variance at each subsequent time period to produce e.g. a fan forecast (smoothing if needed).

#### Advantages

* Captures all sources of uncertainty
* Avoids the need to identify, quantify and combine individual sources of uncertainty
* Based on real-world performance, so avoids optimism/pessimism bias (the estimated uncertainty may be asymmetric as a result)

#### Disadvantages

* Needs the system to be stable over time (i.e. there’s no reason to think that the system is more/less predictable than in past years)
* Needs the approach to forecasting to have been consistent over the years (i.e. there’s no reason to think that our forecasts will be more/less accurate than in previous years)
* Would not work for large and infrequent events
* The forecasts must have been produced for a sufficiently long time so that we have enough historical data on the variance to capture the full range of plausible variances

#### Example

[MoJ prison population forecasting](https://analystsuncertaintytoolkit.github.io/UncertaintyWeb/case_studies.html#estimating_uncertainty_in_prison_population_projections)

{{< /accordion >}}


{{< accordion title="Focussing on the Dominant Uncertainty" >}}

If one source of uncertainty has a much greater impact than all the others, then the uncertainty due to this one factor might be a reasonable proxy for the overall uncertaint.

#### Outline

Consider all the sources of uncertainty affecting the analysis and quantify the impact that each has on the overall uncertainty (even if this is approximate or subjective – see section on 'Defining and Identifying Uncertainty'). If one source has substantially more impact that the others, then simply looking at the uncertainty in this one factor might be a pragmatic approximation for the overall uncertainty measure, ignoring other sources.

This is not a robust way of estimating overall uncertainty, as it ignores all but one source. It should only be used if previous techniques are inappropriate, and there is genuinely one source of uncertainty that has an impact that is an order of magnitude larger than the others. However, when time is tight this may be a pragmatic way of estimating uncertainty.


#### Advantages

* Relatively simple and quick
* No need to combine uncertainties
* Focusses attention on the key driver of uncertainty, avoiding unnecessary discussion of relatively minor elements

#### Disadvantages

* Will always underestimate the overall uncertainty as most sources of uncertainty are excluded
* Can dramatically underestimate uncertainty if the source of uncertainty assumed to be dominant isn’t as dominant as believed

#### Example

The Accuracy Tracking Tool <b>(link to DfE Accuracy tracking tool to come)</b> can be used to estimate the residual uncertainty once the dominant uncertainty has been modelled. This tool assesses the accuracy of different forecast elements and allows you to see the percentage which both the dominant and residual uncertainty contribute to the total error.

{{< /accordion >}}

{{< accordion title="Scenario analysis" >}}

If there are many sources of uncertainty with complex correlations between them and the likelihood of them occurring is unknown, then it may be more sensible to use a set of scenarios to illustrate the range of plausible outcomes.

#### Outline

1. Identify the individual sources of uncertainty, and the range of possible values for each.
2. Create a set of coherent scenarios (jointly agreed with the decision maker), setting each source of uncertainty to a value that could realistically occur in parallel with the others (e.g. a crimewave is unlikely to occur if the economy is booming).
3. Try to ensure that the chosen scenarios cover the full range of possible outcomes, from highly optimistic to highly pessimistic, with equal attention given to each to avoid bias in presenting the results.
4. Then quantify the overall uncertainty in each scenario, combining uncertainties using other methods in this section (the benefit is that this combining can be done manually for a small number of specific cases, rather than having to formulate the combinations mathematically for all possible inputs).

#### Advantages

* Don’t need to mathematically define the correlations between sources of uncertainty
* Gives ‘real-world’ explanations to the range of possible outcomes, which may increase buy-in from the customers
* Can include low-probability, high-impact events (i.e. system shocks) without needing to define their probability

#### Disadvantages

* The choice of scenarios is subjective, and may not cover the full range of plausible outcomes
* Risk of optimism/pessimism bias, with scenarios not evenly distributed around the most likely outcome
* Provides no information about the likelihood of each scenario occurring
* Needs input from a range of knowledgeable people

#### Example

Forecasting where a range of policy options are being considered, particularly where the likelihood of an event occurring is unknown, for example early analysis on Exiting the EU scenarios.

{{< /accordion >}}


{{< accordion title="Judgement" >}}

If the previous methods are unfeasible then you could make a subjective estimate of the overall uncertainty using expert elicitation techniques.

#### Outline

If the previous methods are unfeasible, then adding a subjective estimate of the overall of uncertainty is an option. Where there is too little information or time to do a quantified analysis, it may be better to provide a judgement on the uncertainty than nothing at all. 

Ideally this should be a group decision, using formal expert elicitation methods (e.g. Delphi) to avoid group-think and arrive at a consensus, agreement, or an average (depending on the technique used). If formal expert elicitation isn’t possible, then the judgement of an individual is better than nothing, though less rigorous.

However the uncertainty is estimated, make sure that it is clear that it is a subjective opinion rather than results of analysis to prevent it being misused.

#### Advantages

* May be able to be produced quickly, though can take time if using formal elicitation methods with large groups
* Requires little to no data
* Based on real-world performance, so avoids optimism/pessimism bias (the estimated uncertainty may be asymmetric as a result)
* Do not need to consider all sources of uncertainty individually
* Do not need to mathematically combine uncertainties

#### Disadvantages

* Highly subjective
* Needs a group of knowledgeable experts, who can reasonably be expected to have a grasp of the range of possible outcomes

#### Examples

* Providing context around a high priority figure that needs to be submitted quickly.
* Analysis based on a data source of unknown reliability
* Analysis where the expected range of results would lead to the same outcome

{{< /accordion >}}



