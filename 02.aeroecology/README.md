# Description of a case-study for the Radar Aeroecology group

## Current infrastructure
### Local (UvA)
#### S3 storage [IN USE]: fnwi-s0.science.uva.nl
Serves as input (staging) and output (production)
#### uvaRadar (R) library [IN USE]
Serves as predominant research tool 
### Remote (Surf)
#### Cluster [IN USE]: lisa.surfsara.nl
Serves as main calculation tool for the generation of products out of input files in the staging zone.
#### Cloud storage [DEPREC]: researchdrive.surfsara.nl
Old storage platform
#### HPC Cloud (VM) [NOT IN USE]: https://ui.hpccloud.surfsara.nl
Not yet in use - depends on development of radar cluster

# Whish list:
## Scalable computing 
exploratory analysis
## Tool server
exploratory analysis
## Database(s) for
Business Intelligence

# Irods specifics:
## Data / account permission management
### Account management of varying levels for accessing the S3 store. 
### Institute
### Meteorological Organiziations (Governmental Organiziations)
##  Data policy management / access mangement
###  Colaborators, external & internal
### Data ingestion external colaborators
### Data sharing to public without violation of specific licenses



# Remote sources (input) access // KNMI//UK/NO...ENRAM
## European Operational Program for Exchange of Weather Radar Information (EUMETNET/OPERA) 
## MetOffice(s)
## Research institutes

## Data integration
# Multiple source usage (Weather // GPS // ??)
Research questions can be asked depending on the availability of data. Currently, we rely on our own data store with our farmiliar polar volume & vertical profile data. Some research is now extending in enriching their research with the addition of data which in practice describes the same phenomenon but measured with a different measuring tool, strategy and subsequently data format. These data sources are now sparsely combined due to, what I think, is the lack of calibration between the two. Linking these sources by for example metadata: what? where? how? could provide a first order of identifying relationships which are observed in both methodologies. Currently - manual linking of meta data is done as opposed to a being provided an overview with "possible data sources / types".

The other aspect is a growing need for incorporating more data (types) to provide contextual information on an observed phenomenon. As an example, wind and precipitation data can support why or why not a certain migration is or is not observed. Currently, researchers manually combine the data (in sense of searching) and little work is done on the actual combination of the data. 

I doubt that the working of IRODS should be the execution of data merging - but merely provide the overview and basis on which you can. For instance, being able to query across multiple institutes for a set of meta-data (what where how) where the query relies on perhaps "where" and "what and how" would be two unexplored possibilities for a novel research. 

The actual integration should, probably, be left at the user.

## Account management
# Cross-institute colaboration
# Data policy management