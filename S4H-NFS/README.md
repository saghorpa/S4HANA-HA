# Deploy S/4HANA using *NFS*

This is a **semi-automated** process to deploy S/4HANA in a highly available manner using *NFS* for ASCS instance.

## What is this about?
This is a “Semi-Automation” method of S/4HANA deployment. ***Why do we call it Semi-Automation?*** Because, this is a combination of ARM templates and linux commands to help build the system.  You can deploy the following two most common and complex scenarios using this method:

| Component |  High availability using pacemaker with NFS |
| --- | --- |
| SAP Application Version |  S/4HANA 1809 |
| HANA DB Version | SAP HANA 2 SPS04 |
| Operating System Version | SuSE 12 SP3 for SAP |
| High Availability for ASCS | ASCS – Pacemaker cluster |
| High Availabulity for DB | HANA – HSR with pacemaker cluster |
| Shared file system | NFS |



## How do it do it?
You download the package from https://github.com/saghorpa/S4HANA-HA/S4H-NFS. The package consists of the following files:

- ARM templates (JSON files)
- NFS- An end to end comprehensive guide for S/4HANA HA deployment using NFS (pdf file)

The procedure has been tested by Microsoft internal SAP on Azure team, and by the several of our partners.

Here are the **pre-requisites** before you begin:

- Azure subscription 
- SAP S/4HANA 1809 bits downloaded
- SAP HANA 2 SPS04 bits downloaded
- SAP Basis, Linux, and Azure infra knowledge
- About 2-3 days of time to install and configure each scenario
- S/4HANA and HANA licenses (optional)
