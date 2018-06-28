---
title: "Searching ORCID"
excerpt: ""
---
The ORCID registry can be searched using the v1.2 API.  It supports the SOLR syntax and fields from the bio portion of the ORCID record can be queried.  All query syntaxes available in SOLR 3.6 are supported, including Lucene (with Solr extensions) which is the default, DisMax and Extended Dismax.
[block:api-header]
{
  "type": "basic",
  "title": "External documentation"
}
[/block]
[Official ORCID search api documentation](http://members.orcid.org/api/tutorial-searching-api-12-and-earlier)
[block:api-header]
{
  "type": "basic",
  "title": "Live example - Simple keyword search"
}
[/block]

[block:embed]
{
  "html": "<iframe class=\"embedly-embed\" src=\"//cdn.embedly.com/widgets/media.html?url=https%3A%2F%2Fjsfiddle.net%2FTomDemeranville%2Fdoew6d1u%2F1%2F&src=%2F%2Fjsfiddle.net%2FTomDemeranville%2Fdoew6d1u%2F1%2Fembedded%2F&type=text%2Fhtml&key=02466f963b9b4bb8845a05b53d3235d7&schema=jsfiddle\" width=\"None\" height=\"300\" scrolling=\"no\" frameborder=\"0\" allowfullscreen></iframe>",
  "url": "https://jsfiddle.net/TomDemeranville/doew6d1u/1/",
  "title": "Edit fiddle - JSFiddle",
  "favicon": "https://jsfiddle.net/favicon.png"
}
[/block]

[block:api-header]
{
  "type": "basic",
  "title": "Live example - Parametized search"
}
[/block]
The ORCID serach API supports a wide range of fields (see the documentation below).  For example, we can search for records with a given DOI.  Note how we enclose the DOI with escaped quotes in the query - this is so that we get an *exact* match:


[block:embed]
{
  "html": "<iframe class=\"embedly-embed\" src=\"//cdn.embedly.com/widgets/media.html?url=https%3A%2F%2Fjsfiddle.net%2FTomDemeranville%2Fvhn5m4jn%2F&src=%2F%2Fjsfiddle.net%2FTomDemeranville%2Fvhn5m4jn%2Fembedded%2F&type=text%2Fhtml&key=02466f963b9b4bb8845a05b53d3235d7&schema=jsfiddle\" width=\"None\" height=\"300\" scrolling=\"no\" frameborder=\"0\" allowfullscreen></iframe>",
  "url": "https://jsfiddle.net/TomDemeranville/vhn5m4jn/",
  "title": "Edit fiddle - JSFiddle",
  "favicon": "https://jsfiddle.net/favicon.png"
}
[/block]