---
title: "Querying DOI metadata"
excerpt: ""
---
DOI metadata is available in many formats,  include Bibtex, Citeproc-JSON, RDF as well as XML and JSON specific to Crossref and Datacite.  Crossref and Datacite both support *content negotiation* enabling clients to request DOI metadata in the format most suitable to them.  
[block:api-header]
{
  "type": "basic",
  "title": "External Documentation"
}
[/block]
See the [full content negotiation documentation](http://crosscite.org/cn/) for more details.

[block:api-header]
{
  "type": "basic",
  "title": "Example javascript"
}
[/block]
Crosscite-JSON is a convenient format as it's  usable out of the box by most languages and available from both Crossref and Datacite.  Here is an example, expressed as Crosscite-JSON:
[block:code]
{
  "codes": [
    {
      "code": "{\n  \"volume\" : \"169\",\n  \"issue\" : \"3946\",\n  \"DOI\" : \"10.1126/science.169.3946.635\",\n  \"URL\" : \"http://dx.doi.org/10.1126/science.169.3946.635\",\n  \"title\" : \"The Structure of Ordinary Water: New data and interpretations are \n           yielding new insights into this fascinating substance\",\n  \"container-title\" : \"Science\",\n  \"publisher\" : \"American Association for the Advancement of Science AAAS (Science)\",\n  \"issued\" : { \"date-parts\" : [ [ 1970,8,14 ] ] },\n  \"author\" : [ { \"family\" : \"Frank\", \"given\" : \"H. S.\"} ],\n  \"editor\" : [],\n  \"page\" : \"635-641\",\n  \"type\" : \"article-journal\"\n}",
      "language": "javascript"
    }
  ]
}
[/block]

[block:embed]
{
  "html": "<iframe class=\"embedly-embed\" src=\"//cdn.embedly.com/widgets/media.html?url=http%3A%2F%2Fjsfiddle.net%2FTomDemeranville%2FgL4rzL5f%2F5%2F&src=%2F%2Fjsfiddle.net%2FTomDemeranville%2FgL4rzL5f%2F5%2Fembedded%2F&type=text%2Fhtml&key=02466f963b9b4bb8845a05b53d3235d7&schema=jsfiddle\" width=\"None\" height=\"300\" scrolling=\"no\" frameborder=\"0\" allowfullscreen></iframe>",
  "url": "http://jsfiddle.net/TomDemeranville/gL4rzL5f/5/",
  "title": "Edit fiddle - JSFiddle",
  "favicon": "http://jsfiddle.net/favicon.png"
}
[/block]