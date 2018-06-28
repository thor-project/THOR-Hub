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
The DataCite search is at [http://search.labs.datacite.org](http://search.labs.datacite.org). 

The DataCite search API is at api is based on SOLR and can be found at [http://search.datacite.org/api](http://search.datacite.org/api)

[An example search that returns JSON](http://search.datacite.org/api?q=thor&wt=json)
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
[Datacite search API documentation](http://search.datacite.org/help.html)
[Crossref search API documentation](http://api.crossref.org)