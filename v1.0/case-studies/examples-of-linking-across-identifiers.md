---
title: "Examples of linking across identifiers"
excerpt: ""
---
There are three important uses for linking persistent identifiers:
  * linking between [versions](#section-versions) of research outputs, particularly data
  * linking between articles and their [supporting data](#section-related-works) and code
  * linking between research outputs and their [contributors, institutions and funding sources](#section-linking-creators-and-contributors).

These links are important for navigating the research landscape, but also allow us to look at the far reaching impact of each individual contributor, paper, dataset and grant.

Here we will give examples of how data repositories have linked identifiers to give us a much better view of research networks and dependencies.
[block:api-header]
{
  "type": "basic",
  "title": "Versions and related works"
}
[/block]
Many repositories using DataCite to assign DOIs to their content use their metadata to make links between resources. The [DataCite metadata schema](doc:datacite-metadata-schema) contains the field RelatedIdentifier which makes this possible. This field explains the relationship and gives the identifier locating the related item.

##Versions
The UK's [Archaeology Data Service](http://archaeologydataservice.ac.uk) uses the RelatedIdentifier to show the relationship between different versions of a dataset. More information on versioning data can be found in [Examples of versioning with identifiers](doc:examples-of-versioning-with-identifiers).
[block:code]
{
  "codes": [
    {
      "code": "<relatedIdentifiers>\n\t<relatedIdentifier relatedIdentifierType=\"DOI\" relationType=\"IsNewVersionOf\">10.5284/1000417</relatedIdentifier>\n\t<relatedIdentifier relatedIdentifierType=\"DOI\" relationType=\"IsNewVersionOf\">10.5284/1000341</relatedIdentifier>\n</relatedIdentifiers>",
      "language": "xml",
      "name": "XML showing related identifiers for http://doi.org/10.5284/1011897"
    }
  ]
}
[/block]
##Related works
This dataset from [Durham University](http://durham.ac.uk) links to the paper that has cited the data, as well as the software that was used during creation of the data.
[block:code]
{
  "codes": [
    {
      "code": "<relatedIdentifiers>\n    <relatedIdentifier relatedIdentifierType='URL' relationType='IsCitedBy'>http://dx.doi.org/10.1016/j.ssnmr.2015.05.003</relatedIdentifier>\n    <relatedIdentifier relatedIdentifierType='URL' relationType='Cites'>https://www.dur.ac.uk/solids.nmr/software/pnmrsim/</relatedIdentifier>\n</relatedIdentifiers>",
      "language": "xml",
      "name": "XML showing related identifiers for http://doi.org/10.15128/KK991FK96D"
    }
  ]
}
[/block]
In order to make this a bi-directional link, the persistent identifier, expressed as a URI, should also be used by papers citing data and code.

Outside of DOIs, the [EBI](http://www.ebi.ac.uk) provides a number of life science data resources. Many of these link to related data across the EBI services, as shown in the image below.
[block:image]
{
  "images": [
    {
      "caption": "Cross-linking of major life science resources at EMBL-EBI (source: EMBL-EBI)",
      "image": [
        "https://files.readme.io/UIuwpcLREqpGFD39RDnA_ebilinks.png",
        "ebilinks.png",
        "590",
        "576",
        "#b8956e",
        ""
      ]
    }
  ]
}
[/block]
##Alternate identifiers
The DataCite metadata schema also allows for secondary identifiers that relate to the exact same object. These alternate identifiers tend to be internal IDs or local accession numbers, which are not necessarily globally unique, but may provide additional context. For instance, the InChI for data relating to specific chemical compound:
[block:code]
{
  "codes": [
    {
      "code": "<alternateIdentifiers>\n\t<alternateIdentifier alternateIdentifierType=\"InChI\">InChI=1S/C6H10NO2.2H2O/c1-3-4(2)6(9)7-5(3)8;;/h3-4H,1-2H3,(H2,7,8,9);2*1H2/t3-,4-;;/m0../s1</alternateIdentifier>\n  <alternateIdentifier alternateIdentifierType=\"InChIKey\">UQPNWVSPCKRRTR-RGVONZFCSA-N</alternateIdentifier>\n  <alternateIdentifier alternateIdentifierType=\"Handle\">10042/132754</alternateIdentifier>\n</alternateIdentifiers>",
      "language": "xml",
      "name": "XML showing alternative identifiers for http://doi.org/10.14469/CH/127757"
    }
  ]
}
[/block]
For more on how to integrate DataCite in to you repository, see [Examples of DataCite integration](doc:examples-of-datacite-integration-1).

Across the EBI, many services have multiple identifiers, which can reflect the evolution of a resource. A small group of services have DOIs alongside original accession numbers, although practice is not widespread.
[block:api-header]
{
  "type": "basic",
  "title": "Linking creators and contributors"
}
[/block]
The metadata for an item can also be used to link to the identity of its creators and contributors. The DataCite metadata also supports name identifiers. The example below is for data held in [PANGAEA](https://www.pangaea.de/).
[block:code]
{
  "codes": [
    {
      "code": "<creator>\n  <creatorName>Dengler, Marcus</creatorName>\n  <nameIdentifier nameIdentifierScheme=\"ORCID\" schemeURI=\"http://orcid.org\">0000-0001-5993-9088</nameIdentifier>\n</creator>",
      "language": "xml",
      "name": "XML showing nameIdentifiers for http://doi.org/10.1594/PANGAEA.858896"
    }
  ]
}
[/block]
In many cases, contributors are individuals, but the vocabulary for the Contributor field allows exploration of organisational relationships. Contributors and Creators can be organisations, but there are contributorTypes that relate specifically to organisations. These are:
  * Distributor
  * Funder
  * HostingInstitution
  * RegistrationAgency
  * RegistrationAuthority
  * ResearchGroup

The question of appropriate identifiers for organisations is an open one, but there are examples of organisation identifiers in DataCite:
[block:code]
{
  "codes": [
    {
      "code": "<creators>\n    <creator>\n      <creatorName>UCD Archives</creatorName>\n      <nameIdentifier nameIdentifierScheme=\"ISNI\">0000000404462544</nameIdentifier>\n    </creator>\n</creators>",
      "language": "xml",
      "name": "XML showing the organisation ID included in http://doi.org/10.7925/DRS1.UCDLIB_38829"
    }
  ]
}
[/block]
ORCID has been using ISNIs as organisation identifiers for some time, and so it is possible to link datasets without organisational information to relevant organisations via the ORCID records of its individual creators and contributors. For instance, for our ORCID example in PANGAEA above, we can see that the creator is employed by the Helmholtz Centre for Ocean Research Kiel and so the data is related to that organisation (ISNI:0000-0000-9056-9663). 

##Versions of identities
There are disciplines where people may wish to create separate identities and have separate identifiers and records for them. In such cases, ORCID does not link between identifiers. However, unintentional duplicate ORCID iDs do occur. To deal with this, ORCID depreciates one iD and ensures that it points to the primary record.This ensures the persistence of the depreciated ORCID iD, but allows users to navigate to the appropriate record.


[block:callout]
{
  "type": "success",
  "body": "Fenner, Martin et al.. (2016). THOR: Conceptual Model of Persistent Identifier Linking. Zenodo. http://doi.org/10.5281/zenodo.48705",
  "title": "Content for this article was drawn from:"
}
[/block]