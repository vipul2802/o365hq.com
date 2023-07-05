+++
title = "SharePoint Online tenant-to-tenant migration"
description = "SharePoint Online tenant-to-tenant migration refers to the process of moving SharePoint content, configurations, and settings from one Microsoft 365 tenant to another."
date = 2023-06-29

[taxonomies]
tags = ["microsoft 365", "sharepoint online", "Office 365", "migration"]
+++

### Introduction

SharePoint has become one of the key collaboration platforms for organizations all over the world. Often, modern enterprises face the situation when they are forced to migrate from one tenant to another. SharePoint Online tenant-to-tenant migration is one of the essential steps required at the time of mergers and acquisitions when businesses need to change tenants as a part of their re-branding efforts. In this case, organizations may need not only data migration but also the migration of company documents, sites, collections, libraries, and content with design, structure, and permissions from one environment to a new one.  

### Prerequisites 

1. Make sure you have a Microsoft 365 tenant with SharePoint Online licenses. 
2. Someone from your organization must have admin access to your SharePoint Online. 
3. Identify a dedicated point of contact responsible for collaboration with the appointed service provider to communicate with them before initiating the migration on any customizations and to coordinate any outside vendor resources and schedules. 
4. Plan site(s) structure and permission for SharePoint Online. 
5. Configure all networking equipment, such as load balancers, routers, firewalls, and switches, and provide access to the organization’s resources such as servers, systems, etc. when needed. 
 
### Migration process

**Step 1. Prepare the source system environment for migration**

* Evaluate and analyze the content. 
* Identify the size and types of data that need to be migrated and perform pre-migration source system health check 
* Define the versions of the files that should be available on the new SharePoint Online tenant. 
* Optimize the project`s size by estimating the number of files that need to be migrated.

**Step 2. Prepare the target environment and initiate the migration**

* Create an account with SharePoint Online admin or Site Collection admin rights. 
* Create site libraries and schemas if needed. 
* Replicate the structure of the document library along with any customizations. 
* Create endpoints and provide authentication to the tool for the source and target environments. 

**Step 3. Perform the migration**

* Review the required permissions, prerequisites, and endpoints. 
* Choose the appropriate migration tool or service, this can be either a built-in Microsoft data migration tool, third-party migration tools or custom-built scripts. 
* Migrate data from the source SharePoint Online tenant to the target tenant. 

You should keep in mind that the migration steps may vary based on the number of users within your organization. If you have just a few users, the best approach is to move all the data in a single pass. If the number of users is high, some of the supported items can be first moved before a specific date, and the remaining data can be migrated later. 

**Step 4. Post-migration tasks**

* Verify the data migration and perform the final migration. 
* Check the migrated items, errors, and other critical data. 
* Test the data and ensure that all the content and permissions are in place and working as expected. 
* Monitor the system for any issues or errors post-migration. 

### Challenges and common issues 

SharePoint tenant-to-tenant migration projects can be quite complex and time-consuming. They require certain knowledge and specialized skills to perform the migration smoothly and without disruption. Aligning SharePoint data requires careful planning: 

* Data volumes can be quite large, and the documents are frequently changing, unlike mail data. 
* In single-event migrations, the required UPN changes during the migration will require re-mapping the source to target. 
* There should be enough space for the migrated data. All the content must be in an organized and structured manner. 
* A lot of customizations need to be set up during the migration. Also, the configurations and customizations on the old tenant must be rebuilt. 
* The risk of data loss is still high even after moving data to an Azure-hosted file share and migrating the content to the new tenant. 
* During large-scale cloud migration projects, only the administrator can transfer the data on behalf of the entire organization.  

 