---
title: "Communication basics"
draft: false
weight: 4
summary: 
---

## Identify who your audience is

As mentioned earlier, knowing who your audience is, what their interest is in this analysis, and how they interpret evidence will determine how you communicate. Test your communication with the audience, do they understand the key message from your prose or visualisations?

## Assess whether to describe uncertainty in words or attach figure

How something is written has a major impact on how people perceive the uncertainty. [Research shows](https://www.tandfonline.com/doi/abs/10.1080/17457289.2018.1465061) that analysis is seen as less reliable if the outputs are conveyed only in words.  Numbers should be presented within a sentence if possible as this helps give context, making them easier to read and understand.

To avoid any possible confusion between analytical conclusions and the uncertainty surrounding them, it is good advice to [“keep your expressions of the magnitude of uncertainty clearly separate from the magnitude of any evidence you are trying to communicate” (pdf)](https://royalsocietypublishing.org/doi/pdf/10.1098/rsos.181870), while ensuring that caveats to the overall conclusions cannot be disregarded.

Descriptive terms such as ‘low risk’ or ‘very likely’ can be [interpreted very differently by different people](https://www.tandfonline.com/doi/full/10.1080/02684527.2014.994955). Where possible, it is sensible to attach a numerical probability and use these descriptive terms in support. Emerging research suggests that [numerically defined uncertainty is more trusted than worded statements](https://www.pnas.org/content/117/14/7672) and, in fact, people find worded statements of uncertainty difficult to interpret and may entirely ignore the implication of worded statements in demonstrating that numbers are uncertain.

An exception to this is where there is an established system that your audience is used to for attaching terminology to probabilities and mapping between verbal, pictorial and numerical articulations of uncertainty. There are a variety of scales like this and they differ considerably in how they align verbal expressions to numerical articulations:

- [According to the IPCC (Intergovernmental Panel on Climate Change) (pdf)](https://www.ipcc.ch/site/assets/uploads/2017/08/AR5_Uncertainty_Guidance_Note.pdf) “very likely” means 90-100% probability.
- [According to NICE (National Institute for Health and Care Excellence)](https://bnf.nice.org.uk/guidance/adverse-reactions-to-drugs.html) probabilities of between 1 in 100 and 1 in 10 are referred to as “common”. 
- [According to GLD (Government Legal Department)](https://www.gov.uk/government/publications/guidance-note-on-legal-risk) “high likelihoods” are those greater than 70%.
- [According to PHIA (Professional Head of Intelligence Assessment)](https://www.app.college.police.uk/app-content/intelligence-management/analysis/delivering-effective-analysis/) , >=95% is “almost certain”. 

Presenting the likelihood of success [may be perceived differently (pdf)](https://www.uzh.ch/cmsssl/suz/dam/jcr:00000000-64a0-5b1c-0000-00003b7ec704/10.05-kahneman-tversky-79.pdf) to presenting the corresponding likelihood of failure. Present the information both ways to avoid bias (e.g. “there is an 80% chance of success and a 20% chance of failure”). By adding in the chance of failure, you remind the reader that it exists and how large it is, which may otherwise be overlooked. Visual part-to-whole comparisons can help with this. See the [infographics section]({{< ref "presenting_uncertainty/infographics">}}) for more details.

## Decide how to present your numbers

Research shows that there is no clear preference for choosing between probabilities and fractions (e.g. 10% probability, or 1 out of 10). Given this, [the usual preferences of the audience or the ‘norm’ within the organisation should be followed (pdf)](https://www.annualreviews.org/doi/pdf/10.1146/annurev-statistics-010814-020148) and you should stick to the same format (i.e. do not mix probabilities, fractions, ratios in the same report). Some people are more familiar with percentages than fractions or ratios and articulations such as “1 in 100” in [research contexts](https://www.pnas.org/content/117/14/7672) can risk the misinterpretation that research has only been done on 100 people. 

If using fractions, [keep the denominator constant](https://www.ncbi.nlm.nih.gov/pubmed/24625237) (e.g. “1 in 100 vs. 2 in 100”, rather than “1 in 100 vs. 1 in 50”) and as small as possible while keeping to integers (e.g. “1 in 100” rather than “10 in 1,000”), rounding if appropriate.

Be clear on the specifics and applicability. Saying a ‘10% chance of rain’ is meaningless unless you also state the time period – e.g. in the next hour, or at some point tomorrow – and location.

If the outputs are only intended for use within a specific frame (for example, a specific area or to a particular group of the population), then make sure this is clearly stated alongside the outputs.

Consider the overall uncertainty in the numbers you have calculated. Round them appropriately to avoid spurious accuracy (e.g. perhaps 40% rather than 38.7% if the overall uncertainty is greater than one percentage point).

Presenting a single figure is best avoided as it can give a misleading impression of precision (e.g. “between 1,200 and 1,800”, rather than “1,500”). Further, emerging research (see [here](https://www.pnas.org/content/117/14/7672) and [here (pdf)](https://royalsocietypublishing.org/doi/pdf/10.1098/rsos.181870)) suggests that ranges are better than point numbers for ensuring that decision makers understand that a number is uncertain at all.

Commissioners may request a ‘best estimate’ for ease of onward use, but you must consider the risks in providing this. Try to understand how they intend to use the analysis, so you can provide something that meets their needs while also acknowledging the uncertainty.

Stating a range may be perceived as a uniform distribution across the range. Conversely, stating a range around a best estimate may be perceived as a triangular distribution (or Normal with analytical audiences). The output distribution could of course also be asymmetric or bi-modal. Consider which of these best reflects the actual uncertainty when deciding what to present.

Don’t simply use 95% confidence intervals by default. Think about what the outputs are going to be used for (see [Jointly agreeing how uncertainty should be used](ADD LINK), and discuss the level of risk and uncertainty that the decision maker wants to plan for – this might not be 5%.

Be clear what confidence level you are using and ensure your audience understands what this means (avoiding precise statistical definitions if it will increase comprehension).

People interpret visualisations differently. Always have a title with the key message, otherwise people may not have the time to interpret the visualisation or misinterpret the key message.
