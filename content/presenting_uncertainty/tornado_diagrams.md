---
title: "Tornado diagrams"
draft: no
weight: 8
summary: null
---

Tornado diagrams are different to most other graphs discussed here. They are not used to show the outputs of the analysis, but to show how different sources of uncertainty contribute to the overall uncertainty.

Tornado diagrams depict sensitivity of a result to changes in selected variables. They show the effect on the output of varying each variable at a time, keeping other input variables at their assumed values.

This can help communicate the reasons for uncertainty, and identify further need for analysis. If the level of uncertainty is unpalatable to the customers, then this format can be useful to help focus work on reducing the level of uncertainty in key parameters. Tornado diagrams also help you to focus on the inputs which are most important to focus on getting as “right” as is possible.

One limitation of the format is that only one parameter is changed at a time, which can be misleading in complex models. There are some situations where the uncertainty due to one variable may appear small initially but becomes much more prominent if a second variable takes on a slightly different value (e.g. think of a workflow model with a bottleneck. A tornado diagram might show the bottleneck parameter to be the overwhelming uncertainty. However, if this parameter is increased slightly then the bottleneck may move elsewhere, completely changing the picture)

![Example: [Nuclear Levelized Cost of Electricity, BEIS (pdf)](https://assets.publishing.service.gov.uk/government/uploads/system/uploads/attachment_data/file/566567/BEIS_Electricity_Generation_Cost_Report.pdf). The graph presents the change in the levelized cost of nuclear electricity (&#163;/MWh) that would result from changes in input parameters. Impacts are shown from both 10% upward or downward movement in central estimates and from predetermined parameters ranges (high/low data range). Yellow bars represent an increase in the parameter, blue bar represent a decrease in the parameter.](/images/tornado.png)

Example: [Nuclear Levelized Cost of Electricity, BEIS (pdf)](https://assets.publishing.service.gov.uk/government/uploads/system/uploads/attachment_data/file/566567/BEIS_Electricity_Generation_Cost_Report.pdf). The graph presents the change in the levelized cost of nuclear electricity (&#163;/MWh) that would result from changes in input parameters. Impacts are shown from both 10% upward or downward movement in central estimates and from predetermined parameters ranges (high/low data range). Yellow bars represent an increase in the parameter, blue bar represent a decrease in the parameter.
