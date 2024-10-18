---
title: "Predicting staff pay costs"
draft: false
weight: 4
---

## The situation

Each department has to manage their pay costs to ensure they stay within their budget, making decisions to recruit (or not) in the face of uncertainty over staff turnover, pay rises, etc.

## The analytical approach

Use a microsimulation to model staff members over time, with departures, promotions, and new recruits modelled stochastically.

## Asking the right questions

* Initially 'what will our pay costs be at the end of the year for a given recruit plan?'
* Redefined as 'how likely is it that our costs will exceed our budget?', allowing a risk-based approach to decision-making, and also allowing uncertainty in the budget to be incorporated.

## Defining and identifying uncertainty

Unknowns:

* The pay budget including additional sources of funding not known until the start of the year

Assumptions:

* Number of staff who will join or leave the department in future months
* Variation in starting salaries, pension etc. for new staffs
* Variation in pay awards based on staff performance

## Understanding and measuring uncertainty

* A Monte Carlo approach was used due to the large number of sources of uncertainty, its suitability in microsimulation, the (assumed) lack of correlation between sources, and availability of time. Given that the model was likely to be reused many times, it was worth investing the time to build a full probabilistic uncertainty assessment into the model.
* Most numerical assumptions in the model (including dates) can be entered as a distribution (exact, uniform, or triangular, along with some bespoke distributions for specific purposes).
* This resulted in a full probability distribution of the range of possible outcomes.

![Examples of different types of distributions](/images/staff_pay_1.png)





## Presenting and communicating uncertainty analysis

* All major uncertainties were quantified, and presented (with any unquantified sources noted elsewhere).
* The key output was simply the likelihood of remaining within budget, using positive and negative framing (e.g. "We have an 70% chance of staying within budget, and a 30% chance of exceeding our budget")
* As the budget holder was an analyst, we chose to present the full probability density profile to illustrate the range of possible over-/under-spends.
* Alongside, simple prose descriptions of the 90% prediction intervals to describe the likely range of the over-/under-spend
* A further graph was used to show how performance against budget was predicted to evolve over the year, using multiple line graphs to show the 90% prediction intervals.



![Probability density profile and line graph showing positive and negative framing](/images/staff_pay_2.png)

