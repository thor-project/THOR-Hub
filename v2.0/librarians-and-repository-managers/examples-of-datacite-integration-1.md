---
title: "Case study: DataCite workflow integration: Humanities and Social Sciences"
excerpt: ""
---
Assigning DOIs with DataCite in repositories can be integrated into repositories at various stages in the [workflow for content management](doc:repository-workflows). The most common point for assigning DOIs is as part of the ingest process, so that as soon as the item is published it is made available with a DOI for citation.

Below are summaries of what that integration looks like within repositories for social sciences, high energy physics and humanities, with brief reference to their metadata.

For more more detailed explanations of how the workflows of these repositories were adapted to integrate DataCite DOIs, please see the following report:
[block:callout]
{
  "type": "success",
  "body": "Consortium, ODIN; Rueda, Laura; Dallmeier-Tiessen, Sünje; Kotarski, Rachael; Newbold, Elizabeth; Herterich, Patricia; Lavasa, Artemis; Brown, Josh (2015): D3.3: Proofs of concept and commonality. figshare. [https://doi.org/10.6084/m9.figshare.1373665](https://doi.org/10.6084/m9.figshare.1373665)",
  "title": "These workflow case studies are taken from:"
}
[/block]
## Case study in humanities
Our case study from the humanities is centered on the [Archaeology Data Service](http://archaeologydataservice.ac.uk), based in York in the United Kingdom. As THOR develops, we will also be including the British Library's [EThOS](http://ethos.bl.uk) service, which provides discovery and access to UK electronic theses.

The Archaeology Data Service (ADS) holds data collections and grey literature produced during archaeological investigations. Collections submitted to the ADS are manually checked by an ADS archivist. The archivist curates the submissions before assigning a DOI to the collection at the point of publication. 

A click of a button is all that is required within ADS's bespoke collection management system to send metadata to DataCite and assign the DOI. Archivists can view the latest metadata held by the collection management system and the metadata as sent to DataCite side-by-side. This allows them to verify whether the metadata held by DataCite can and should be updated. The archivist can also view the associated landing page and update the DOI if the landing page URL changes.

The ADS assign a new DOI for each version of an item, and associated versions through the RelatedIdentifier field. For more information on versioning, see [Examples of versioning with identifiers](doc:examples-of-versioning-with-identifiers).

## Case study in social sciences
Our case study from the social sciences is centered on the [UK Data Service](http://ukdataservice.ac.uk), based at the University of Essex. The UK Data Service (UKDS) provides archiving for a wide range of social science data from various sources, including government, business and research. As the sources and types of data it receives are broad, it has more than one repository and so more than workflow for assigning DOIs. In general, DOIs are assigned during the ingest process, after quality assurance by the UKDS team. Approval of data by service administration is a one-click process, which also integrates assignment of the DOI using the DataCite API (see [Creating DOIs and DOI metadata.](doc:creating-dois-and-doi-metadata)). During the approval and DOI assignment process, the UKDS send only the mandatory metadata to DataCite.

For both the ADS and UKDS, assigning data on ingest is very much dependent on the way that data is stored and accessed. During investigation of the workflows of social science data repositories, we also looked at the [National Survey of Health and Development](http://nshd.mrc.ac.uk) (NSHD) a longitudinal study which has been following participants since 1946. 

Rather than storing each new data collection event as a separate object, NSHD stores a single dataset, new data combined with older. Researchers do not access and use the whole dataset, but apply to use specific data and variables of interest that are extracted by the NSHD team for them. This model means that assigning DOIs on ingest would not represent how the data is stored and used, and so would not support reproducibiltiy of the research. Instead, a workflow was considered where DOIs are assigned to the data that is extracted for reuse. While this model has not yet been implemented at the NSHD, it is actively being used in other domains, such as for the [Sir Alister Hardy Foundation for Ocean Science](http://sahfos.ac.uk).
[block:callout]
{
  "type": "success",
  "title": "Sir Alister Hardy Foundation for Ocean Science (SAHFOS)",
  "body": "SAHFOS is a not-for-profit organisation that provides continuous plankton recorder data for oceanographic research. This dynamic data is stored as a single object, with data of interest extracted byt the SAHFOS team on behalf of researchers. DOIs cannot be assigned on ingest, as those DOIs would not be representative of the SAHFOS data that is used in research.\n\nInstead, the SAHFOS team assign DOIs to each subset that they extract and make available to requesters. For example:\nSAHFOS; (2015): Plankton Data for the North Atlantic 20150416; SAHFOS. [http://doi.org/10.7487/2015.106.1.900](http://doi.org/10.7487/2015.106.1.900)"
}
[/block]