##Processing Service
###Definition:  
A partner offers a (digital) service that applies some algorithmic processing (statistical analysis, annotation) on given data, or provides means to edit/curate data (e.g. web interface for collaborative editing).  

A processing service is distinct from content hosting service in that it does not store data, but generates new data based on given input. Ideally, processing services are connected seamlessly with hosting service to appear to a user as one (virtual research) environment.

###Enterprise Viewpoint
####Communities
The processing Services 
-	**Data Creation Community:** The Data Creation Community is represented by whom creates or collects data. These data can be the results of digitization of [cultural heritage objects](./DARIAH-RA-Glossary.md#g-cho "glossary description of a cultural heritage object") or research outputs from scientific investigation. 
Within [DARIAH](./DARIAH-RA-Glossary.md#g-dariah "glossary description of DARIAH and link"), this community can be represented by a single or a group of researchers, as well as by a single or a group of institutions. 

-	**Data Processing Community:** this community allows the transformation (editing, curation, visualization) or the enrichment of the data created by the **Data Creation Community** by creating and applying an algorithmic process.

####Data Processing Roles

The following roles within the **Data Creation Community** have been identified:

- **Data Creation Subsystem (passive role):** the community component that represents the data creation community as a whole. 
-	**Data Creator (active role):** the agent or agents responsible for the creation of the data
-	**Instrument Designer (active role):** the agent who is responsible to design, build and maintain the instrument that is used for data collection
-	**Instrument (passive role):** a system that is used by the data collector to collect the data 
-	**Data Collector (active role):** The agent that is responsible to collect the data created by the Data Creator

The following roles within the **Data Processing Community** have been identified:
- **Data Processing Subsystem (passive role):** the community component that represents the data processing community as a whole. 
- **Data Process Service Owner (active/passive role):** the agent who maintains & manages the processor.
-	**Processor Designer (active role):** an agent who builds, maintains and configures an algorithmic processor.
-	**Processor (passive role):** software or service used by the **Process Consumer** that transforms the data.
-	**Process Consumer (active role):** an agent that is responsible for applying the algorithmic process to the data created by the **Data Creation Community**.

#### Data Processing Behaviours
The following behaviour is identified in the Data Processing Community: 

* *Process Data:* the behaviour performed by the **Process Consumer** through the application of the **Processor** (applying an algorithmic process) upon the original data created by the **Data Creation Community**.  

###Information Viewpoint
Differently from the Enterprise viewpoint (where the community was central), for this type of in-kind contribution the information type represents the core of the investigation. The information type needs to be considered in itself, with no reference from the community that created or is responsible for it. 

####Information Object Types:
* *Data:* For the in-kind contribution ‘Processing Services “ data are represented by the algorithm that is necessary to process the input data (Code) and the data themselves, that are the object of the the transformation. Finally, the processed data are also a data type in the information viewpoint and represent the data that are object of the transformation, at the end of the processing. 

* *Agents:* Three are the main agents identified at the information viewpoint level for the Processing Services: the Data Owner, who owns and is responsible for the quality and outcome of the data after their processing. The service owner is responsible for the processing service provided as well as the application of the processing algorithm. The service interface represents the interface between the service owner/ provider and the data owner. 

* *Services:* The algorithmic processing lies at the heart of this in-kind contribution, as it represents the core activity and service that service owner can provide to a data owner.

* *Contract:* In terms of contracts, a Processing Agreement can be identified between the **Data Owner** and the **Process Consumer**. 

<table><tr><th>
Case Study: TextGrid 
</th></tr>
<tr><td>
<p><a href="https://textgrid.de/en" title="TextGrid home page in English">TextGrid</a> is a <a href="./DARIAH-RA-Glossary.md#g-vre" title="glossary description of a VRE and links">virtual research environment (VRE)</a> for researchers in the text-based humanities and cultural studies. Since 2006, TextGrid has been funded by the German Federal Ministry of Education and Research and, today, forms an integral part of DARIAH-DE. TextGrid has a large and growing community of users that roughly fall into the categories of individual researchers and research projects of varying sizes.  
</p><p>
Among other features, it supports the creation of digital editions using free, project-specific and expandable tools and services. Tools, data and methods can be used independently, regardless of operating system, software equipment and location.
</p><p>
TextGrid consists of the TextGrid Laboratory (TGLab), a desktop application for all major operating systems, and the TextGrid Repository (TGRep). TGLab is the central Service Interface which is used as the Instrument by which a Data Owner ingests her research data provided by the Data Creator into the TextGrid storage, which is managed by DARIAH-DE infrastructure partners as the Data Collectors. The data can be used further in TGLab’s tools, the Processors, operated, maintained and supported by DARIAH-DE development partners as Service Owners. Within TGLab the user can use tools such as the Text-Image-Link Editor, a Processor, to enrich images with text annotation and link the image with (parts of) its plain text transcription. This Processed Data can, ultimately, be published to the Hosting Service TGRep.</p>
</td></tr></table>

