---
title: "Introduction for integrators"
excerpt: ""
---
The information you need to start integrating persistent identifiers [PIDs](doc:introduction-to-persistent-identifiers) depends on your use cases.  Some services will be concerned with creating  [DOIs](doc:what-is-a-doi)  while others simply need to query the metadata.  Likewise, some systems may require authenticated [ORCID IDs](doc:explaining-orcid) to aid interoperability, others will want to retrieve metadata or update records.
[block:api-header]
{
  "type": "basic",
  "title": "Integrating DOIs"
}
[/block]
## Querying DOI metadata

Querying DOI metadata is as simple as making a request to the DOI URL using content negotiation.  See [Accessing DOI metadata](doc:accessing-doi-metadata) for more details.

## Searching DOI registries

Searching DOI registries is complicated by the fact there is more than one of them.  Each offers its own search API.  [Searching DOI registries](doc:searching-doi-registries) contains more information.

## Creating DOI metadata

Creating DOI metadata is a bit more complex.  You need to work with a DOI registration agency, become a member, create XML in the correct format and submit it.  Workflows vary between registrars.  [Creating DOIs and DOI metadata.](doc:creating-dois-and-doi-metadata) explains this in more detail.
[block:api-header]
{
  "type": "basic",
  "title": "Integrating ORCID"
}
[/block]
ORCID has a [Public API](doc:orcid-public-api-tutorial) and a [Member API](doc:orcid-member-api-tutorial).  At a high level, the public API is read only and the member API allows updates.  With the user's permission, the member API also enables you to query data users have marked as 'limited access' and set up notifications.

There are other differences so make sure you understand the difference and choose the right one for your use case.

## Querying ORCID metadata

The ORCID API enables client applications to retrieve biographical information about a researcher and their works, peer review activities, education and employment.  The [ORCID Public API](doc:orcid-public-api-tutorial) section contains a couple of examples and further information.

## Updating ORCID records
Updating records requires the [ORCID Member API](doc:orcid-member-api-tutorial).  With the members permission, you can add and update an ORCID record.

## Authenticating ORCID users

ORCID uses OAuth to authenticate users and authorise actions with the API.  The two-step (application) flow is used to access public data or authenticate a user.  Actions that require user authorisation use the three-legged approach.  See the [ORCID API - Authenticating users](doc:orcid-api-authenticating-users) section for more details.

## Searching the ORCID registry

ORCID exposes a SOLR endpoint for machine to machine searching.  [Searching ORCID](doc:searching-orcid) explains how this works with examples.
[block:api-header]
{
  "type": "basic",
  "title": "External information"
}
[/block]
There is a great [integration presentation on the ORCID website](https://orcid.org/organizations/integrators) that walks through the integration process.  There is also [extensive ORCID API documentation](http://members.orcid.org./api)

There is an excellent [help system at Crossref](http://help.crossref.org/) and [API documentation at Datacite](https://mds.datacite.org/static/apidoc)

Crosscite.org contains detailed information about using content negotiation to [resolve DOIs into metadata](http://www.crosscite.org/cn/).