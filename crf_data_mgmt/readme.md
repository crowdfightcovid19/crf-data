# crf_data_mgmt

## Info 
This folder contains data generated with the `crf_data_mgmt` Python module by joining information 
from the datasets of the different systems (Google Forms, MailerLite, or FreshDesk.

## Generated data
Information to get the generated data can be found in the [crf-data-mgmt repository](https://github.com/crowdfightcovid19/crf-data-mgmt)

## Directory structure
    .
    ├── volunteers_hashes.csv    # Generated by crf_data_mgmt.pseudonymization. Data from Google forms (task_distribution, volunteers) and Mailerlite
    ├── volunteers.csv           # Generated by crf_data_mgmt.joining. Data from Google forms (task_distribution, volunteers) and Mailerlite.
    └── tasks.csv                # Generated by crf_data_mgmt.joining. Data from Google forms (task_distribution) and FreshDesk
        
