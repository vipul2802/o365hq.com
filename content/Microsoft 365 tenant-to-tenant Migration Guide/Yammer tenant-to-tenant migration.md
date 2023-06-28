+++
title = "Yammer tenant-to-tenant migration"
description = "Yammer tenant-to-tenant migration is the process of transferring Yammer network data from one Yammer network (tenant) to another. This might be necessary in situations such as company mergers, acquisitions, or divestitures, where two separate Yammer networks need to be combined or separated. "
date = 2023-06-27

[taxonomies]
tags = ["microsoft 365", "yammer", "Office 365", "migration"]
+++

### Introduction

Yammer tenant-to-tenant migration is different from migrating Yammer data to another platform or application, such as moving Yammer data to a different social network or collaboration tool. Tenant-to-tenant migration specifically involves transferring data between two Office 365 tenants while preserving the existing Yammer network structure and features. During the migration process, all data within the Yammer network, including users, groups, messages, files, and other Yammer content, is transferred from the source tenant to the target tenant. The migration process can be complex and may require careful planning and execution to ensure a smooth transition with minimal disruption to users. 

### Prerequisites   

Before starting a Yammer tenant-to-tenant migration, there are several prerequisites that need to be met to ensure a smooth and successful migration. Here are some of the most important prerequisites to consider: 

1. Verify the Yammer network is eligible for migration. The network must be part of an Office 365 subscription and use a supported Yammer configuration. 
2. The target tenant must also have an active Office 365 subscription and meet the prerequisites for Yammer. Additionally, the target tenant must be properly configured to receive Yammer data. 
3. User permissions and roles should be defined and correctly assigned for both the source and target tenants.  
4. If the Yammer network includes customizations or third-party integrations, these need to be assessed and accounted for during the migration planning phase. 
5. If there are DNS or email changes associated with the migration, these need to be planned and communicated to users in advance to minimize disruption. 
6. Identify a migration tool or service and test it before beginning the migration to ensure compatibility and optimal performance. 
7. Users should be informed of the migration process and provided with training and support to ensure a smooth transition. 

### Migration process 

The Yammer tenant-to-tenant migration steps may vary depending on the specific requirements of the migration. Here are some general steps involved in a Yammer tenant-to-tenant migration: 

**Step 1. Plan the migration**

It is important to understand the structure, usage, and content of both Yammer networks to determine the scope of the migration and any potential issues that may arise. Determine the migration approach, identify the migration tools that will be used, and create a detailed migration plan that includes timelines, responsibilities, and contingency plans. 

**Step 2. Prepare the source and the target Yammer network**

This involves taking steps to ensure that the source Yammer network is ready for migration and the target Yammer network is ready to receive data from the source Yammer network. This may include disabling the automatic provisioning of users, cleaning up data, and making necessary changes to user permissions. 

**Step 3. Perform the migration**

Use migration tools to transfer Yammer network data from the source network to the target network. This may include transferring user accounts, groups, messages, files, and other Yammer content. 

**Step 4. Verify the migration**

After the data transfer is complete, verify that all data has been successfully migrated and is accessible in the target Yammer network. Communicate with users about the migration and provide training and support as needed to ensure a smooth transition. 

### Challenges and common issues 

Yammer tenant-to-tenant migration can cause several potential challenges and common issues that can arise. Here are some of the most common challenges and issues you may encounter during a Yammer tenant-to-tenant migration: 

* The source and target Yammer networks may have different configurations, which can result in compatibility issues during the migration process. 
* If data is not migrated properly or is corrupted during the transfer, it can result in data loss or corruption, which can cause issues in the target Yammer network. 
* If the Yammer network includes third-party integrations, these may need to be reconfigured or may not be compatible with the target Yammer network. 
* Users may experience disruption or changes to their workflows during the migration process, which can impact user adoption and overall productivity. 
* Insufficient communication and training to users can lead to confusion and frustration during the migration process. 
* DNS or email changes associated with the migration can result in temporary email delivery issues or other disruptions that can affect user experience. 
* There may be periods of downtime or service interruption during the migration process, which can impact user productivity and cause frustration.

To mitigate these challenges and issues, it is important to plan and prepare thoroughly, engage with Yammer experts and third-party migration services, and communicate effectively with users throughout the migration process. It is also recommended to conduct testing and validation before, during, and after the migration to ensure a successful and smooth transition. 

