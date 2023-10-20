---
title: "Sources of uncertainty: Experimental and quasi-experimental evaluation design"
date: 2023-02-27T17:25:32Z
draft: false
weight: 5
summary: "Sources analysis summary..."
---

Experimental and quasi-experimental evaluation designs are used in government to understand and estimate the impacts of policies. They do so through statistical comparison to a group or time period unaffected by the intervention. This unaffected group acts as a proxy for what would have happened to the affected group in the absence of the policy and is commonly called the counterfactual. It is also possible to compare multiple versions of an intervention with a control group, these are known as multi-arm trials.

Commonly used experimental and quasi-experimental methods include randomised control trials, difference in difference and interrupted time series analysis. [The Magenta Book](https://www.gov.uk/government/publications/the-magenta-book) provides a full guide to evaluation methods. When conducting or commissioning this type of research, analysts have an important role in ensuring that potential sources of uncertainty are understood, adequately addressed and effectively communicated to stakeholders.

The sources of uncertainty in experimental and quasi-experimental research can be broadly categorised into data, study design and statistical analysis. Analysts who employ these methods should consider to what degree each of these three areas create uncertainty in understanding and estimating the impact of a given policy or intervention.

## Data

Regarding quantitative data for evaluations, some of the things you need to consider are the sample size, representativeness, choice of indicators and whether there is any missing data.

### Sample size

Ensure your sample size is large enough to answer your research question(s). If the sample size is too small for an experimental or quasi-experimental design, it will not be possible to achieve sufficient statistical power and provide a robust answer to the research question(s). It is also important to consider whether you need to provide estimates for population subgroups. The more you break down the sample into groups, the greater the overall sample size needs to be in order to draw statistically significant conclusions about the subgroups of interest. A statistical power analysis helps to estimate the minimum sample size required for a study, given a desired significance level, effect size and statistical power.

### Representativeness

Is your data broadly representative of the target population that is being studied? The generalisability of the research findings may be limited if certain subgroups of the population are not adequately represented in the sample. This is particularly true when differences between population subgroups are related to the outcomes that are being studied.

Some concepts cannot be measured directly and therefore must be proxied by other observable or measurable phenomena, a process called operationalisation. For example, health status is a concept that cannot be observed directly, and therefore researchers need to operationalise the concept by other indicators (e.g. body mass index or smoking status). Uncertainty is introduced when a concept of interest is not operationalised appropriately, and the proxy indicators do not adequately capture that concept or distinguish it from others. You should ask yourself how well the indicators measure the concept that is being studied. Are the assumptions underlying the operationalisation valid?

### Missing data

Missing data or missing values are a common source of uncertainty and can have a significant effect on what can be inferred from the data.

Uncertainty is introduced when data is missing systematically, or in other words, not completely at random. There are two types of systematically missing data: missing not at random (MNAR) and missing at random (MAR).

Missing data is particularly problematic when the reason why data is missing is related to a concept or intervention that is being studied. Data which are MNAR are missing due to reasons related to unobserved outcomes. Data are MAR when the reason the data are missing is related to the observed outcomes (i.e. variables for which we have complete information).

For example, in a study on depression, data would be MNAR if men did not respond to a survey because of their level of depression. This is because the concept of interest (depression in this case) is unobserved.

On the other hand, data on depression would be MAR if men were generally less likely to respond to a survey, irrespective of their level of depression. In this example, sex is a variable that is directly observed.

Reasons for missing data include: social desirability bias in surveys, attrition in longitudinal studies, data entry errors, poor quality data collection instruments, or under-sampling of groups that are difficult to reach. You should ask: is some of the data in your dataset missing? If so, why is it missing?

## Study Design

The design of a study and assumptions about how potential effects will be identified can be a significant source of uncertainty.

### Choice of control group

Uncertainty is increased when the chosen control group is not comparable to the group that is affected by the policy or intervention. In the absence of a valid counterfactual, the estimated impact of a policy or intervention may be significantly biased and the true impact will be uncertain. For example, when the research does not include an independent control group and relies solely on a before-after analysis. The problem of relying on a before-after analysis is that it is not possible to determine whether the observed effects of an intervention would have occurred in the absence of the intervention.

### Before-after comparisons

Binary before-after comparisons can be misleading if they are presented without contextual information. Comparisons from one period to another (such as comparing this week or month to the same period last year) are common. However, they present data out of the context of the underlying trend or do not account for the effect of seasonality. For example, drawing comparisons in outcomes between January 2020 and January 2021 would be misleading as external factors, such as the COVID-19 pandemic, would have had significantly impacted trends. Alternatives to before-after comparisons are discussed in chapter 4, [Mitigating uncertainty]({{< ref "/mitigating_uncertainty" >}}).

### Randomised controlled trials

Randomised controlled trials (RCTs) are the gold standard for testing hypotheses. They involve randomly assigning participants to the intervention or control group. This creates a counterfactual to which you can compare the intervention group. When randomisation is compromised or not possible, there will be greater uncertainty in attributing changes in outcomes to a given intervention.

A few examples of randomisation being compromised are:
- Endogeneity (i.e. when the allocation of an intervention is influenced by the outcome indicator)
- Non-compliance (i.e. when participants who should receive the intervention do not receive the intervention)
- Breach of protocol
- Treatment contamination or spill over (i.e. when participants in the control group are exposed to the intervention). This can be an issue with studies involving cluster randomisation based on geographic areas, such as local authorities.

However, in many contexts randomisation is not feasible or ethical. In these situations, it is possible to employ a quasi-experimental method to create a counterfactual (for more details see the [Magenta Book](https://www.gov.uk/government/publications/the-magenta-book)). Analysts must ask themselves if the design of the counterfactual creates potential for uncertainty in the research findings.

## Analysis

### Statistical analysis

Statistical analysis can present an important source of analytical uncertainty in evaluation design, which may lead researchers to unwittingly make biased or invalid inferences. Analysts should ask themselves if the chosen statistical models accurately describe the relationships between the variables of interest and take account of potential sources of bias. Are effects conditional on other variables, or are they expected to vary across groups? Have potential alternative explanations or theories been explored in the analysis? Have all relevant variables been included in the analysis?

### Interaction effects and heterogeneous treatment effects

Common issues in experimental and quasi-experimental studies include interaction effects. This is when the causal relationships between two variables depend on the state of a moderating variable, or when effects of an intervention vary across different groups (i.e. heterogeneous treatment effects). For example, where the relationship between the dose of a drug and the efficacy of the treatment varies across genders.

When policy interventions have heterogeneous effects, focusing only on aggregate effects and failing to account for differences across groups may lead to invalid inferences. Similarly, uncertainty will result from failing to account for relevant moderating variables in the analysis. Another source of uncertainty results when the statistical model falsely attributes the effect of a missing variable to those variables that are included in the model. This is known as omitted variable bias.

### Interpretation of research findings

The way in which research findings are interpreted can also be a source of uncertainty. An example is the ecological fallacy, in which findings from analysis of aggregate data are erroneously attributed to an individual. For example, research of aggregate data shows that countries where there is a high average fat consumption also have a high breast cancer death rate. If you were to infer from this finding that a woman who has a high fat diet is more likely to die from breast cancer, this would be falling foul of ecological fallacy. The error here lies in the fact that statistical inference is intended to generalise from a sample to a population, and not from a population to an individual. Committing an ecological fallacy can lead researchers to make invalid inferences, thereby creating uncertainty around the true impact of a given policy or intervention.
