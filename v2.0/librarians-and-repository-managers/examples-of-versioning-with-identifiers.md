---
title: "Case study: Versioning with identifiers"
excerpt: ""
---
Digital research objects are more flexible and mutable than their physical or analogue counter parts. As access to data at the point of citation is key to reproducibility, there is a need for more consideration of how we describe and identify them. This article highlights some examples of how various organisations are managing the versioning and granularity of their digital content.

## Case studies in the social sciences
Social science research produces a number of longitudinal datasets. These datasets are regularly updated as new data is collected, often on the same research participants. This causes a problem for reproducibility if data that is cited is later changed - it could make it impossible to accurately reproduce and earlier analysis of that data.

One approach to using identifiers to version data is taken by the UK Data Archive. The UK Data Archive holds a large number of longitudinal studies, some updated on an annual basis, or more regularly.

Rather than simply update the original data, each new data collection 'wave' is stored discretely. Each new wave is then assigned its own DOI and so its own citation.

In order to help the user navigate these versions, each DOI resolves to the same landing page as the other data for the same study. In this way, user accessing the data from a later wave can still discover and access earlier data and vice versa. An example of this can be seen with the following items:
[block:callout]
{
  "type": "success",
  "body": "Office for National Statistics. Social Survey Division and Northern Ireland Statistics and Research Agency. Central Survey Unit, Quarterly Labour Force Survey, January - March, 2011: Special Licence Access [computer file]. Colchester, Essex: UK Data Archive [distributor], December 2011. SN: 6903, [http://doi.org/10.5255/UKDA-SN-6903-1](http://doi.org/10.5255/UKDA-SN-6903-1)"
}
[/block]

[block:callout]
{
  "type": "success",
  "body": "Office for National Statistics. Social Survey Division and Northern Ireland Statistics and Research Agency. Central Survey Unit, Quarterly Labour Force Survey, January - March, 2011: Special Licence Access [computer file]. 5th Edition. Colchester, Essex: UK Data Archive [distributor], March 2015. SN: 6903, [http://doi.org/10.5255/UKDA-SN-6903-5](http://doi.org/10.5255/UKDA-SN-6903-5)"
}
[/block]


This is a simple solution providing versions of your data are stored as separate files. It is more complicated if additional data are absorbed into a single aggregated dataset. 

The UK Data Archive's Nesstar tool, and the National Survey of Health and Development have data that is stored in aggregate, with data of interest extracted for research on a case-by-case basis. Potential approaches to citation of data versions in that form discussed in the ODIN project. See: Consortium, ODIN; Rueda, Laura; Dallmeier-Tiessen, Sünje; Kotarski, Rachael; Newbold, Elizabeth; Herterich, Patricia; Lavasa, Artemis; Brown, Josh (2015): D3.3: Proofs of concept and commonality. figshare. 
[https://doi.org/10.6084/m9.figshare.1373665](https://doi.org/10.6084/m9.figshare.1373665). 

## Identifying Works, Expressions, Manifestations and Items
The THOR project is looking in more details of how identifiers can be applied to 'versions' of a research object in the FRBR model. Case studies resulting from this work will be included here as the work develops.