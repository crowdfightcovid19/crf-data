# I/O data folder

This folder contains raw and generated data from different scripts in the project.

## Accessing the raw data. 

The following explains how we currently access the data. Most of it is accessed manually but it is meant to be
automatized in the future.

### Volunteers raw data

Volunteers subscribe to the platform filling a Google Form and subscribing to MailerLite (platform used to send 
different kind of emails to the volunteers)

* `Crowdfight COVID-19 volunteer database (Responses).xlsx` is downloaded from Google Drive. It contains 
volunteers information and descriptions from the Google Form that they fill at subscription.
* `~($HOME)/mailerlite_YYYYMMDD-HHMM_<type>.json` is downloaded from MailerLite through the mailerlite_backup.py 
script in a different repository of CrowdFight-COVID19. It contains information about the volunteers 
subscriptions to MailerLite and their interaction with the emails sent.  

### Requests raw data

Requests from researchers arrive to the FreshDesk platform where they are managed, labeled and filled with a given
task list. All this is done manually by coordinators of CrowdFight-COVID19.

* `./freshdesk_tickets/1372943 (XX).zip` is downloaded from the FreshDesk platform. It contains multiple XML files
from which only the `Tickets*.xml` are important. They contain the information about the different requests from the
researchers. 

### Tasks distribution forms raw data

Volunteers receive every 2-4 days an email with a Google Form containing the descriptions of several tasks. They fill
the Google Form indicating how suitable they are for each of the tasks.

* `./task_distribution/drive-download-YYYYMMDDTHHMMSS-001.zip` is downloaded from Google Drive. It contains multiple
`Task distribution YYYYMMDD (Responses).xlsx` with the responses of the volunteers to the different task distribution 
forms sent on the date specified by YYYYMMDD. 

## Generating data

### Pseudonymized data

The previous data contains emails, names and IP addresses that are kept out or pseudonymized during the processing of 
the data. Data is pseudonymized with the command: `make pseudonym_data`, more information can be found in 
the [Makefile](../Makefile). 


### Preprocessed data

Data needs to be cleaned and given a proper format to simplify the functioning of other scripts in the pipeline. 
Data is preprocessed with the command: `make preprocessed_data`, more information can be found in the 
[Makefile](../Makefile). 

### Data for training

Some data is further preprocessed to simplify the functioning of the scripts used to train networks. This data is
generated with the command: `make datatrain`, more information can be found in the [Makefile](../Makefile)

### Vectors data

Tasks and volunteers vectors of semantic embeddings are also stored in this folder. Files of vectors are generated
with the command: `make vectors`, more information can be found in the [Makefile](../Makefile).

### Clusters data

Before sending an email with tasks distribution Google Form to the volunteers, the volunteers and tasks are 
clustered so that volunteers receive the tasks in order of relevance according to their expertise. The clustering
can be run with the command: `make clusters`, more information can be found in the [Makefile]






