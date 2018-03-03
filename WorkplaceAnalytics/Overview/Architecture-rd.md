---
# Metadata Sample
# required metadata

title: Workplace Analytics - How it Works
description: This is a Checklist to introduce what is required to implement Workplace Analytics for your Organization
author: rodonahu
ms.author: rodonahu
ms.date: 01/19/2018
ms.topic: get-started-article
ms.prod: mya
---

# Architecture / How it Works

<CENTER>
![Architecture Diagram](../Images/WpA/Overview/Architecture.png) </CENTER>
Workplace Analytics leverages Office 365 collaboration data to deliver powerful new insights for enterprise productivity. It provides a way for companies to understand the communication behaviors and collaboration patterns across their organization and how they influence productivity and corporate performance.

Workplace Analytics analyzes Office 365 [email and calendar header level metadata](Privacy-And-Data-Access.md) and combines it with organizational data from line of business applications.  By combining these datasets, analysts are able to provide a [variety of organizational insights](http://insights.office.com). Workplace Analytics provides a workbench to run custom analysis and pre developed aggregated dashboards.  All data is owned by the customer and stored within the O365 Compliance Boundary pursuant to the [Office 365 Compliance Framework](http://go.microsoft.com/fwlink/p/?LinkId=615657).


By design, Workplace Analytics provide organizations with choice:
* Our customers decide the scope of mailboxes to analyze.
* Our customers decide who within their organization has access to de-identified datasets and aggregated visual dashboards
* Our customers configure options to exclude specific meeting and email metadata from analysis as directed by their legal and HR teams

Our [Privacy and data access document](Privacy-And-Data-Access.md) describes these considerations in greater detail.


## Data Inputs
It is important to understand the data that is required to run the system, and the form that is generated that is accessed by analysts who can utilize the service.  The image below provides context into this. 

<CENTER>
![Workplace Analytics Data Flow](../Images/WpA/Overview/Flow.png)
</CENTER>

**Collaboration Data**|**Organizational Data**
:-----:|:-----:
Header information from emails|PersonId,Organization,ManagerId, Layer,Timezone,Level,Location, EffectiveDate|
Header information from Meetings|*At a minimum, the above data fields are required for the population scope that you are analyzing.*

>[!Important]
>Attachments and text in the body of emails and meetings are never used by Workplace Analytics.


## Data outputs

**Output type**|**Example**|**Role that has access**
-----|-----|-----
De-Identified Row Level Data|[Sample.csv](../ExamplePersonQuery.csv)|Analyst
Meeting Query Output|[Sample.csv](../ExampleMeetingQuery.csv)|Analyst
Meeting Query output with subject lines encrypted|[Sample.csv](../ExampleMeetingHASHQuery.csv) |Analyst
Group Query|[Sample.csv](../ExampleGroupQuery.csv) |Analyst
-----|-----|-----
Visual Dashboards with Minimum Aggregation Threshold||Analyst, Analyst (Limited)
Data Sources | |Administrator 

## Privacy Options
* Include Subject lines – As part of a meeting query, an administrator can choose to have meeting subject lines encrypted
* Minimum group size - By default our aggregated dashboards default to a minimum group size of 5, this can be increased to a larger number as needed

### Exclusion
All exclusion occurs before metadata is processed within the Workplace Analytics data engine
>[!Important]
>By default, Private meetings and email with digital rights management enabled are automatically excluded.

Customers can exclude any meeting or mail metadata based on the following parameters, (which may have impact on analysis):
* Subject lines – provide keywords to exclude from analysis
* Domains – exclude involving specific domains from the dataset
* Email addresses - exclude content involving specific email addresses from the dataset

### Related topics

[Configure settings for Workplace Analytics] (../use/settings.md) 

[Privacy and data access](Privacy-And-Data-Access.md)

## FAQ

### How does the Workplace Analytics Service handle data?
As part of the Office 365 offering, we are currently a Category A Office 365 service, Moving towards Category C. Please visit the [Office 365 Trust Center Top 10 security and privacy features] (https://products.office.com/en-us/business/office-365-trust-center-top-10-trust-tenets-cloud-security-and-privacy) and [Office 365 Compliance Framework](http://go.microsoft.com/fwlink/p/?LinkId=615657) for more information about our data handling standards.

### Can you describe the de-identification process?
Workplace Analytics processes metadata from Office 365 email and calendar. Email addresses are never shown in Workplace Analytics through dashboards or query results. The Workplace Data Engine de-identifies by using a symmetric hashing to ensure that supplemental organizational data can be added when needed. Encryption keys are securely maintained by Microsoft only allowing programmatic access.



### Is Workplace Analytics compliant with workers councils?
