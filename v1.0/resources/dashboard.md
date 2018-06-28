---
title: "THOR Metrics Dashboard"
excerpt: ""
---
THOR has developed a dashboard to monitor the evolving landscape of persistent identifiers (PIDs) over the life of the project and beyond. Access the dashboard at: 

http://dashboard.project-thor.eu
[block:api-header]
{
  "type": "basic",
  "title": "Audience"
}
[/block]
The dashboard is intended for repository managers, integrators, policy makers, and all others interested in the interplay of persistent identifiers broadly. Its role is that of a high level aggregator of PID information. The dashboard does not have the level of granularity necessary to be used as a tool for monitoring outputs of individual researchers. 
[block:api-header]
{
  "type": "basic",
  "title": "Data Sources"
}
[/block]
The dashboard harvests publicly available information from the following sources:
* DataCite Metadata Search
  * Documentation - https://search.datacite.org/help.html
  * API endpoint - http://search.datacite.org/api
* ORCID Statistics
  * Documentation - https://pub.orcid.org/v2.0_rc1#!/Statistics_API_v2.0_rc1/
  * API endpoint - https://pub.orcid.org/v2.0_rc1/statistics
* CrossRef 
  * Documentation - http://api.crossref.org/
  * API endpoint - http://api.crossref.org/
[block:api-header]
{
  "type": "basic",
  "title": "Sharing"
}
[/block]
The dashboard code is Open Source. It is available on GitHub in two parts: 
* Dashboard (for visualization of the data) - http://github.com/thor-project/dashboard
* Data Harvester (for aggregating the data) - http://github.com/thor-project/data-harvester

A tutorial to create your own metrics dashboard can be found here:
https://thor-project.github.io/dashboard-tutorial/