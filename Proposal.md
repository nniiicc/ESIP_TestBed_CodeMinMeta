
<center><h1>A Minimal Metadata Standard for ESIP Software</h1></center>

### Project Description 

The discovery and meaningful reuse of research software depends, in part, on accurate and meaninful descriptive metadata. While a number of software metadata standards exist, these are often too specific (e.g. focused on a narrow stakeholder group or programming language) or too generic (i.e. extensions of metadata schemas used for related digital objects- such as DCMI) to be used in research domains like the geosciences.

This test bed project will explore the deveolopment of a minimal metadata standard for science software in JSON-LD - a lightweight semantic format. We will build off of the the "code as a research object" project by Mozilla Sciene, Github, and Figshare, in particular the [ongoing work](https://github.com/mbjones/codemeta) of Matt Jones at NCEAS. 

Our initial work will include the following:

1. Completing a cross walking exercise that maps attribute value pairs from different existing software metadta standards. These include (but are not limited to):
 
- [Software Ontology (SWO)](http://www.jbiomedsem.com/content/5/1/25)
- [eml-software](http://knb.ecoinformatics.org/sofwtare/eml)
- [EBM Tools database](http://www.ebmtools.org/)
- [DataONE Software registry](https://www.dataone.org/software-tools)
- [Winning model documentation](https://www.kaggle.com/wiki/WinningModelDocumentationTemplate)
- [MyExperiment workflow repository](http://www.myexperiment.org/)
- Language/System specific package frameworks
    - [Debian packages](http://www.fossology.org/projects/fossology/wiki/Debian_metadata)
    - [CRAN R packages](e.g. http://cran.r-project.org/web/packages/spBayesSurv/index.html)
    - [RPM packages](e.g. http://rpmfind.net/linux/rpm2html/mirroring.html)

2. From this crosswalking exercise, we will work in conjunction with other domains to create a minumum, or core, set of variables that can reliably describe the form and function of research software. This will include two rounds of use cases from the ESIP community (more details below). 

**Some questions and some (preliminary answers)** 

*Doesn't the DOAP project already provide an ontology for describing science software?*

The Description Of A Project (DOAP) ontology is very relevant to this project- but in short, No. 

[DOAP](https://github.com/edumbill/doap) proposes an "XML/RDF vocabulary to describe software projects, and in particular open source projects" 

Here, we're interested in exploring a number of different standards, including DOAP - and finding a minimal - or 'core' set of attribute value pairs (in the [Dublin Core](http://dublincore.org/documents/dces/) / [Darwin Core](http://rs.tdwg.org/dwc/)sense) for describing scientific software - notably Earth System Science software that is developed and used in the ESIP community. 

The limitations to depending - solely- on DOAP for doing this are: 

1. It is aimed at RDF - and well, RDF gets complicated quickly. We want to do something lightweight and easily adoptable. 

2. Part of the ambition in using JSON-LD is so that metadata creation can be automated in the future... and that future seems a lot more distant in an RDF / DOAP world.  

*Why JSON-LD?*

[JSON-LD](http://json-ld.org/) is a lightweight format that offers semantic meaning at a substantially lower barrier of creation than RDF, it has emerged over the last 2-3 years as the standard for serving data via APIs, and more importantly for our work here, it can leverage existing ontologies, like 'creative works' in [schema.org](http://schema.org/Code), for describing a codebase.

*Are there any other benefits to working with existing efforts**

This coordinated work should make it possible for tools like [Fidgit](https://github.com/openjournals/fidgit) -  developed to lower the barrier to archiving and obtaining a persistent identifier for code -  to be leveraged and used by a broader network of software archves. 

*How does the ESIP community benefit from this work?*

After completing the crosswalking exercise we will complete 3-5 use cases from ESIP software. This will include working with a software producer to create the metadata using our minimum standard -and then asking users (potential and actual) of that softare to judge the quality, and meaningfullness of these descriptions. 

We will report on this work at the 2015 ESIP Summer Meeting, and contribute our findings back to the 'code as a research object' project. At the summer meeting we will solicit another 3-5 candidate use cases, and complete these with the refined minumum standard. 

This work will produce a white paper with best practices for creating metadata using the standard. 

We are largely seeking funds in order to formally publish the findings from our use cases in an open access journal. 

**This sounds optimistic. What are the known problems in existing efforts?**
 
- *Controlled vocabulary* : This will be especially important in deciding on ESIP relevant CV for subject categories (e.g. we can do better than the original proposal to use [PLoS's taxonomy](http://www.plosone.org/taxonomy) for academic subjects)
 
- *Function of software* : How do we "uniformally"  the *function* of software? This will require best practices guidelines and likely to be major contribution of use cases. 

### Timeline

The activities described above will be carried out following the schedule below:

![](https://raw.githubusercontent.com/nniiicc/ESIP_TestBed_CodeMinMeta/master/Images/Gantt-MinMeta.png)


### Names and Roles of Team Member

| Name | Role | Description |
|-----------|-----------|------------|
| Nic Weber | Role | PhD candidate in Information Science at University of Illinois. Experience in developing standards and policy for Data Conservancy, and linked data applications. |
| You  | Your Role | Your qualifications |


### Budget

| Item                                                                    | Estimated Cost | Explanation                                                                                        |
|-------------------------------------------------------------------------|----------------|----------------------------------------------------------------------------------------------------|
| Poster Creation (ESIP Winter Meeting)                                   | 65             | Cost of printing poster                                                                            |
| Poster Submission (AGU)                                                 | 75             | Cost of submission to AGU                                                                          |
| Poster Creation (AGU)                                                   | 65             | Cost of printing poster                                                                            |
| Publication in Open Access Journal ( target: Earth Science Informatics) | 3000           | [Open access fee for Spring Journals](http://www.springer.com/gp/open-access/springer-open-choice) |
| **Total**                                                                  | 3205           |                                                                                                    |


