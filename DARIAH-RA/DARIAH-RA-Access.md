##Access to Resources
###Definition
(Online) access to resources (datasets). This can be raw data, (Web) applications offering rich access to data, or web services that allow a programmatic access to the data (via an API). 
This type of contribution does not include (national or domain-specific) [aggregators, or metadata catalogues](./DARIAH-RA-Glossary.md#g-agg "glossary description of aggregators and metadata catalogues"), i.e. services that collect information about resources from multiple providers and allow to browse and search in it. These will/can ideally become a source of information about contributions.

It also does not include Web services that process data (see [Processing Services](./DARIAH-RA-Processing.md "Processing Services") contribution).

###Enterprise Viewpoint
####Community
The Access to Resources IKC comprises of the following communities.

* **Data Provision Community:** who provides discovery of, and access to data. Within DARIAH this community can both be represented by a community of researchers/research institutions (that through means of communications, disseminates information about the deposited data, or provides interfaces for the discoverability of the deposited data) or by the same community that provides the storage for the research data. 

####Data Provision Community Roles
The following roles within the Data Provision Community have been identified:

-	**Data Provision Subsystem (passive role):** the community component representing the data provision community. 
-	**Data Owner (active role):** the agent which owns the data
-	**Data Provider (active role):** a person or organization that is responsible for making the research data from the data owner available for the data consumer. 
-	**Data Discovery System (passive role):** a system facilitating discovery of research data and its context.
-	**Documentalist (active role):** an agent who documents data with metadata according to widely accepted standards of **Data Management Community**.
-	**Data Retrieval System (passive role):** a system that enables retrieval of research data. Data retrieval includes access control (and thus, authorization).
-	**Data Consumer (passive/active role):** an agent that requests and receives the research data (for further use). Access to the data may be direct, or mediated via a third-party.

####Data Provision Community Behaviours
The following behaviours are identified in the Data Provision Community:

-	*Data Publication:* A behaviour of the **Data Provider**, the **Data Discovery System** and the **Data Retrieval System** for making research data discoverable and accessible.

-	*Data Discovery:* A behaviour of the **Data Consumer** and the **Data Retrieval System** whereby the data consumer uses the Data Retrieval System to discover data of interest.
-	*Data Retrieval:* A behaviour by the **Data Consumer** and the **Data Retrieval System** whereby the Data Consumer request data or metadata and the Data Retrieval System responds, after successful authorization, with the requested metadata and/or data. The metadata may be used for referral.

Communities that typically collaborate with the **Data Provision Community** are: the **Data Management Community** for improving metadata for discovery, the **Data Processing Community** for harmonisation or just-in-time conversion during access, the **Data Identification Community** for global identification or referral, the **User Authentication Community** for global authentication of **Data Consumers**, and the **Data Creation Community** for capturing enrichments to the provisioned data.

###Information Viewpoint
Differently from the Enterprise viewpoint (where the community was central), for this type of in-kind contribution the information type represents the core of the investigation. The information type needs to be considered in itself, with no reference from the community that created or is responsible for it. 

####Information Object Types:
* *Data:*
	-	*Data Object Type (e.g. Datasets or digitized cultural object):* the minimum available information object type that can be shared from an institution with an end user
	-	*Metadata Object Type:* the information object type that describes and contextualizes the data object type
	-	*Web Applications (Service Object Type) (e.g. web interfaces, portal, faceted research):* the information object type that translates the data object type (in raw format) into a comprehensible information object for the end user. 
-		*Transfer Service Object Type (e.g. API, OAI-PMH, FTP):* the information object subsystem that makes it possible for the researcher to access the data
	-	*AAI response:* Object derived from the authentication service

* *Agents:*
	-	*Data Owner:*	 the agent who owns the data that are made accessible 
	-	*Data Consumer:* the agent who access the data 
	-	*Data Manager:* the agent who makes sure that the quality of the data is met and that the user experience is satisfactory

* *Services:*
	-	*User guide/ manual:* information on how to access the resources
	-	*[AAI](./DARIAH-RA-Glossary.md#g-aai "glossary description of AAI"):* (**Authentication Subsystem**) information object about the user in order to access the resources

* *Contracts:*
	-	*Contract:* e.g. reuse licenses and intellectual property rights clearance
	-	*Agreement:* An agreement (e.g. a standard) defines the choice by a community to use a certain standard in order to harmonise the access to the data and metadata.

<table><tr><th>
Case Study: the CENDARI AtOM
</th></tr>
<tr><td>
The [CENDARI project](https://archives.cendari.dariah.eu/index.php/ "CENDARI Archival Directory") ran from January 2012 to January 2016 funded under the FP7 grant scheme.  CENDARI created a data space whose data have been created in two different ways. On the one hand memory institutions and aggregators delivered their data to the CENDARI federated data space. On the other hand, CENDARI made available hundreds of the so-called “hidden collections” from European archives: these collections were not aggregated by third-party institutions, nor were they digitised - in fact they often belong to small archives whose digitisation resources are often lacking. Rather, the CENDARI researchers manually encoded in a structured format the metadata describing those collections, by making these collections discoverable and reusable for the first time. 

From an enterprise viewpoint, the **Data Provision Community**, in this case the CENDARI researchers, played a crucial role in this contribution, by providing a first and unique access to resources that otherwise would have never been accessible. The **Data Provision Community** related directly with the data owner, which in this case is represented by the Archive, who owns and archives the original documents and artefacts. 
The **Data Discovery System** - the tool [AtOM](https://www.ica-atom.org/ "ICA-AtOM home page") in our case, facilitates the discovery of the research data and their context; AtOM also acts as the **Data Retrieval System**, which is a passive role as its actions are not tangible directly, but nonetheless allow actions like user-control and thus authorisation. 

From an information viewpoint, the user interface represents the information object *“web applications”*, as it translated the data object type into a comprehensible information object for the end user. 
In the case of AtOM, then, the Data object type, can be described in tight connection with the metadata object type, as in our case the object is purely made of metadata, without any object attached to it. 
In terms of service…
</td></tr>