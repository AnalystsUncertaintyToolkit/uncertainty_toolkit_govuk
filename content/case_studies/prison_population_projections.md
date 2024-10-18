---
title: "Estimating uncertainty in prison population projections"
draft: false
weight: 2
---

## The Situation

Prison population projections are the end result of a number of criminal justice system interconnected models. The uncertainty around each of these models had not been estimated, but understanding the uncertainty of prison projections was essential for capacity planning.

## The analytical approach

Court demand and sentencing and forecasts were used within a prison population microsimulation model, with policy forecasts overlaid.

## Asking the right questions

* How confident are we that the prison population will not exceed a particular threshold?
* Was there sufficient resource to estimate uncertainty using a traditional bottom-up approach (i.e. combining the uncertainty from all constituent models)?

## Defining and identifying uncertainty

* Court demand projections
* Sentencing assumptions (custody rate)
* Impact estimates of future policy changes
* Unknown impacts such as exogenous system shocks or policy changes not known at time of projection
* Estimation error (such as sampling bias) from simulation model

## Understanding and measuring uncertainty

* A top-down approach was chosen as the resource requirement for a traditional bottom-up approach would have been prohibitive.
* The variance of all the previous forecast errors after 1 time period were fitted to a chosen probability distribution (in this case a normal distribution was chosen). This distribution was used to estimate the uncertainty of the new forecast after 1 time period.
* This process was repeated for the variance at each subsequent time period.
* The rate of change of variance was used to extrapolate the variance for periods where no forecast error existed.

## Presenting and communicating uncertainty analysis

* We presented our historical forecast errors, explaining their main drivers and how each contributes to our current uncertainty range. This helped our key customers to better understand the uncertainties inherent in the system we model, and therefore why we can't produce more precise forecasts.

* The other aspect was helping customers think about how they should use the uncertainty estimates. For example: for the prison estate, assessing the likelihood of prison population reaching different levels together with an assessment of risk appetite and contingency measures we could use. This allowed for an evidence based approach for how much capacity we should plan for, not simply planning to the central estimate.

<img src="/images/prisons.png" height = "auto" width = "900" alt = "Population projections with future error spread modelled">

