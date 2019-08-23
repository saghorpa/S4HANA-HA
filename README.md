# An end to end S/4HANA deployment with High Availability in Azure

This is a **semi-automated** process to deploy S/4HANA in a highly available manner. This method offers both NFS and ANF deployment methods for ASCS instance.

## What is this about?
This is a “Semi-Automation” method of S/4HANA deployment. ***Why do we call it Semi-Automation?*** Because, this is a combination of ARM templates and linux commands to help build the system.  You can deploy the following two most common and complex scenarios using this method:

| Component | High availability using pacemaker with NFS	| High availability using pacemaker with Azure NetApp File (ANF) |
| --- | --- | --- |
| SAP Application Version | S/4HANA 1809 | S/4HANA 1809 |
| HANA DB Version | SAP HANA 2 SPS04 | SAP HANA 2 SPS04 |
| Operating System Version | SuSE 12 SP3 for SAP | SuSE 12 SP3 for SAP |
| High Availability for ASCS | ASCS – Pacemaker cluster | ASCS – Pacemaker cluster |
| High Availabulity for DB | HANA – HSR with pacemaker cluster | HANA – HSR with pacemaker cluster |
| Shared file system | NFS - Pacemaker cluster	| ANF (Azure Netapp Files) |


## Why do I use this method?
When you want to build and configure highly available S/4HANA system with deep understanding of each layer like infrastructure, clustering, SAP Application, HANA, Replication etc. - You use this method!

By following a comprehensive document with screen shots, you learn it by doing each step on your own. **You understand how each step is performed and why it is being done.**

After you complete manual installation, you are good to use automation approach for a quick and repeatable deployment. 

Here are some **benefits** for you:

- Gain hands-on experience 
- Deploy and configure complex SAP HA setup with confidence
- Create a demo or a reference environment for your CoE
- Exercise your HA test scenarios

## How do it do it?
You download the package from https://github.com/saghorpa/S4HANA-HA. The package consists of the following files:

- ARM templates (JSON files)
- ANF- An end to end comprehensive guide for S/4HANA HA deployment using ANF (pdf file)
- NFS- An end to end comprehensive guide for S/4HANA HA deployment using NFS (pdf file)

Based on the scenario you want to test out, you start with the respective deployment guide (NFS or ANF). These guides enable you to perform end to end deployment. These are the comprehensive guides (110+ pages each) with screen shots, and common problems with their resolution.

The procedure has been tested by Microsoft internal SAP on Azure team, and by the several of our partners.

Here are the **pre-requisites** before you begin:

- Azure subscription 
- SAP S/4HANA 1809 bits downloaded
- SAP HANA 2 SPS04 bits downloaded
- SAP Basis, Linux, and Azure infra knowledge
- About 2-3 days of time to install and configure each scenario
- S/4HANA and HANA licenses (optional)

