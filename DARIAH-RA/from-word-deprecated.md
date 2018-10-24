1. Introduction
1.1 Why a reference architecture for DARIAH-EU? 
The project Humanities at Scale (http://has.dariah.eu/) is currently developing a service for the submission of the in-kind contributions for the DARIAH-ERIC member states. Currently, the in-kind contributions delivered to DARIAH-EU are submitted via a FileMaker database, which has been customized by the DARIAH-EU team in the last years. This system fulfilled its goals in the starting years of the DARIAH ERIC, but it doesn’t meet the requirements of stability and scalability that are requested in this growing phase of the infrastructure.
 
This document aims to develop a reference architecture   for the submission of in-kind contributions of DARIAH EU. This reference architecture develops in parallel with the current documentation on the in-kind contributions developed by WP5: in fact, it further develops their definition and components by using a formal language, borrowed from the theoretical models used in ICT systems.
 
The main goals of such reference architecture are:
 
1.	To communicate and to describe contributions in a common language and to have a common understanding of what components should be described. The in-kind contributions have never been formally described before, including their creation processes. The result is that up to now the contributions have been interpreted and labelled in different ways by each contributing country, by making the in-kind registry highly heterogeneous and unreliable from an end user perspective.
 
2.	To facilitate the description of the interactions between components of the in-kinds, according to the services or functions they provide. How do the components of the contributions interact? How are they connected? What this reference architecture brings to life is not only a reliable description of the DARIAH contributions, but their description as processes and evolving systems, rather than immovable objects. We think therefore that it is important to describe these changes and interactions with the environments in which the contributions evolve.
 
3.	To offer an architectural reference for other projects and infrastructures that wish to offer similar services to their (research) communities. 

4.	To Mitigate and Reduce the risk. We consider this reference architecture as a way to reduce the risk mainly derived from point 1: that of interpreting the in-kind contributions in different ways, to describe them without a common reference model. This risk exists not only among partners inside the same research infrastructure but also for anyone who accesses the DARIAH contributions from other infrastructures. 
1.2 Methodology
In the process of creating a Reference Architecture for the DARIAH in-kind contributions, we were able to count on the support of already existing reference models and reference architectures, both in the fields of ICT, humanities and social sciences

The models that we used as a reference for our architecture are well known models implemented in the design of ICT processes like the RM-ODP (Reference Model - Open Distributed Processing). 
In addition, a recently developed model as the RM-SSH (Reference Model for Social Science and Humanities) for social sciences and humanities developed by the DASISH project provides a more specific reference model for our work on the DARIAH ERIC, whose field of action is in the digital arts and humanities. 

A.	RM-ODP Reference Model 

Reference Model of Open Distributed Processing (RM-ODP) is a reference model in computer science which provides a framework to describe the architecture of open distributed processing (ODP); whenever possible RM-ODP uses a formal description techniques for specification of the architecture, in order to guarantee consistency and reliability of such description. 

This framework is composed of two main approaches:
•	Object modelling: Object-oriented modelling (OOM) is an approach used to model applications and systems by applying the object-oriented paradigm to the entire system. Object modelling usually applies to the modelling of dynamic systems (e.g. business processes) as well as to static structures (components of a system)

•	The description of the system in different viewpoints (Viewpoint Modelling): it is an effective approach when dealing with complex systems as It represents the subdivision of the specification of a complete system. Despite being relatively independent, the viewpoints are interconnected as some of the key items are identified in other viewpoints. 


 
		    Figure 1: overview of the RM- ODP Reference Model viewpoints

Enterprise viewpoint: allows to focus on the purpose, scope and policies of a system by describing interrelated communities. These communities are described by community contracts which contain the objectives, roles, policies and behaviour.  The SSH Data Infrastructure is composed of the following communities:

•	Data Creation Community, who gather data from deployed instruments, 
•	Data Management Community, who ingest, administer and curate data, 
•	Data Provision Community, who provide discovery of, and access to data, 
•	Data Processing Community, who generate processed data from deployed processes, 
•	Data Identification Community, who provide resolution of identifiers for research data,
•	User Authentication Community, who provide federated authentication services for users.

Information viewpoint: the focus is on the information object without considering representation, implementation or distribution details. The aim of the information viewpoint is to provide a common understanding of the model of the shared information for all stakeholders of the reference model. The information viewpoint is independent from functions that transform and manipulate the data and the computational interfaces. This viewpoint defines a configuration of information objects, their behaviours, actions that can be performed upon the information object and constraints. Those information objects are: 

•	Data: Data information object types can be content objects (observation, concept, and metadata), or container objects (dataset, inventory) grouping similar content object types.
•	Agents: Agents are typically human users or machines acting on behalf of human users.
•	Service: Services can be human- or automated services and are described by their behaviour or interaction.
•	Contracts: Contracts usually exist between two agents, whereas standards exist within a community. They are used to describe agreements between two agents or within a community.

Computational viewpoint: describes the functionality of a system. It decomposes the system into objects performing specific functions with specific interfaces. The viewpoint is expressed using an object model which defines the interfaces that objects can have, how these can be bound with other interfaces, the interaction that can take place at these interfaces and the actions that an object can perform (such as creation of new objects, interfaces and bindings).

[In our deliverable, we won’t work on the engineering viewpoint. Probably we won’t take it into consideration for DARIAH/HaS.
The engineering viewpoint:  focuses on the mechanisms and functions required to support distributed interactions between objects in the system]



B. DASISH SSH Social Sciences and Humanities Data Infrastructure Reference Model

The DASISH project  developed a Reference Model based on the previous observation that there was a lack of understanding of research infrastructures and the relationships between their entities: as Research Infrastructures are distributed infrastructures, they gather numerous stakeholders and have complex organisations. Their structure and functioning is therefore not always clear to an external user. 
In this context, RM-ODP appears to be the most pertinent model to describe them, by providing definition of the core entities and their archetypal distribution.  

 
Figure 2: SSH Data Infrastructure Community, its Data Infrastructure Community and other communities
1.3 Further Development
This reference architecture is the first attempt, and a work-in-progress, to create a reference architecture in the Social Sciences and Humanities and the first based upon the SSH reference model. As such, it required validation against existing and future architectures for services and activities in DARIAH, and elsewhere.
Moreover, it requires further development of the viewpoints, and in particular the computational viewpoint, for DARIAH contribution subtypes (see chapter 3). This will aid the understanding of the computational viewpoint with concrete examples of how the described computational objects interact. Naturally the glossary needs refinement, because, as with all first drafts, it is never complete.
Furthermore, feedback from users of the reference architecture is essential to the further development as well as a governance structure for future releases.
2. Glossary
Activity: In general terms, an activity can be described as one or a set of actions, performed by an agent (single or institution) in order to achieve a result or product that can be shared with another agent. Differently from a service, an activity is discrete, as it is marked by a beginning and an end. 

Cultural Heritage Object: analogue and original physical object or its digital representation of an artefacts from a cultural heritage institution 

Cultural Heritage Institution: Institution that preserves the cultural heritage objects and that makes available digitally cultural object and/ or metadata of specific collections to researchers.

Archival Information Package: The definition of the term Archival Storage in OAIS includes the services and functions necessary for the storage of the Archival Information Package (AIP). Archival storage encompasses data management and includes processes such as storage media selection, transfer of AIP to storage system, data security and validity, backup and data restoration, and reproduction of AIP to new media. (IASA)

DARIAH-EU: Digital Research Infrastructure for Arts and Humanities. DARIAH is a European research infrastructure (ERIC).  It connects several hundreds of scholars and dozens of research facilities in currently 17 european countries, the DARIAH member countries. People in DARIAH provide digital tools and share data as well as know-how. They organize learning opportunities for digital research methods, like workshops and summer schools, and offer training materials for the Digital Humanities.

DARIAH (affiliated) Institutions and Projects: initiatives whose activity and even existence are closely related on the technical and strategic background established by DARIAH (and vice -versa) 

Data: digitized version of an existing object (when referred to a cultural heritage object); it can be research data (input or outcome of research, conducted through digital means); it can be information (e.g. data about a certain topic, which can be collected and stored)

Information object: Information objects model the data about entities in the real world, their state and behaviour and interactions with other information objects. An information object has a type that share a common set of features and behaviours (RM- SSH, DASISH)

Information object type: The information types are identified from an inventory of the communities. These were then abstracted to common information types that are independent of the communities into four categories: Data, Agent, Service and Contract. 

In-kind contribution (IKC): “the provision of goods or services to an organisation by one of its members, valued in monetary terms according to rules agreed upon beforehand by the members of the organisation, and accounted for as part of the member’s contribution to the budget.” 

Knowledge transfer: act of sharing and disseminating knowledge from one organisation to another, or from one field of expertise to another.

Metadata: Metadata is additional data about an informational object and can be "descriptive" or "structural" in nature. A standard is normally employed to define the form of the metadata takes.

OAI-PMH: The Open Archives Initiative Protocol for Metadata Harvesting (OAI-PMH) is a low-barrier mechanism for repository interoperability. It is a protocol developed for harvesting (or collecting) metadata descriptions of records in an archive so that services can be built using metadata from many archives. An implementation of OAI-PMH must support representing metadata in Dublin Core, but may also support additional representations.

OAIS: Reference Model for an Open Archival Information Systems https://public.ccsds.org/pubs/650x0m2.pdf

Resource Creation Community: equivalent to the Data Creation Community in the RM-SSH Enterprise Viewpoint

Data Hosting Community: equivalent to the Data Management Community in the RM-SSH Enterprise Viewpoint

Research Infrastructure (RI): distributed organisation which provides services (e.g. tools, hosting, processing, archiving, displaying data), access to research data and community support for researchers. 

Research Object: Research data part of a scientific investigation. It can be identified (DOI), described (metadata) and aggregated. 

Service: a service can be described as one or multiple objects, systems or activities that an agent makes available to another agent, in order to enable the service using agent to perform a specific activity. 

Service Provider: An organisation or group, whom together, provide a specific service for a designated community.

Service Consumer: an agent that requests, receives and utilises a service. 

Software: programming interfaces used in order to produce code. 
3. In-kind contributions
 3.1 What is an in-kind contribution? 
In-kind contributions are a form of support for not-for-profit organisations, communities, or infrastructures. Such contributions represent the provision of services or activities to an organisation by one of its members, valued in monetary terms according to rules agreed upon beforehand by the members of the organisation, and accounted for as part of the member’s contribution to the budget.
The contribution can be in the form of a direct provision of a tangible asset to the infrastructure or an expenditure incurred directly by the member, which benefits the infrastructure and satisfies its high-level principles or objectives .

In-kind contributions include goods, access to and use of services and facilities, expertise in the form of staff time, provision of or access to equipment. They must be viewed as necessary to carry out tasks of and in the infrastructure and meet the objectives commonly agreed by the members. The value of the contribution should be assessed according to the accounting rules agreed upon by the members in the infrastructure through a governance structure. These rules may rely on the costs incurred by the contributor or on standard cost equivalents defined to ensure fairness among partners (this applies in particular to the accounting of personnel costs). For research infrastructures, in-kind contributions represent a revenue stream. Even though they are not monetary contributions, they may represent a large portion of the research infrastructure's revenue . 

In-kind contributions help to build relationships within an infrastructure as the providers support the mission and activities without the need for large investments of cash and can collaborate to provide contributions jointly. During the construction of the infrastructure contributors become partners in that they may take over the responsibility of construction tasks and equipment, and effective interfacing with other parts of the infrastructure . Fixed-term projects with specific goals and set of partners is an effective method in the solving of start-up difficulties. Ensuring that a provider is informed of what is done with their in-kind contribution encourages them to take on a greater role in development of the infrastructure . 
3.2 In-kind contributions for DARIAH-EU
The new submission and assessment system of contributions, which is currently in development by the project Humanities at Scale, differentiates between contributions and in-kind contributions. 

Contribution	Any relevant research output or activity a DARIAH partner submits as DARIAH-related work.
See The types of contributions and assessment criteria for typology and criteria. 
In-kind contribution (IKC)	A contribution selected by National Coordinator as in-kind for given member country and year. 

All the research outputs created by DARIAH affiliated institutions are considered as contributions: this means that the whole DARIAH research community can benefit from such services (e.g. digitized resources, tools, registries etc.) without them having been recognised as “in-kind contributions”, which represents a further level of selection and assessment. 

This selection is performed by the country’s national coordinators, who decides which contributions will be officially submitted to DARIAH-EU as part of their annual participation to the DARIAH-ERIC. In a second phase, the selected contributions are assessed both for their formal aspects (e.g. responding URL) as well as for the quality of the content, performed by peer reviewers among the working groups and the VCC heads. Both submission and assessment of the contributions are performed in the DARIAH Contributions Tool, whose scope and functioning is explained in detail in the document “DARIAH (in-kind) contributions –  Concept and Procedures”.
3.3 Classes of DARIAH-EU in-kind contributions
Type of contribution	Subtype	Remarks
SERVICE 		
	DATA HOSTING SERVICE 	e.g. data repository service, data deposit service, software repository.
	PROCESSING SERVICE 	E.g. NERD service
	SUPPORT SERVICE	e.g helpdesk, software maintenance
	ACCESS TO RESOURCES	e.g. educational resources, data resource, enriching/creating metadata not normally available ...
ACTIVITY 		
	EVENT	e.g. summer school, webinar, training
	CONSULTING	
	DARIAH COORDINATION	
	CREATING RESOURCES	e.g. educational resources, data resource … controlled vocabularies/thesauri
	DEVELOPMENT OF SOFTWARE	
4. Services
4.1 DARIAH Service Provision
Generally speaking, a service can be described as one or multiple objects, systems or activities that an agent makes available to another agent, in order to enable a user to perform a specific activity. 
In the context of DARIAH a service represents an action that one or more institutions affiliated to DARIAH (the service provider/s) offers to another (DARIAH) institution or single researcher in order to enable the user of the service to reach a certain objective (related to the enrichment, dissemination and sustainability of research outputs).
4.1.1 Enterprise Viewpoint
The DARIAH Service Provision comprises the following community: 
-	Generic Service Provision community: the objective of the Generic Service Provision community is to provide value to an agent through bringing about results that the agent want to achieve, through the provision of a service environment, service delivery, and service product.
DARIAH Service Provision Roles
The following roles are identified in the DARIAH Service Provision community:
-	Service Provision Subsystem (passive role): the community component representing the generic service provision community.
-	Service Owner (active role): has the overall responsibility for the Service Management Subsystem. The Service Owner sets the key objectives and provides overall direction for the Service Management Subsystem through governance protocol, procedure and service agreements made.
-	Service Provider (active role): an agent, usually an institution, which makes a service available for use by the Service Consumer in accordance with a service agreement.
-	Service Consumer (active/passive role): an agent that requests, receives and utilises the service. Access to the service may be direct, or mediated via a third-party, but in accordance with a service agreement.
-	Service Designer (active role): a person who designs, defines, and documents a service based upon the objectives set by the Service Owner.
-	Process Designer (active role): a person who defines, designs and documents a process based upon the objectives of the Process Owner.  
-	Service Manager (active role): The Service Manager coordinates all efforts in the day-to-day running, planning, implementing, monitoring, reviewing and improving the service provision. The Service Manager is the point of contact for issues with the service
-	Service Management Subsystem (passive role): the system and/or policies used to run a service provision.
-	Process Owner (active role): Has overall responsibility for the process, sets the key objectives, and overall direction, goals, & governance for the process.
-	Process Manager (active role): Coordinates all efforts in the day-to-day running, planning, implementing, monitoring, reviewing and improving the process. The Process Manager is the point of contact for issues with the process and manages incidents or changes to the process.
-	Process Implementer (active/passive role): An agent which is involved in the execution one or more activities within a process. The agent carries out defined activities according to the defined process and, as applicable, its exception procedures and reporting incidents to the Process Manager.
DARIAH Service Provision Behaviours
The following behaviours are identified as part of the generic service provision:

-	Service Deployment: the behaviour of the service subsystem performed by the Service Manager, the designer and the service management subsystem, whereby an service is requested, build, instantiated and deployed.
-	Service Provision Management: the behaviour of the service subsystem performed by the Service Manager in taking care of the day-to-day running, planning, implementing, monitoring and reviewing the service provision. 
-	Process Management: behaviour of the process manager, who coordinates all efforts in the day-to-day running, planning, implementing, monitoring, reviewing and improving the process. 
-	Activity Execution: behaviour of the Process Implementer, who is involved in the execution of activities within a process. 
4.1.2 Information Viewpoint
In the Information viewpoint, the information transmitted between the different stakeholders in the context of service providing within the infrastructure is represented. It is specified by Information Objects and their interrelationships. 

The objective of the Information Viewpoint is to provide a common model for generic DARIAH Activities that occur in the infrastructure. It defines a set of Information Viewpoint objects and the set of actions acting upon those objects. The Information Viewpoint specifies the types of Information Objects and their interrelationships.

Platform-specific, or implementation, details are not considered here. The information viewpoint is independent of the Computational Viewpoint interfaces and functions that manipulate the objects, and the technology used to provide the technical infrastructure upon which the objects are stored or transmitted.
Information Object types 
Data:
-	Data Object Type (e.g. Datasets or digitized cultural object): the minimum available information object type that can be shared from an institution with an end user
-	Metadata Object Type: the information object type that describes and contextualizes the data object type
-	Web applications (Service Object Type) (e.g. web interfaces, portal, faceted research): the information object type that translates the data object type (in raw format) into a comprehensible information object for the end user. 
-	Transfer Service Object Type (e.g. API, OAI-PMH, FTP): the information object subsystem that makes it possible for the researcher to access the data
-	AAI response (Object derived from the authentication service)
-	Service Documentation: the documentation component of a service (e.g. procedure, list of documents used for the planning and execution of a service).

Agents: Agents are typically human users or machines acting on behalf of human users.
An Agent refers to the information object type defined in the RM-SSH. There are a number of agents that may be considered part of the generic DARIAH Service Provision.

-	Service Owner: the agent who owns the service and its running
-	Service Provider: the agent who gives instruction to the implementer of a service
-	Service Implementer: the agent that executes a certain action on behalf of the service provider.
-	Service Consumer: an agent that requests, receives and utilises the service.
-	Service Designer (active role): a person who designs, defines, and documents a service based upon the objectives set by the Service Owner.
-	Process Owner (active role): Has overall responsibility for the process, sets the key objectives, and overall direction, goals, & governance for the process.
-	Process Designer (active role): a person who defines, designs and documents a process based upon the objectives of the Process Owner.  
-	Process Manager (active role): Coordinates all efforts in the day-to-day running, planning, implementing, monitoring, reviewing and improving the process. The Process Manager is the point of contact for issues with the process and manages incidents or changes to the process.
-	Process Implementer: the agent that executes a certain action on behalf of the process owner. 
-	Activity Implementer: the agent that executes a certain activity.
-	Service Management Subsystem (passive role): the system and/or policies used to run a service provision.

Service:
Services can be human or automated services and are described by their behaviour or interaction.
-	AAI (authentication subsystem): system to authenticate the user in order to access the resources

Contracts:
-	Service Level Agreement: agreement defining the levels of service and their management between the Service Provider and the Service Consumer.

 
Figure 3: Service Information Object Types and Roles
4.1.3 Computational Viewpoint
A research Infrastructure (RI) such as DARIAH provides services which facilitate scholars to create, interact, process and store, or deposit, data. Other services maybe provided by the DARIAH community. Here we consider a general form of a service. 

The computational viewpoint (CV) describes the functionality of a system. It decomposes the system into objects encapsulating specific functionality that are implemented by a service or activity. Specific interfaces bind the computational objects together, thus allowing the functionality to be distributed. 

This viewpoint is expressed using an object model in which computational object (CV Object) are abstractions, in this instance, of a research infrastructure’s systems & functions, and the interfaces (CV Interfaces) the computational objects can have, are defined. 

Computational objects can relate to other computational objects in the following ways:
-	Interaction: Two objects exchange information as either an operation (request/response), as a (continuous) flow, or as a signal.
-	Instantiation: An object creates a new object via instantiation.
-	Inheritance: An inherited object has the same interface(s) as its parent object and extends it with additional interface(s).

Specific types of computational objects are used here: 

-	Binding object: An object to support more complex interactions between two or more interfaces. These binding objects coordinates this interaction by providing bindings to all required interfaces.
-	Proxy object: An object that provides all external interactions of a subsystem and takes care of managing the internal objects of that subsystem.
-	Controller object: An abstract object to represent the external interaction with custom objects. It is used to represent specific instruments and processing. 

Research infrastructures, including DARIAH, tend to have a service-orientated architecture (SOA) with core functionality encapsulated and accessed via externally facing services and user interfaces which act as brokers.

The CV for a generalised DARIAH service contribution describes set of computational objects that could be expected to constitute a service within the infrastructure. For each of the specific contributing service types a subset of computational objects would normally be expected to be present in the SOA for the functionality of the contribution.

Four groups of computational objects are described below which correspond to architectural layers in a SOA-like structure :

-	Presentation Objects: computational objects that provide access to the service by human users (user interfaces)
-	Service Objects: computational objects that are service intermediaries that broker and orchestrate the use of the component objects (which may be distributed).
-	Component Objects: computational objects that manage and provide access to data
-	Back End Objects: computational objects that manage and maintain the data of the service

Figure 4 below shows the grouping of CV objects for a generalised DARIAH Service Contribution.
 
 
Figure 4: DARIAH Generalized Service Provision CV objects
CV Presentation Objects
CV Presentation objects are the entry points for human users to the services provided.
The user interfaces consist of both service management and researcher (consumer) access points, or gateways.
Service Manager UI
The Service Manager UI provides an user interface to access the Service Subsystem for authenticated human users with management credentials.

 
Figure 5: Computational Viewpoint Service Manager User Interface object
Process Manager UI
The Process Manager UI provides an user interface to access the Process Subsystem for authenticated human users with management credentials.

 
Figure 6: Computational Viewpoint Process Manager User Interface object
Consumer UI
A community portal for interacting with a service, or services, of the distributed infrastructure.

 

Figure 7: Computational Viewpoint Consumer User Interface object

The Consumer UI encapsulates the functions required to interact with the services provided by the research infrastructure externally to the infrastructure. It supports the following interactions:
●	request process (client): takes input from the researcher to request and start a service.
●	authenticate user (client): a client interface which requests confirmation of the identity of the user agent.

This object may take the form of a Virtual Research Environment (VRE), providing a persistent context for a researcher, or group of researchers, service component objects, research data, and interactions between these. Alternatively, it may be an object that facilitates access to a single discreet service.
CV Service Objects
Administration Functions
These objects may be internal or external to the RI and services, provided by an external agent such as a national authority.
User Authentication Service 
The User Authentication Service is a proxy object which confirms the identity of an agent when an agent makes a request to the service (or infrastructure) . As part of the (generalised) service provision it is only composed of an authentication service object.
 
Figure 8: Computational Viewpoint User Authentication Service object
The User Authentication Service is a proxy object for all actions needed to verify the identity of an agent. It supports the following interactions:
●	Authenticate user (server): is a public interface for determining whether the agent is who it claims to be.
●	Request user attributes (server): is a public interface for requesting provided attributes from the agent.

Data Identification Service 
The Data Identification Service provides global identification and location functions for research data resources. It is composed of a persistent identification (PID) service object.
 
Figure 9: Computational Viewpoint Data Identification Service object
The Data Identification Service is a proxy object for all actions needed to register, maintain, and retrieve the location of an identified object. It supports the following interactions:
●	acquire identifier (server). Public interface for registering new identifiers for data resources and updating the current location.
●	resolve identifier (server). Public interface for retrieving the current location of an identified data resource.
Catalogue Service
The Catalogue Service object provides resource discovery functions within the research infrastructure.

 
Figure 10: Computational Viewpoint Catalogue Service object
The Catalogue Service is a proxy object, which encapsulates all all the actions needed to allow research resources (data or otherwise) to be discovered. It supports the following interactions:
●	Update Catalogue (server): is an interface for registering, updating and indexing resources in the catalogue.
●	Query Catalogue (server): is an interface for querying the catalogue for registered/indexed research resources.
●	Query Resource (client): retrieves metadata from data stores or other catalogues and sources
●	Export Metadata (server): provides functionality to gather metadata.
Broker Service
The Broker Service facilitates data access and storage of research data. It facilitates data transfers, query requests, annotation and curatorial services. The broker service validates all requests and verifies the identity and privileges of agents making data requests. 
 
Figure 11: Computational Viewpoint Broker Service object

A broker service is a proxy object, which encapsulates all all the actions required to access data. It supports the following interactions:
●	data request (server): provides functions for requesting the import or export of datasets, the validation of the request and agent making the request.
●	annotate data (client): is used to request annotation of data held within the data curation subsystem.
●	prepare data transfer (client): is used to initiate and negotiate data transfers with the data curation subsystem or the data provision subsystem.
●	query data (client): is used to forward queries onto the data provision object receive the results.
Service Functions
CV service functions offer access to distributed systems and resources (internal and external). This allows building of customer (researcher) services using both internal and external sourced components used in the research and data lifecycles.
Service Subsystem
The Service Subsystem provides service functions and is composed of a service subsystem object, a service workbench object and a service controller object. Each request to deploy a service on behalf of an agent, an instance of the service controller object is instantiated by the service workbench. 

 
Figure 12: Computational Viewpoint Service Subsystem

The Service Subsystem is a proxy object for managing the service, input and resulting data in the service. It supports the following interactions:
●	deploy service (server): the public interface for the deployment of a new service controller.

The Service Workbench is a computational object that instantiates service controller objects. It supports the following interactions:
●	create service controller (server): is the interface for requesting a new service controller.
●	new service controller (instantiation): Instantiation of a new service controller object by the service workbench.

The Service Controller is a controller object that runs the service. It supports the following interactions:
●	configure service (server): the public interface for configuring and managing the service.
●	monitor service (server): is the public interface for monitoring the service.
●	request process (client): is used to deploy a process within the service workflow and controller from the process subsystem.
Process Subsystem
The Process Subsystem provides access to process functions and is composed of a process subsystem object, a process workbench object and a process controller object. For each request to deploy a process from a service controller, an instance of the process controller object is instantiated by the process workbench. A process can request to deploy a process by which a workflow (chain) or processes can be deployed within a service.

 
Figure 13: Computational Viewpoint Process Subsystem 

The Process Subsystem is a proxy object for managing the process, input and resulting data in the service. It supports the following interactions:
●	deploy process (server): the public interface for the deployment of a new process controller.

The Process Workbench is a computational object that instantiates a new process controller objects. It supports the following interactions:
●	create process controller (server): is the interface for requesting a new process controller.
●	new process controller (instantiation): Instantiation of a new process controller object by the process workbench.

The Process Controller is a controller object that runs the process. It supports the following interactions:
●	configure process (server): the public interface for configuring and managing the process.
●	monitor process (server): is the public interface for monitoring the process.
●	request process (client): is used to deploy a process within the service workflow and controller from the process subsystem.
Coordination Service
The coordination service delegates all servicing and processing tasks, coordinates multi-stage workflows and initiates execution and manages data flow within a service.
 
Figure 14: Computational Viewpoint Coordination Service object

The coordination service is a proxy object for processing tasks deployed on infrastructure execution resources. It supports the following interactions:
●	process request (server): which provides functions for scheduling the execution of process tasks. 
●	coordinate process (client): is used to coordinate the execution of data processing tasks on execution resources presented by process controllers. Complex workflows involving many sub-tasks and processes may be orchestrated in this way.
●	prepare data transfer (client): This is used if data is required for or generated in a service and is moved into and out of the data store via the data transfer service.
CV Component Objects
Data Curation Service 
The Data Curation Service allows data curation by monitoring data and performing transfer, processing and provisioning of the data. The subsystem is composed of a Data Curation Service object.
 
Figure 15: Computational Viewpoint Data Curation Service, Provenance Data Service and User Metadata Service
The Data Curation Service provides only one computational function, which is the monitoring of data. When needed, it consumes other subsystems to perform the actual curation. It provides the following interfaces:
●	monitor data (server): this is a public interface that allows data to be monitored.
●	transfer data (client): this is an interface for transferring data from e.g. data provisioning to data processing.
●	process data (client): the interface for processing the monitored data. This may include the calculation of checksums, or the transformation to new data formats.
●	create data (client): the interface for the creation of new data. This may include the creation of new metadata.
Provenance Data Subsystem
The provenance data subsystem is a specialised form of the data curation service which deals with the capture and maintenance of provenance data about the creation, processing, and dissemination of data within a service. See Figure 15.

User Metadata Subsystem
The user metadata subsystem is a specialised form of the data curation service which deals with the capture and maintenance of user metadata within a service, for example user and groups privileges within a VRE instance of a VRE service. See Figure 15.
Data Provision Subsystem 
The Data Provision Subsystem provides data sharing, data discovery and data access functions and is composed of a data provision service object, a data inventory service and a data storage controller.
 
Figure 16: Computational Viewpoint Data Provision Subsystem

The Data Provision Service is a proxy service for the Data Provision Subsystem. It supports the following interactions:
●	share data (server): is a public interface for allow data to be shared.
●	discover data (server): is a public interface for searching provided data.
●	access data (server): is a public interface for accessing provided data.

The Data Storage Controller is a controller object that persists the published data. It supports the following interactions:
●	post data (server): is an interface for persisting data to the data storage controller.
●	retrieve data (server): is an interface for getting data from the storage controller.

The Data Inventory is a computational object that allows data to be discovered. It supports the following interactions:
●	index data (server): is an interface for registering/indexing data in the inventory .
●	query inventory (server) is an interface for querying the inventory for registered/indexed data.
Data Creation Subsystem 
The Data Creation Subsystem creates data by recording observations. The subsystem is composed of a data creation service object, a creation instrument workbench object and an creation instrument controller object.

 
Figure 17: Computational Viewpoint Data Creation Subsystem
The Data Creation Service is a proxy object for managing the instruments and the resulting data. It supports the following interactions:
●	deploy instrument (server): is a public interface for the deployment of a new tool.
●	configure tool (server): is a public interface for controlling the tool.
●	provide data (server): is a public interface for retrieving the created data from the tool.

The Creation Instrument Workbench is a computational object that instantiates creation tool controller objects. It supports the following interactions:
●	create tool controller (server): is an interface for requesting a new instrument controller.
●	new creation tool controller (instantiation): an instantiation of a new tool controller object by the creation instrument workbench.

The Creation Tool Controller is a controller object that records observations. It supports the following interactions:
●	configure tool (server): is an interface for configuration of the tool controller.
●	get data (server): is an interface for requesting the data created by the controller.

Data Processing Subsystem 
The Data Processing Subsystem provides data processing functions and is composed of a data processing service object, a data process workbench object and an data process controller object.
 
Figure 18: Computational Viewpoint Data Processing Subsystem
The Data Processing Service is a proxy object for managing the processing controllers and the data that is (to be) processed. It supports the following interactions:
●	deploy process (server): is a public interface for requesting a new process.
●	get data (client): is a public interface for retrieving the processed data.
●	post data (client): is a public interface for providing data to the process.

The Data Process Workbench is a computational object that instantiates data process controller objects. It supports the following interactions:
●	create data process controller (server): is an interface for requesting a process controller object.
●	new data process controller (instantiation): is the instantiation of the new data process controller object.

The Data Process Controller is a controller object that processes data. It supports the following interactions:
●	configure process (server): the interface for configuring the process.
●	get data (server): is the interface for retrieving processed data from the data process controller object.
●	post data (server): is the interface for providing data to the data process controller object.

Data Transfer Subsystem 
The Data Transfer Subsystem provides transfer services within the service and RI. The subsystem is composed of a Data Transfer Service and an Abstract Data Transfer Object, which may be instantiated as e.g. a Data Importer Object or a Data Exporter Object.


 
Figure 19: Computational Viewpoint Data Transfer Subsystem
The Data Transfer Service is a proxy object for providing data transfers. It supports the following interface:
●	deploy transfer (server): is a public interface for requesting a data transfer.
●	
The Abstract Data Transfer Object is an abstract object that provides the following interfaces.
●	fetch data (client): is a client interface for retrieving data from a source.
●	post data (client): is a client interface for providing the data to a target.

The example Data Importer implements the Data Transfer Object for specific environments. In this case, the data importer may specify how the data is fetched from a remote source, whether specific processing needs to take place (via a Data Processing Subsystem) and how the outcome should be provided to the target system.
CV Back End Objects
Back End Objects are objects which encompass the systems and resources provided for preserving, publishing, and processing research data through user accessible services.
Storage System
The Storage System is a system that manages and stores data and metadata of the research infrastructure.
 
Figure 20: Computational Viewpoint Storage Systems
The File Management System manages the storage and retrieval of data as files in a computer system.
The Database Management System manages the storage and retrieval of data and metadata in logically structured repository systems.
Service Registry
The service registry is an information system for registering services within the research infrastructure.

	 
Figure 21: Computational Viewpoint Service Registry object
The Service Registry is a proxy object that encapsulates all actions needed to register, update and request service information. It supports the following interactions:
	register/update service (server): is a public interface for registering a service and any maintenance events. 
	request service attributes (server): is a public interface for requesting provided attributes for a registered service.
4.2 Data Hosting Service
DEFINITION:
A service provider manages, oversees, and has responsibility for infrastructure, software and administrative tasks and makes this system available as a hosted service to users, usually, but not necessarily, over the Internet. A hosted service provider may consist of one organisation, or a collaboration between more organisations and/or sub-contracted specialist service providers. The hosted service may be provided on a dedicated or shared-service model . 

Hosting services are most often used for hosting Websites, but can also be used for hosting research data objects such as: audio-video qualitative data, quantitative data, software (and software configuration), digital documents, or information about research object and similar content. In the context of DARIAH IKC all research data object types are considered as research data, and hence services that concentrate on a specific object type as a specialisation of a hosting service. 

A hosting service generally comprises of a repository, a depositing (acquisition) service, a discovery service, and (optionally) a provision service that gives access to the deposited data resources - even if the provision service per se is more connected with the contribution type “Access to resources”. 

4.2.1 Enterprise Viewpoint
COMMUNITIES
The Hosting Service IKC comprises the following communities: 

Data Hosting Community: The Data Hosting Community is that who acquires, administers and curate those data created or collected by the Resource Creation Community. Within DARIAH, this community is represented by an institution which has the technical capacity of hosting research data on its servers, for a defined period of time. 

Data Hosting Roles
-	Data Hosting Subsystem (passive role): the community component representing the data hosting community as a whole. 
-	Data Owner (active role): a person or organisation that owns the data and determines the conditions for deposit/access with the Data Manager. 
-	Data Manager (active role): a person that is responsible for ensuring the quality of the research data during its ingest and management. 
-	Preservation Manager (active role): a person that is responsible for generating data products, and entering/registering them in the data administration service. 
-	Data Administration System (passive role): A system that is responsible for registering the data products for management purposes. 

Data Hosting Behaviour 
The following behaviours are identified in the Data Hosting Community: 

-	Acquire Data: the behaviour performed by the data manager, the data owner and the data administration system whereby they negotiate a submission agreement, transfer a submission information package to the data administration system and appraise it. 
-	Curate Data: the behaviour performed by the data manager, the preservation manager, and the data administration system, whereby the data manager check the quality of the data and removes faults. The data manager then adds meaningful documentation  (metadata) to the data. The preservation manager transforms the data to a preservation format or migrates it to another platform, creates an Archival Information Package and stores it in a data administration system. 
-	Administer Data: the behaviour performed by the data manager and the data administration System whereby the required information for data management is administered. 

Communities that typically collaborate with the data hosting community related are: resource creation community, data provisioning community for retrieving (well-documented) data and for making the data accessible, and the data processing community for e.g. transforming data.
4.2.2 Information Viewpoint
Differently from the Enterprise viewpoint (where the community was central), for this type of in-kind contribution the information type represents the core of the investigation. The information type needs to be considered in itself, with no reference from the community that created or is responsible for it. 

Information Object Types:
Data
For this type of contribution, the “data” are represented by the humanities research outputs that need to be hosted.  These data can be organised in structured/ unstructured data; digitized cultural objects and its related (descriptive) metadata; digital and enhanced publications

Agents
The administrative roles that describe who can perform an action in the hosting system and what kind of role he/she can perform (e.g. administrator, editor, user). Three are the main agents identified at the information viewpoint level for the Hosting Services: The Data Owner, who owns and is responsible for the quality of the hosted data; the Service owner is responsible for the hosting service provided; the Service Interface represents the interface between the service owner/ provider and the data owner. 

Service 
The process of hosting data for an agent by a service provider. 

Contract
It usually describes the relation between two or more agents. In the case of hosting of humanities data, the contract can establish the following responsibilities: for how long will the data be maintained? how will they be preserved? will they be enriched? how will they be accessed? what are the responsibilities of the agents? In terms of contracts, a Hosting Agreement can be identified between the Data Owner and the Service Owner. 
4.2.3 Case Study - EASY Data Archive 
Easy is the data archive for the social science and humanities in the Netherlands. Such data archive has been developed and is currently maintained and enriched by DANS, an institute of the Dutch Royal Academy of Science, that has a leading role (nationally and internationally) in the development of data quality policies and research data management plans. 

As such, EASY offers to the research community the possibility to host their data after they have finished their research and therefore can be considered as a candidate for a DARIAH contribution Data Hosting Service. 

In terms of Enterprise Viewpoint, the Data Hosting community is represented by the DANS team, which is the community who acquires, administers and curates the dataset created by the Resources Creation Community (the researcher depositing the datasets). The team at DANS acquires the data (with the support of a submission agreement) through the submission of information packages. 

To all the archived data, DANS applies the principles of the Preservation Policies Data Archiving and Networked Services, which draws the lines of the agreement between the Data Hosting Community and the Resource Creation Community. 

In terms of information Viewpoint, the research outputs and the data delivered to EASY in order to be archived are the main information object type for this type of contribution. According to the recommendation of DANS, the data need to be structured according a series of preferred data and metadata formats and they need to include reference to their accessibility and reuse possibility. A contract (another data object type) will then establish duties and rights for the Data Hosting Community and the Data Resource Community by answering questions like: for how long will the data be maintained? what are the responsibilities of the stakeholders involved?

4.3 Processing Services
DEFINITION: A partner offers a (digital) service that applies some algorithmic processing (statistical analysis, annotation) on given data, or provides means to edit/curate data (e.g. web interface for collaborative editing).
Processing service is distinct from content hosting service in that it does not store data, but generates new data based on given input. Ideally, processing services are connected seamlessly with hosting service to appear to a user as one (virtual research) environment.
4.3.1 Enterprise Viewpoint
Communities
-	Data Creation Community: The Data Creation Community is represented by whom creates or collects data. These data can be the results of digitization of cultural heritage objects or research outputs from scientific investigation. 
Within DARIAH-EU, this community can be represented by a single or a group of researchers, as well as by a single or a group of institutions. 

-	Data processing Community: this community allows the transformation (editing, curation, visualization) or the enrichment of the data created by the Data Creation Community by creating and applying an algorithmic process.

Roles

Roles within the Data Creation Community:
-	Data Creator: the agent or agents responsible for the creation of the data
-	Instrument Designer: the agent who is responsible to design, build and maintain the instrument that is used for data collection
-	Instrument: a system that is used by the data collector to collect the data 
-	Data Collector: The agent that is responsible to collect the data created by the Data Creator

Roles within the Data Processing Community: 
-	Processor Designer: an agent who builds, maintains and configures an algorithmic processor.
-	Processor: piece of software used by the Process consumer that transforms the data.
-	Process Consumer: an agent that is responsible for applying the algorithmic process to the data created by the Data Creation Community.

Behaviours: the following behaviour is identified in the Data Processing Community: 

Process Data
the behaviour performed by the processor (software) which processes the original data created by the data Creation Community; the behaviour performed by the Process Consumer (agent), when applies the algorithmic process to the data created by the data Creation Community. 
4.3.2 Information Viewpoint
Data
For the in-kind contribution ‘Processing Services “ data are represented by the algorithm that is necessary to process the input data (Code) and the data themselves, that are the object of the the transformation. Finally, the processed data are also a data type in the information viewpoint and represent the data that are object of the transformation, at the end of the processing. 

Agents
Three are the main agents identified at the information viewpoint level for the Processing Services: the Data Owner, who owns and is responsible for the quality and outcome of the data after their processing. The service owner is responsible for the processing service provided as well as the application of the processing algorithm. The service interface represents the interface between the service owner/ provider and the data owner. 

Service
The algorithmic processing lies at the heart of this in-kind contribution, as it represents the core activity and service that service owner can provide to a data owner.

Contract
In terms of contracts, a Processing Agreement can be identified between the Data Owner and the Service Owner. 
4.3.3 Case Study: TextGrid 
TextGrid is a virtual research environment for researchers in the text-based humanities and cultural studies. Since 2006, TextGrid has been funded by the German Federal Ministry of Education and Research and, today, forms an integral part of DARIAH-DE. TextGrid has a large and growing community of users that roughly fall into the categories of individual researchers and research projects of varying sizes.
Among other features, it supports the creation of digital editions using free, project-specific and expandable tools and services. Tools, data and methods can be used independently, regardless of operating system, software equipment and location.
 
TextGrid consists of the TextGrid Laboratory (TGLab), a desktop application for all major operating systems, and the TextGrid Repository (TGRep). TGLab is the central Service Interface which is used as the Instrument by which a Data Owner ingests her research data provided by the Data Creator into the TextGrid storage, which is managed by DARIAH-DE infrastructure partners as the Data Collectors. The data can be used further in TGLab’s tools, the Processors, operated, maintained and supported by DARIAH-DE development partners as Service Owners. Within TGLab the user can use tools such as the Text-Image-Link Editor, a Processor, to enrich images with text annotation and link the image with (parts of) its plain text transcription. This Processed Data can, ultimately, be published to the Hosting Service TGRep.

4.4 Support Services
DEFINITION:
Support services are designed to help for the use of a tool or a service. They also contribute to the update and maintenance for a service an institution provides. 
This type of contribution includes helpdesks (services charged to answer requests from the users). It can be an automated helpdesk (email address).
On a second level, support services can be the components helping to maintain the configuration for a software. It can be human support, on the base of a service level agreement, or a helpdesk providing the information for the maintenance of a service.

4.4.1 Enterprise Viewpoint
Community
-	Support Provision Community: Community providing and maintaining the support services.
-	Support Receiving Community: Community requesting the support services.

Roles
-	Support provider: the agent who legally provides the support activity (e.g. institution)
-	Support implementer: the agent/or system who performs the support service
-	Support receiver: subject of the consultancy: the agent who instantiates the request for support and receives the outcome of it.
-	Support Provision System (passive): the system and/or policies used to run a support service.

Behaviours
-	Support management: the behaviour of the Support provider,  who overviews the running of the support services, and ensures the maintenance of the service.
-	Support execution: the behaviour of the support implementer, who maintains the service.
4.4.2 Information Viewpoint
Data Object Types:
Data
-	Support Documentation: the documentation component of the support service (Helpdesk)

Agents
-	Support provider: the agent who legally provides the support activity (e.g. institution)
-	Support implementer: the agent/or system who performs the support service
-	Support receiver: the agent who instantiates the request for support and receives the outcome of it.

Service
-	AAI (authentication subsystem): system to authenticate the user in order to access the support service.

Contracts
-	Support Service Contract: Service Level Agreement between the Support provider and the Support implementer, that provides a support activity


4.5 Access to Resources
DEFINITION:
(Online) access to resources (datasets). This can be raw data, (web) applications offering rich access to data, or web services that allow a programmatic access to the data (API). 
This type of contribution does not include (national or domain-specific) aggregators, or metadata catalogues, i.e. services that collect information about resources from multiple providers and allow to browse and search in it. These will/can ideally become a source of information about contributions.
It also does not include web services processing data (see Processing services contribution).
4.5.1 Enterprise Viewpoint
Community
Data Provision Community: who provides discovery of, and access to data. Within DARIAH this community can both be represented by a community of researchers/research institutions (that through means of communications, disseminates information about the deposited data, or provides interfaces for the discoverability of the deposited data) or by the same community that provides the storage for the research data. 

Roles
-	Data Provision Subsystem (passive role): the community component representing the data provision community. 
-	Data Owner: who owns the data
-	Data Provider (active role): a person or organization that is responsible for making the research data from the data owner available for the data consumer. 
-	Data Discovery System (passive role): a system facilitating discovery of research data and its context.
-	Documentalist (active role): a person who documents data with metadata according to widely accepted standards of Data Management community.
-	Data Retrieval System (passive role): a system that enables retrieval of research data. Data retrieval includes access control (and thus, authorization).
-	Data Consumer (passive/active role): an agent that requests and receives the research data (for further use). Access to the data may be direct, or mediated via a third-party.

Behaviours
-	Data Publication: A behaviour of the data provider, the Data Discovery System and the Data Retrieval System for making research data discoverable and accessible.
-	Data Discovery: A behaviour of the data consumer and the Data Retrieval System whereby the data consumer uses the Data Retrieval System to discover data of interest.
-	Data Retrieval: A behaviour by the Data Consumer and the Data Retrieval System whereby the Data Consumer request data or metadata and the Data Retrieval System responds, after successful authorization, with the requested metadata and/or data. The metadata may be used for referral.

Communities that typically collaborate with the data provision community related are: data management community for improving metadata for discovery, data processing community for harmonisation or just-in-time conversion during access, data identification community for global identification or referral, user authentication community for global authentication of data consumers and data creation community for capturing enrichments to the provisioned data.
4.5.2 Information Viewpoint
Data
-	Data Object Type (e.g. Datasets or digitized cultural object): the minimum available information object type that can be shared from an institution with an end user
-	Metadata Object Type: the information object type that describes and contextualizes the data object type
-	Web applications (Service Object Type) (e.g. web interfaces, portal, faceted research): the information object type that translates the data object type (in raw format) into a comprehensible information object for the end user. 
-	Transfer Service Object Type (e.g. API, OAI-PMH, FTP): the information object subsystem that makes it possible for the researcher to access the data
-	AAI response (Object derived from the authentication service)

Agents
-	Data Owner: the agent who owns the data that are made accessible 
-	Data Consumer: the agent who access the data 
-	Data Manager: the agent who makes sure that the quality of the data is met and that the user experience is satisfactory

Services
-	User guide/ manual: information on how to access the resources
-	AAI (authentication subsystem): system to authenticate the user in order to access the resources

Contracts
-	Contract: e.g. reuse licenses and intellectual property rights clearance
-	Agreement: An agreement (e.g. a standard) defines the choice by a community to use a certain standard in order to harmonize the access to the data and metadata.

4.5.3 Case Study: the CENDARI AtOM
The CENDARI project ran from January 2012 to January 2016 funded under the FP7 grant scheme.  CENDARI created a data space whose data have been created in two different ways. On the one hand memory institutions and aggregators delivered their data to the CENDARI federated data space. On the other hand, CENDARI made available hundreds of the so-called “hidden collections” from European archives: these collections were not aggregated by third institutions, nor were they digitised - in fact they often belong to small archives whose digitisation resources are often lacking. Rather, the CENDARI researchers manually encoded in a structured format the metadata describing those collections, by making these collections discoverable and reusable for the first time. 

From an enterprise viewpoint, the data provision community  in this case the CENDARI researchers -  played a crucial role in this contribution, by providing a first and unique access to resources that otherwise would have never been accessible. The data provision community related directly with the data owner, which in this case is represented by the Archive, who owns and archives the original documents and artefacts. 
The data discovery system - the tool AtOM in our case, facilitates the discovery of the research data and their context; AtOM also acts as the Data Retrieval system, which is a passive role as its actions are not tangible directly, but nonetheless allow actions like user-control and thus authorisation. 

From an information viewpoint, the user interface represents the information object “web applications”, as it translated the data object type into a comprehensible information object for the end user. 
In the case of AtOM, then, the Data object type, can be described in tight connection with the metadata object type, as in our case the object is purely made of metadata, without any object attached to it. 
In terms of service…
5. Activities
5.1 DARIAH Activity Provision
In general terms, an activity can be described as one or a set of actions, performed by an agent (single or institution) in order to achieve a result or product that can be shared and valued by another agent. 

In the context of DARIAH, an activity is interpreted as a collection of people, work items, communications and processes to achieve a specific goal , whose outputs can be made accessible and valued by the DARIAH community (e.g. single researchers as well as research institutions or cultural heritage institutions). 
Differently to the services, an activity is discrete, as it is marked by an agreed beginning and an end. An activity can be part of a service or of a process. 

The examples listed below provide an overview of different activities performed in the DARIAH-ERIC, by displaying different types of data, different communities involved in the creation as well as in the usage/ consumption of the outputs of such activities. 
5.1.1 Enterprise Viewpoint
Who are the communities involved in the performing of DARIAH activities?

-	Data Creation Community: The Data Creation Community is involved in the DARIAH activities at different levels and different in-kinds contributions, especially in the “Development of Software” and “Creating resources in-kinds”. This community creates the research data, which in the DARIAH case are represented by digitized cultural objects, as well as training resources. 
-	Data Management Community: also in this case, this community is involved in different DARIAH activities, especially in the DARIAH “Consulting” in-kinds. The Data management community has two main aims: on the one hand, it makes sure that the data quality is as high as possible. It also administers and curates the research data. 
-	Data Provision Community: It’s involved in the DARIAH activities, especially at the level Consulting and Coordination. The ultimate goal of the DARIAH Coordination is that of making the data and services in DARIAH recognized among the research community. Similarly, as part of the Consulting Activity, the main aim might be that of making the DARIAH resources and activities well known and accessible. 

Roles 
The following roles are identified in the Activity community

-	Activity Creation Subsystem (passive) the community component representing the activity creation community
-	Activities Owner: (single or institution) the agent who owns and is ultimately responsibility of the owned activity 
-	Activity Provider (different from the activity implementer): the agent (individual or institution) that performs a certain action in the context of DARIAH
-	Activity Implementer: the agent that executes a certain action on behalf of the activity provider.
-	Activity Consumer: the agent (individual/ institution) that receives, consumes or experiences the outputs created during an activity. 
-	Activity Manager: has a day to day overview of the running of the activity. This role is also the point of contact for issues with the expected running of the activity
-	Activity Management System (passive): the community component representing the activity management community (e.g. management tools and object buro)
-	Activity Support: agent who provides support for the planning and running of an activity. This can be represented by a service (link to service here). 

Behaviours
The following behaviours are encountered:

-	Activity management: the behaviour by the activity manager, who overviews the running of the activities on a daily basis. 
-	Activity support: the behaviour of the activity support agent, offering support for the planning and running of an activity. 
-	Activity execution: the behaviour of a number of agents (activity provider, activity implementer) performing certain actions in the context of an activity. 

5.1.2 Information Viewpoint
The objective of the Information Viewpoint is to provide a common model for generic DARIAH Activities that occur in the infrastructure. It defines a set of IV objects and the set of actions acting upon those objects. The IV specifies the types of Information Objects and their interrelationships.

Platform-specific, or implementation, details are not considered here. The information viewpoint is independent of the Computational Viewpoint interfaces and functions that manipulate the objects, and the technology used to provide the technical infrastructure upon which the objects are stored or transmitted.


Information Object types 
Data
-	Activity Documentation: the documentation component of an activity (e.g. procedure, list of documents used for the planning and execution of an activity). 

Agent
An Agent refers to the information object type defined in the RM-SSH . There are a number of agents that may be considered part of the generic DARIAH Activity Provision. 
-	Activity Owner: the agent who owns the activity and its running
-	Activity Provider: the agent who gives instruction to the implementer of an activity
-	Activity Implementer: the agent that executes a certain action on behalf of the activity provider. 
-	Activity Consumer: the agent (individual/ institution) that receives, consumes or experiences the outputs created during an activity. 
-	Activity Manager: has a day to day overview of the running of the activity. This role is also the point of contact for issues with the expected running of the activity
-	Activity Management System: the community component representing the activity management community (e.g. management tools and project officer)

Service
-	Support Service: series of services that make an event possible (e.g. catering, AV recording)

Contract
-	Activity Agreement: between the activity provider and the activity owner, and the activity consumer. 
-	Support Service Contract: between the activity provider and service provider, that provides a support activity (e.g. catering, venue)

 
Figure 22: Information Viewpoint - Activity Objects and Roles
5.1.3 Computational Viewpoint
The CV for a generalised DARIAH activity contribution describes set of computational objects that could be expected to constitute an activity within the infrastructure. For each of the specific contributing activity types a subset of computational objects would normally be expected to be present in the SOA for the functionality of the contribution.

As per the CV for a generalised service, there are four groups of computational objects as can be seen in figure 7 below.

 
Figure 23: Computational Viewpoint DARIAH General Activity
CV Presentation Objects
Presentation objects are the entry points for human users to the services provided.
The user interfaces consist of both service management and researcher (consumer) access points, or gateways.
Activity Management UI
The Activity Management User Interface provides an user interface to access the Activity Subsystem for authenticated human users with management credentials.

 
Figure 24: Computational Viewpoint Activity Management User Interface object
Support Service UI
The Support Service User Interface provides a user interface to access the Support Services Service for authenticated human users with management credentials.

 
Figure 25: Computational Viewpoint Support Service User Interface
Consumer UI
A community portal for interacting with an activity, or activities, of the distributed infrastructure.
 

The Consumer UI encapsulates the functions required to interact with the activities provided by the research infrastructure externally to the infrastructure. It supports the following interactions:
●	request process (client): takes input from the researcher to request and start a service.
●	authenticate user (client): a client interface which requests confirmation of the identity of the user agent.
CV Service Objects
Administration Functions
These objects may be internal or external to the RI and activities, provided by an external agent such as a national authority.
User Authentication Service 
The User Authentication Service is a proxy object which confirms the identity of an agent when an agent makes a request to the service (or infrastructure) . As part of the (generalised) service provision it is only composed of an authentication service object.
 
Figure 5: Computational Viewpoint User Authentication service object

The User Authentication Service is a proxy object for all actions needed to verify the identity of an agent. It supports the following interactions:
●	Authenticate user (server): is a public interface for determining whether the agent is who it claims to be.
●	Request user attributes (server): is a public interface for requesting provided attributes from the agent.
Activity Subsystem
The Activity Subsystem provides access to activity functions and is composed of an activity service object, an activity workbench object and a activity controller object. For each request to deploy an activity from a service controller, an instance of the activity controller object is instantiated by the activity workbench. 


 
Figure 26: Computational Viewpoint Activity Subsystem

The Activity Service is a proxy object for activity subsystem, managing the activity. It supports the following interactions:
●	deploy activity (server): the public interface for the deployment of a new activity controller.

The Activity Workbench is a computational object that instantiates a new activity controller objects. It supports the following interactions:
●	create activity controller (server): is the interface for requesting a new activity controller.
●	new activity controller (instantiation): Instantiation of a new activity controller object by the activity workbench.

The Activity Controller is a controller object that runs the activity. It supports the following interactions:
●	configure activity (server): the public interface for configuring and managing the activity.
●	monitor activity (server): is the public interface for monitoring the activity.
●	get data (client): is the interface to get data for use in the activity.
●	post data (client): is the interface to receive data created in the activity.
Coordination Service
The coordination service delegates all activity tasks. It coordinates multi-stage workflows and initiates execution and manages any data flow within an activity.
 
Figure 27: Computational Viewpoint Coordination Service object

The coordination service is a proxy object for activity tasks deployed on infrastructure execution resources. It supports the following interactions:
●	process request (server): which provides functions for scheduling the execution of activity tasks. 
●	coordinate process (client): is used to coordinate the execution of activity tasks on execution resources presented by activity controllers. Activity workflows may be orchestrated in this way.
●	prepare data transfer (client): This is used if data is required for or generated in a service and is moved into and out of the data store via the data transfer service.
Support Services Service
The support services service provides access to services provided externally to the research infrastructure and activity. For example, catering services for an event, or software publishing services (e.g. GitHub).

 
Figure 28: Computational Viewpoint Support Services Service object

The support service is a proxy object for support services service for external services. It supports the following interactions:
●	request support service (server): is the interface for initiating a support service for an activity.
●	query support (server): is the interface which provides status information about the support service.
●	get data (client): is the interface to get data for use in the support service.
●	post data (client): is the interface to receive data created in the support service.
CV Component Objects
Storage Controller
Data storage needs for an activity are significantly less complex than potentially for a service, for example, a data hosting and preservation service, thus an activity requires storage controller objects to interface with storage system used by the activity.
 
Figure 29: Computational Viewpoint Storage Controller object
The Storage Controller is a controller object that manages the storage used in an activity. It supports the following interactions:
●	get data (client): is the interface to get data from the storage system.
●	post data (client): is the interface to post data to the storage system.

CV Back End Objects
Back End Objects are objects which encompass the systems and resources provided for preserving, publishing, and processing research data through user accessible services.
Storage System
The Storage System is a system that manages and stores data and metadata of the activity in a research infrastructure.
 
Figure 30: Computational Viewpoint Storage Systems

The File Management System manages the storage and retrieval of data as files in a computer system.
The Database Management System manages the storage and retrieval of data and metadata in logically structured repository systems.
Activity Registry
The activity registry is an information system for registering activities within the research infrastructure.

 
Figure 31: Computational Viewpoint Activity Registry
		
The Activity Registry is a proxy object that encapsulates all actions needed to register, update and request activity information. It supports the following interactions:
	register/update activity (server): is a public interface for registering an activity and any maintenance events. 
	request activity attributes (server): is a public interface for requesting provided attributes for a registered activity.
5.2 Events
DEFINITION:
This type of in-kind contribution describes events organised in the field of digital arts and humanities and cultural heritage, whose aim is to:
-	offer a theoretical insight of the methods, practices, history and future developments in the field of digital arts and humanities
-	showcase case studies in the field of digital arts and humanities
-	offer training and guidance in the application of digital methodologies in traditional humanities curricula

Examples for this type of contribution are:
-	lecture
-	Symposium
-	Conferences
-	workshop
-	training day/s
-	summer/ spring/ winter school
-	academic course
-	academic program
-	MOOCs and other forms of online education

5.2.1 Enterprise Viewpoint
Communities

The “Event” in-kind contribution comprises the following communities: 

Outreach, Training & Support Community: who provides community services to the SSH research community. They interact with the data infrastructure community for developing standards or for providing training for or about the data infrastructure community. This community is not directly involved in the data creation process, but it rather disseminates and gives training on the data developed and processed. 


Roles
-	Event owner: the agent who initiates and is responsible for the event; it can be an individual or the organization
-	Event host: institution hosting the event 
-	Event manager: the agent who supervises the organization of the event  on a daily basis in view of its successful outcome 
-	Event deliverer: the agent who delivers the event, (e.g. a conference or an academic course)
-	Event participant: the agent who attends the event or training
-	Event Support: the agent who provides support with organizational aspects of the event or training
-	Event documentation System (Passive): written material that accompanies the event or the training material provided in support of a training
-	Event Registration System (Passive): the system that allows the registration of the participants to the event 
-	Event Assessor: the agent who i.e. assesses the papers, abstract for the conference // or assesses the test at the end of the training; in training, i.e. the assessor assesses the quality of the outcomes and maybe gives a certificate
-	Event Assessment System (Passive): the community component representing the event assessment community 


EXAMPLE BEHAVIOURS IN THE PREPARATION OF A DH EVENT

1.	Paper submission: the behaviour of the event deliverer, who submits a proposal to be presented at the DH event. 
2.	Registration attendees: the behaviour of the event participants, who register for the event via the event registration system in order to attend the event itself
3.	Running the event: the behaviour of the Event Manager, who makes sure that the event runs smoothly and according to the programme
4.	(Post Event activities): the behaviour of a number of stakeholders (event manager, event host and event owner) that reflect on the organised event, focussing in particular on the successes and failures. 



Example of Event from the Enterprise viewpoint perspective

An event is a system instantiated by an Event Owner. The last DH2016 conference was held in Krakow and organized jointly by a Programme Committee (international) and a local organization team. The local organization team also acts as the Event Manager, supervising the successful outcome of the event. 
The event documentation system includes written material that accompanies the event (brochure, maps, abstracts). One important aspect of such big event as the DH2016 is represented by the event registration system. The event assessment system is also very important and comprises one or more Event Assessors, who are responsible for assessing and accepting the proposals submitted. 
The Event Participants are the conference attendees, while the Event Deliverer are the people presenting at the conference. 

5.2.2 Information Viewpoint
This paragraph provides an overview of the category type: “event” from an Information Viewpoint. 

Data 
Information that is used as support or training material during an event (including training event).  The data can consist of research outputs, both in the form of raw data or publications, standardized in order to describe consistently the observation and analysis. 
Data information objects can be content objects (observation, concepts and metadata) or container objects (dataset, inventory). 

Agents 
-	Event owner: the agent who initiates and is responsible for the event; it can be an individual or the organization
-	Event host: institution hosting the event 
-	Event manager: the agent who supervises the organization of the event  on a daily basis in view of its successful outcome 
-	Event deliverer: the agent who delivers the event, (e.g. a conference or an academic course)
-	Event participant: the agent who attends the event or training
-	Event Support: the agent who provides support with organizational aspects of the event or training
-	Event documentation System (Passive): written material that accompanies the event or the training material provided in support of a training
-	Event Registration System (Passive): the system that allows the registration of the participants to the event 
-	Event Assessor: the agent who i.e. assesses the papers, abstract for the conference // or assesses the test at the end of the training; in training, i.e. the assessor assesses the quality of the outcomes and maybe gives a certificate
-	Event Assessment System (Passive): the community component representing the event assessment community 

Service
-	Information material about the event: advertising, but also training material distributed to support the behaviour of the event deliverer
-	Event support: support during the organization of the event

Contract
-	Standards: standards that exist between a community (e.g. a certain standard use in a exercise during the training) 
-	Access conditions: access conditions that regulate the participation to the event
-	Attendance Certificate: the certificate that proves the participation of an attendee to the event
5.3 Development of Software
DEFINITION: Availability of software, i.e. executable code that can be installed and run by other partners. The contribution should include the source code (not just the binaries).
ScopeNote: We distinguish between software and service as separate contributions. Every (digital) service is an activation of some software. If both a service and the underlying software are provided, then it counts as two distinct (though related) contributions.
The code can be in any programming language, it can also be only a simple script dedicated to one specific task, as long as it is working and documented.

5.3.1 Enterprise Viewpoint
Communities

-	Data Creation Community: the community that creates the code necessary to install and run a software
-	Data Provision Community: The Community who provides discovery and access to the software developed by the Data Creation Community. 

Roles 
-	Software owner: the agent who owns the software and it is ultimately “responsible” for its functioning 
-	Software developer: the agent who develops the source-code of the software
-	Software manager: the agent who is responsible of the release and good functioning of the software
-	Software architect: the agent who is responsible of the overall architecture of the software, from its design to the completion of the software
-	Software Tester: the agent who is responsible for the testing of the software during the production phase and before its release
-	Documentation/ training subsystem (passive): the documentation that will facilitate the comprehension of the software by the end users once it is released
-	Software publisher: the agent who publishes and makes available the software
-	Software development subsystem (passive): the underlying system supporting the software developer
-	Software publishing subsystem (passive): the system supporting the publication and release of the software, initiated by the software publisher
5.3.2 Information Viewpoint
Data
-	Code
-	Software: programming interfaces used in order to produce code 
-	Documentation/ training subsystem (passive): the documentation that will facilitate the comprehension of the software by the end users once it is released

Agents
-	Software owner: the agent who owns the software and it is ultimately “responsible” for its functioning 
-	Software developer: the agent who develops the source-code of the software
-	Software manager: the agent who is responsible of the release and good functioning of the software
-	Software architect: the agent who is responsible of the overall architecture of the software, from its design to the completion of the software
-	Software Tester: the agent who is responsible for the testing of the software during the production phase and before its release
-	Data Owner: the agent who owns the code and it is ultimately “responsible” for its correct functioning 
-	Data Consumer: the agent who will make use of the software produced
-	Data Manager: the agent who makes sure that the quality of the code is met and that the user experience is satisfactory
-	Software publisher: the agent who publishes and makes available the software

Services
-	User guide/ manual: information on how to use the software
-	Software development subsystem (passive): the underlying system supporting the software developer
-	Software publishing subsystem (passive): the system supporting the publication and release of the software, initiated by the software publisher

Contracts
-	Contract: e.g. reuse licenses and intellectual property rights clearance
5.4 Consulting
DEFINITION 
Consulting is a time-based support activity about a situation or a problem offered to another DARIAH member or the DARIAH community. This may cover advice including audit, design or other activities where expertise support and knowledge transfer form the basis of the service. 

5.4.1 Enterprise Viewpoint
Community
-	Consultancy provider community: the community which legally provides the consultancy activity. It holds the expertise to provide and perform it.
-	Consultancy receiver community: the community requesting consultancy and receiving it. 

Roles
-	Consultancy provider: the agent who legally provides the consultancy activity (e.g. institution)
-	Consultancy implementer: the agent who performs the consultancy activity 
-	Consultancy consumer: subject of the consultancy: the agent who instantiates the request for an activity and receives the outcome of the activity. 
-	Consultancy Provision System (passive): ((how do we define this object when put somewhere else)) 

Behaviours
-	Consultancy Management: the behaviour of the consultancy provider,  who overviews the running of the consultancy activity, and ensures the transfer of knowledge.
-	Consultancy Support: the behaviour of the consultancy implementer, giving his expertise 
-	Consultancy Execution: the behaviour of a number of agents (Consultancy provider, Consultancy implementer) performing certain actions in the context of consulting. 
5.4.2 Information Viewpoint
Data
-	Raw Data: notes
-	Documentation: procedure, list of documents used for the planning and execution of the consultancy
-	Report: official output resulting of the consultancy

Agents
-	Consultancy provider: the agent who legally provides the consultancy activity (e.g. institution)
-	Consultancy implementer: the agent who performs the consultancy activity 
-	Consultancy receiver: subject of the consultancy: the agent who instantiates the request for an activity and receives the outcome of the activity. 

Services
-	Supports of communication: external (DARIAH website), internal (team collaboration software such as Confluence Wiki, Basecamp)


Contracts
Very important in this type of in-kind is in fact the agreement and contract side of the consultancy, which is essential to stipulate the detail of the performance, e.g. whether the consultancy is for free or not, how long will it be etc.

5.4.4. Case Study 
The Data Seal of Approval enounces Guidelines that are of interest to data producers and institutions that create digital data, to organizations that archive data, and to consumers of data.
The objectives of the Data Seal of Approval are to safeguard data, to ensure high quality and to guide reliable management of data for the future without requiring the implementation of new standards, regulations or high costs.

An institution requests consultancy to DANS on how to get the Data Seal Of Approval Certification. This institution requiring consultancy is the Consultancy Receiver Community. 
DANS represents the Consultancy Provider Community. As the institution providing consultancy, DANS is the Consultancy Provider. The institution receiving consultancy is the Consultancy Receiver.

5.5 DARIAH Coordination
DEFINITION: This type of contribution involves the coordination of DARIAH activities. The coordination roles that are paid by DARIAH-ERIC can not be considered as in-kind contributions. 
For instance coordination of or cooperation in:
●	National Coordinator coordinates DARIAH activities in his or her country. In the NCC they meet regularly to integrate their national DARIAH activities at the European level. Each DARIAH Member Country has its own National Coordinator.
●	VCC Heads: their work is based on pro-bono activities. A Memorandum of Understanding defines the amount of hours that a VCC head should dedicate to DARIAH per year. 
●	Working Groups (coordinators): their work is based on pro-bono activities. Their work is regulated by a tacit contract 

5.5.1 Enterprise Viewpoint
Communities
-	DARIAH Coordination Community

Roles
-	Coordination Activity Subsystem (passive):
-	Coordination Activity owner: (single or institution) the agent that  has the responsibility of the coordination activity.
-	Coordination Activity provider: an agent (institution) that performs a certain action in the context of the DARIAH coordination 
-	Coordination Activity Implementer: the agent who performs the activity on the behalf of the Coordination Activity provider
-	Coordination Activity consumer/ attendee (active/ passive role): an agent (individual/ institution) that receives, consumes or experiences the outputs created during an activity
-	Coordination Activity Manager: the agent that has a day to day overview of the running of the activity. This role is also the point of contact for issues with the smooth running of the activity

Behaviours
-	Coordination Activity management: the behaviour of the Coordination Activity Manager, who has a day to day overview of the running of the activities. 
-	Coordination Activity support: the behaviour of the support agent, whose task is to support the coordination activities 
-	Coordination Activity execution: the behaviour of the Coordination Activity Implementer, who is responsible to perform a certain action on behalf of the Coordination Activity Provider. 
5.5.2 Information Viewpoint
Data
Data object type: information useful for the participants, internal project documentation (shared documents such as action plans for example), official outputs (official documents)

Agents
-	Coordination Activity owner: (single or institution) the agent that has the responsibility of the coordination activity.
-	Coordination Activity provider: an agent (institution) that performs a certain action in the context of the DARIAH coordination 
-	Coordination Activity Implementer: the agent who performs the activity on the behalf of the Coordination Activity provider
-	Coordination Activity consumer/ attendee (active/ passive role): an agent (individual/ institution) that receives, consumes or experiences the outputs created during an activity
-	Coordination Activity Manager: the agent that has a day to day overview of the running of the activity. This role is also the point of contact for issues with the smooth running of the activity

Services
-	Communication Support: external (DARIAH website), internal (team collaboration softwares such as Confluence Wiki, Basecamp)
-	Processing tool: contribution tool

Contracts 
-	Memorandum of understanding: defines the amount of hours a VCC Head should dedicate to DARIAH a year.
5.5.3 Case Study
A DARIAH institution offers a contribution. The institute fills a self-assessment and submits it via the Contribution Tool. The assessment criteria are provided by the tool. Assessment criteria are offered for each type of contribution. 
This self-assessment is peer reviewed by the appropriate peer review group via the tool, composed of VCC Heads and members of the Working Groups. When the VCC Heads peer-review in-kind contributions, they act as Coordination Activity implementer. The Coordination Activity provider is the peer-reviewing group (composed of VCC heads and Working groups members). It acts on the behalf of DARIAH, which is the Coordination Activity owner. The Coordination Activity Consumer is also DARIAH, since it will beneficiate of the expertise of this group to review in-kind contributions. The Coordination Activity subsystem is represented by the Contribution Tool. DARIAH and the VCC belong the DARIAH Coordination Community.

5.6 Creating Resources
DEFINITION: 

This type of in-kind contribution describes the resources that an agent (institution, individual) creates in order to make them digitally available with the DARIAH community. In this context a “resource” is considered as an asset that supports a certain research activity (e.g. can be the digitized document that was not previously available or the training material to support an educational trajectory).

The resources can also have different forms for example:
-	Text
-	Images
-	Data 
-	Video recordings
-	Audio recording
-	Interactive resources (e.g. quizzes, interactive maps and diagrams etc.) 

If the resource proposed is code, its specificity will make it affiliated with the in-kind contribution “Development of software”.

5.6.1 Enterprise Viewpoint 
Data Creation Community: the objective of the data creation community is to create and/ or collect research data using specific instruments and methodologies.
Within DARIAH this community can be represented by the community of cultural heritage institutions that make available digitally cultural object and/ or metadata of specific collections to researchers. It can also be represented by the organization of a conference that creates ancillary material to support the conference (e.g. abstracts) or by the training material created for an online course (e.g. test, readings etc.)

Data Management Community: The main objective of the data management community is to maintain or improve the quality of the research data for verification and reuse. In the context of this in-kind contribution, the data management community is involved only for what concerns the communication between the data creation community and the data management community about the appropriateness of the data created for its storage and for making sure that the data management community will take good care of the data. 

Data Provision Community: the objective of the Data Provision community is to disseminate and to provide access to the data. Their main objective is to make data accessible and discoverable. 

Roles
-	Data Creation Subsystem (passive)
-	Data Creator: person responsible for the data creation
-	Data Collector: person or organization responsible for the collection of existing data
-	Metadata Creator: person or organization responsible for creating metadata related to the data examined, according to agreed metadata standards. 
-	Data Manager: person responsible for communicating with the Data Creator, and maintaining the quality of the data on a technical perspective (keeping/improving it to defined quality/standards).
-	Data Owner: a person or organisation that owns the data and determines the conditions for deposit/access with the Data Manager.
-	Data Provider: person responsible for making the data accessible and discoverable.
-	Data Discovery System (passive role): a system facilitating discovery of research data and its context.
-	Data Consumer: an agent that requests and receives the research data (for further use).

Behaviours
-	Collect Data: the behaviour of the data creation subsystem performed by the collector and the instrument whereby the data collector records and aggregates observations from the instrument into a dataset.
-	Curate Data: the behaviour performed by the data manager whereby he checks the quality of the data and removes faults. He then adds meaningful documentation (metadata) to the data. 
-	Data Publication: A behaviour by the data provider, the Data Discovery System and the Data Retrieval System for making data for making research data discoverable and accessible.
-	Data Discovery: a behaviour by the data provider, to making the created data discoverable and accessible. 
5.6.2 Information Viewpoint 
Data
-	Data Object Type: (e.g. digitized cultural object or training material for a course): the minimum available information object type that can be shared from the data creator to the data consumer
-	Metadata Object Type: the information object type that describes and contextualizes the data object type

Agents
-	Data Owner: the agent who ultimately owns the data
-	Data Creator: the agent who creates the data
-	Data Collector: the agent who collects already existing data, creating new type of resources
-	Data Manager: agent who makes sure that the data/ resources are of good quality
-	Data consumer: the agents who accesses the data created

Services
-	Digitization service:  information object type that translates the analogue object type into a data object type

Contracts
In this case (creating resources) the use of a standard might be crucial in the harmonization of the data and metadata of a research or heritage institution. The agreement and eventually the contract for this in-kind is represented by the agreement between the resource owner and the data creator (in the sense of digitisation) if they are two different agents. Another agreement can be thought in the case of teaching material between students and teacher, where the agreement  is about the students studying/ reading the material. 
5.6.3. Case Study: Creation of linguistic data 
EASY  is the data archive for the social science and humanities in the Netherlands. Such data archive has been developed and is currently maintained and enriched by DANS, an institute of the Dutch Royal Academy of Science, that has a leading role (nationally and internationally) in the development of data quality policies and research data management plans. 

As such, EASY offers to the research community the possibility to host their data after they have finished their research and therefore can be considered as a candidate for a DARIAH contribution Data Hosting Service. 

In terms of Enterprise Viewpoint, the Data Hosting community is represented by the DANS team, which is the community who acquires, administers and curates the dataset created by the Resources Creation Community (the researcher depositing the datasets). The team at DANS acquires the data (with the support of a submission agreement) through the submission of information packages. 

To all the archived data, DANS applies the principles of the Preservation Policies Data Archiving and Networked Services, which draws the lines of the agreement between the Data Hosting Community and the Resource Creation Community. 

In terms of information Viewpoint, the research outputs and the data delivered to EASY in order to be archived are the main information object type for this type of contribution. According to the recommendation of DANS, the data need to be structured according a series of preferred data and metadata formats and they need to include reference to their accessibility and reuse possibility. A contract (another data object type) will then establish duties and rights for the Data Hosting Community and the Data Resource Community by answering questions like: for how long will the data be maintained? what are the responsibilities of the stakeholders involved?



