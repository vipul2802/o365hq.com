+++
title = "Exchange Online Tenant-to-Tenant migration"
description = "Exchange Online Tenant-to-Tenant migration is the process of moving email data from one Office 365 tenant to another. This can be necessary if an organization merges with another company or if a company splits into multiple entities, and each entity needs its own Office 365 tenant."
date = 2023-04-07

[taxonomies]
tags = ["microsoft 365", "Office 365", "migration"]
+++

*This article is part of a series. Check out our full* *[Microsoft 365 tenant-to-tenant migration Guide](https://o365hq.com/blog/microsoft-365-tenant-to-tenant-migration-guide/)*

### Introduction

Exchange Online Tenant-to-Tenant migration involves exporting mailbox data from the source tenant and importing it into the destination tenant. There are several methods for performing this migration, including using third-party tools or Microsoft's native migration tools. 

It is important to plan and prepare for the migration, as there are many factors that can impact the success of the migration, such as the size of the mailbox data, the number of mailboxes to be migrated, the network bandwidth available, and the level of user disruption that can be tolerated. Proper planning, testing, and execution of the migration can help ensure a successful transition to the new tenant with minimal downtime and data loss. 

### Prerequisites 

Before you begin an Exchange Online Tenant-to-Tenant migration, there are several prerequisites that one needs to be aware of: 

1. The migration will require administrative access to both the source and destination tenants. 
2. Each user mailbox in the destination tenant must have a valid Office 365 license to receive the migrated data. 
3. The domain being migrated must be verified in both the source and destination tenants. 
4. Administrative permissions must be granted to the migration account in both the source and destination tenants. 
5. Multi-factor authentication should be enabled for all accounts involved in the migration process. 
6. A comprehensive plan should be created, including a timeline for the migration, data mapping, and contingency plans for any issues that may arise during the migration. 

### Migration process 

**Step 1. Plan the migration**

* Create a detailed plan that includes the timeline for the migration. 
* Identify the number of mailboxes to be migrated and the type of data to be migrated. 
* Define the migration method to be used. 

**Step 2. Prepare the source and destination tenants**

* Verify the domains in both the source and destination tenants. 
* Create administrative accounts with appropriate permissions. 
* Assign Office 365 licenses to the destination tenant users. 

**Step 3. Prepare the migration tools and the data for migration**

* Install and configure the migration tools that will be used for the migration, such as Microsoft's native migration tools or a third-party tool. 
* Export the mailbox data from the source tenant and prepare it for import into the destination tenant. This may involve creating CSV files, mapping source and destination mailboxes, and cleaning up mailbox data to minimize the amount of data that needs to be migrated. 

**Step 4. Perform the migration**

* Use the migration tool to transfer the mailbox data from the source tenant to the destination tenant. This may involve batch migrations or performing the migration all at once. 
* Monitor the migration process to ensure that all mailbox data is successfully migrated.  

**Step 5. Post-migration tasks**

* Address any issues that arise during the migration, such as failed migrations or corrupted data. 
* Verify that all mailbox data has been successfully migrated to the destination tenant and that users can access their email accounts in the new tenant. 
* After verifying the successful migration, decommission the source tenant and remove any unnecessary data or accounts. 

The Exchange Online Tenant-to-Tenant migration process can be complex, but following these steps and properly planning and preparing for the migration can help ensure a successful transition to the new tenant. 

### Challenges and common issues 

Exchange Online tenant-to-tenant (T2T) migration can be a complex and challenging process, here are some common challenges and issues to keep in mind: 

* **Domain Name System (DNS) Changes**: When moving to a new Tenant, all DNS records need to be updated, including MX records, Autodiscover records, and other important records that are associated with email delivery. 
* **Tenant Setup**: The new Tenant needs to be configured with the correct settings, such as retention policies, archiving settings, and other configurations that match the existing Tenant. 
* **Permissions and Access**: Permissions and access levels need to be reviewed and configured for each user account, ensuring that users have the appropriate level of access to the resources they need. 
* **Third-Party Integration**: If the existing Tenant is integrated with third-party applications or services, these integrations need to be reconfigured to work with the new Tenant. 
* **Public Folders**: If there are public folders in the existing Tenant, these need to be migrated to the new Tenant, which can be a complex and time-consuming process. 
* **Customizations and Add-Ons**: Any customizations or add-ons that were installed on the existing Tenant need to be reinstalled and configured on the new Tenant. 
* **Testing and Verification**: Once the migration is complete, it is essential to thoroughly test and verify that all email is being delivered correctly and that users have the appropriate access to resources. 
* **Downtime**: Depending on the complexity of the migration and the number of users involved, there may be some downtime associated with the migration. This downtime needs to be minimized as much as possible to avoid disruption to business operations. 
* **Data Loss**: During the migration process, there is always the risk of data loss or corruption. It is essential to have a comprehensive backup and recovery plan in place to minimize the risk of data loss. 

In summary, tenant-to-tenant migration can be a complex and challenging process, but with careful planning and execution, it is possible to minimize the impact on users and ensure a successful migration. It is essential to understand the common challenges and issues associated with T2T migration and take steps to mitigate them. 

