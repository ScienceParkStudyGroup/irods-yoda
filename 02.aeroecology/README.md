# Description of a case-study for the Radar Aeroecology group
Three major points:
-Reusability of existing infrastructure
-Accesibility management of varying systems for varying users for varying datasets
-Integration of datasets within and between institutes / organizations. Be able to query a large vault for data which "might" enrich your data
-Integration of datasets as a new product?



# Reusability: Current infrastructure
## Local (UvA)
### S3 storage [IN USE]: fnwi-s0.science.uva.nl
Serves as input (staging) and output (production). Is hosted by FEIOG and part of the FNWI-S0 setup. S3 functionality on top of Samba / network drives through Minio
### uvaRadar (R) library [IN USE]
Serves as predominant research tool. 
Library expands on a industry standard library (bioRad) and acts as a bridge between our infrastructure, existing tools & platform for new tools used for this type of research.
## Remote (Surf)
### Cluster [IN USE]: lisa.surfsara.nl
Serves as main calculation tool for the generation of products out of input files in the staging zone. Directly connects to our S3 datastore, reads input, places output
### Cloud storage [DEPREC]: researchdrive.surfsara.nl
Old storage platform. This platform is deprecated as the performance for our purpose did not meet demands.
### HPC Cloud (VM) [NOT IN USE]: https://ui.hpccloud.surfsara.nl
Not yet in use - depends on development of radar cluster. 
This is a possible tool we might use for a monitoring tool / auto deployement of jobs based on staging area 
### REST api [NOT IN USE] 
Part of future plans to use REST to perform certain BI / routine tasks.

# Remote sources (input) access // KNMI//UK/NO...ENRAM
## European Operational Program for Exchange of Weather Radar Information (EUMETNET/OPERA) 
## MetOffice(s)
## Research institutes


# Irods specifics (whish list?):
## FAIR
### Submission of papers & data, tracking & reusing
## Data / account permission management
### Account management of varying levels for accessing the S3 store. 
### Institute
### Meteorological Organiziations (Governmental Organiziations)
##  Data policy management / access mangement
###  Colaborators, external & internal
### Data ingestion external colaborators
### Data sharing to public without violation of specific licenses
## Data integration
# Multiple source usage (Weather // GPS // ??)
Research questions can be asked depending on the availability of data. Currently, we rely on our own data store with our farmiliar polar volume & vertical profile data. Some research is now extending in enriching their research with the addition of data which in practice describes the same phenomenon but measured with a different measuring tool, strategy and subsequently data format. These data sources are now sparsely combined due to, what I think, is the lack of calibration between the two. Linking these sources by for example metadata: what? where? how? could provide a first order of identifying relationships which are observed in both methodologies. Currently - manual linking of meta data is done as opposed to a being provided an overview with "possible data sources / types".

The other aspect is a growing need for incorporating more data (types) to provide contextual information on an observed phenomenon. As an example, wind and precipitation data can support why or why not a certain migration is or is not observed. Currently, researchers manually combine the data (in sense of searching) and little work is done on the actual combination of the data. 

I doubt that the working of IRODS should be the execution of data merging - but merely provide the overview and basis on which you can. For instance, being able to query across multiple institutes for a set of meta-data (what where how) where the query relies on perhaps "where" and "what and how" would be two unexplored possibilities for a novel research. 

The actual integration should, probably, be left at the user.


# actual use case to test a full workflow
## Description of the use case with the actors and actions


# General Whish list:
## Scalable computing 
For exploratory analysis, scalable computing could prove to be very beneficial. 
Currently, our department is working on scalable computing for a data exploration environment through Jupyter notebook(s).
However, there are many flavors of options that can be used, the exact one depends heavily on the eventual use of the system. 
Now, jupyter notebook is explored to provide a single access point for researchers where existing code can be run efficiently on a large amount of resources.
## Tool server
Closely intertwined with the scalable computing. The difference 
## Database(s) / metrics / insights
Business Intelligence
## Account management
# Cross-institute colaboration
# Data policy management

