# Introduction

## About this Workshop

In this workshop, you will learn how to replicate the content from one WebCenter Content server (referred to as the Source) to another (referred to as the Target) using the Archiver — a Java-based WebCenter Administration utility.

**Estimated Lab Time**: *TBD*

### **Description**

Organizations often require a reliable backup solution for their WebCenter Content data and the ability to seamlessly transfer this data to another WebCenter Content instance. This workshop will guide you through the process of:

* Creating a content archive on the Source instance.
* Transferring and importing the archived content into the Target instance.

### **About Archiver unitlity**
Oracle WebCenter Content (WCC) provides a robust Archiver utility designed to facilitate the export, import, and replication of content between Content Server instances. This functionality is essential for scenarios such as system migrations, content synchronization across environments, and establishing reliable backup and disaster recovery solutions.

## Workshop Objectives

This workshop will guide you through:


* **Configuring the Archiver on the Target Instance:** Setting up the Archiver utility to receive content from the source instance.
* **Setting Up Outgoing Providers:** Establishing connections between source and target instances to facilitate content transfer.
* **Creating and Managing Archives:** Exporting content from the source and importing it into the target instance using the Archiver utility.
* **Automating Replication Processes:** *(Coming soon)* Implementing automated export, transfer, and import operations to streamline content synchronization.
* **Troubleshooting Common Issues:** *(Coming soon)* Identifying and resolving common challenges encountered during the replication process.

### **Prerequisites**

Before proceeding, ensure the following prerequisites are met:

- **Source and Target Instances:** Both the source and target WCC instances should be installed, configured, and operational.
- **Network Connectivity:** Ensure that both instances can communicate over the network, particularly that TCP port 4444 is open and accessible, as it's commonly used for Archiver transfers.
- **Unique Instance Names:** Each WCC instance must have a unique `Instance Name`. Having duplicate instance names can lead to replication failures and data corruption. Verify and, if necessary, modify the `Instance Name` to maintain uniqueness across environments.
- **User Permissions:** Administrative access is required on both source and target servers to configure providers, create archives, and manage replication settings.

### **Learn More**

* [Administering Oracle WebCenter Content - Managing Archives, Collections, and Batch Files ](https://docs.oracle.com/en/middleware/webcenter/content/12.2.1.4/webcenter-content-admin/managing-archives-collections-and-batch-files.html#GUID-D6CDC8D3-28E7-42B5-99F9-096D0BFCAC82)


## Acknowledgements

* **Authors-** Nazar Doroshenko, Development Manager, Oracle WebCenter Content
* **Contributors-** Sameer Chikkerur, Mandar Tengse
* **Last Updated By/Date-** Nazar Doroshenko, May 2025