---
title: "Searching DOI metadata"
excerpt: ""
---
Both Datacite and Crossref have simple REST-like search endpoints.  
[block:api-header]
{
  "type": "basic",
  "title": "Datacite Search"
}
[/block]
The DataCite search is at [http://search.datacite.org](http://search.datacite.org). 

The DataCite search API is at api is based on SOLR and can be found at [http://api.datacite.org/](http://api.datacite.org/)

[An example search that returns JSON](https://api.datacite.org/works?query=thor)
[block:api-header]
{
  "type": "basic",
  "title": "Crossref search"
}
[/block]
The crossref search is at [http://search.crossref.org](http://search.crossref.org). The CrossRef search API can be found at [http://api.crossref.org](http://api.crossref.org)

[An example search that returns JSON](https://api.crossref.org/works?query=thor)
[block:api-header]
{
  "type": "basic",
  "title": "External documentation"
}
[/block]
[Datacite search API documentation](https://support.datacite.org/v1.1/docs/api)
[Crossref search API documentation](http://api.crossref.org)