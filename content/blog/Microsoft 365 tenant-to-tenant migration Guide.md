+++
title = "Microsoft 365 tenant-to-tenant migration Guide"
description = "At the time of mergers and acquisitions, organizations might need a migration inside the Microsoft 365 cloud platform. The migration process requires preparation and additional planning to avoid Data Loss and bounced emails."
date = 2021-11-26

[taxonomies]
tags = ["microsoft 365", "migration"]
+++

### What is a tenant-to-tenant migration?

A Microsoft 365 tenant is an individual and unique customer account that provides an environment for controlling Microsoft 365 users, services, and data. Tenants are hosted on Microsoft’s cloud servers, which are redundantly backed up and spread out all over the world. Microsoft 365 tenants are used in a variety of ways depending upon the needs of different customers, and licensing determines which features get unlocked.  

Tenant-to-tenant migrations involve the migration of mailboxes and service settings from one Microsoft 365 tenant to another one. 

### When do I need a tenant-to-tenant migration? 

The number of cloud adoptions among businesses is increasing each day. There are several architecture approaches for mergers, acquisitions, divestitures, and other scenarios that might lead you to migrate to a new cloud tenant: 

**Microsoft 365 tenant name change**

Once you create a tenant with the name, there is no option to change it. So, it's really important to choose the right name before creating a tenant. In this case if you want to use a different tenant name, you will need to create a new tenant and move/migrate data and users to it. 

**Microsoft 365 tenant location (region) change** 

When you create a new Microsoft 365 tenant account, it automatically checks up the external IP that generated the request and provisions the tenant in that particular region. You cannot change the Microsoft 365 tenant region as Microsoft has already created the specific instances for all workloads and secured the required namespaces which cannot be modified. The only way to change the tenant location is to create a new tenant on your desired location and migrate the data from the old to a new one. 

**A merger or an acquisition**

Dealing with a company merger or acquisition can be challenging as this involves migrating data to Microsoft 365 or merging tenants. There are several scenarios you can consider at the time of mergers and acquisitions: 

* *Tenant-to-tenant migration without rebranding.*
You may use this scenario if you are selling your business unit and brand identity. Identities will migrate to a target tenant and will keep the existing domain as part of the migration. 

* *Tenant-to-tenant migration with rebranding.* 
This business scenario is used when the business unit adopts the target company’s branding. In this case identities will migrate to a new target tenant and will change the brand identity as part of the migration. 

* *Cloud tenant move.*
When you need to split users across two tenants, you should consider cloud tenant move. If you follow this scenario, identities will remain in the source tenant, but all users in the affected domain and all workloads are moved to a new cloud tenant.  

![Microsoft 365 tenant-to-tenant migration](/img/T2T.png)

### What are the services that require data migration?

Tenant-to-tenant migration involves the migration of a large number of services. We would like to indicate the most frequently used types of services that almost always require data migration:  

**[Exchange Online tenant-to-tenant migration](https://o365hq.com/blog/exchange-online-tenant-to-tenant-migration/)**

Commonly, during mergers or divestitures, organizations need the ability to move users and content into a new tenant. This type of service involves the migration of mailboxes from one tenant to another one in the same Exchange Online service. Exchange Online mailbox migrations are supported for tenants in hybrid or cloud only, or any combination of the two. The move process includes tenant authorization checks during mailbox synchronization and finalization. 
  
**[SharePoint Online tenant-to-tenant migration](https://o365hq.com/blog/sharepoint-online-tenant-to-tenant-migration/)**

Sometimes during mergers companies may require not only data migration from one environment to a new one, but also the migration of documents, sites, collections, libraries, and lists along with their permission and design. [SharePoint Online tenant-to-tenant migration](https://o365hq.com/constructor/services?item=ITPWW340MIGOT) implies the migration of content with design, structure, and permissions from one SharePoint Online tenant to another. 
  
**[Microsoft Teams tenant-to-tenant migration](https://o365hq.com/blog/teams-tenant-to-tenant-migration/)**

Organizations are increasingly looking for solutions to enhance their communication and collaboration capabilities. [Microsoft Teams tenant-to-tenant migration](https://o365hq.com/constructor/services?item=ITPWW370MIGOT) can pose some risks and challenges as it involves the migration of a large number of components, documents and the whole your Microsoft Teams structure from one Microsoft 365 tenant to another. 
 
**[OneDrive tenant-to-tenant migration](https://o365hq.com/blog/onedrive-tenant-to-tenant-migration/)**

[OneDrive file migration to another tenant](https://o365hq.com/constructor/services?item=ITPWW450MIGOT) can become a significant challenge if a company plans to combine tenants after a merger or an acquisition. OneDrive for business is a part of Microsoft 365, it lets you share and collaborate on work documents with co-workers, so it is essential to perform the file migration with minimal downtime for your employees.  

**[AAD user accounts and groups tenant-to-tenant migration](https://o365hq.com/blog/aad-user-accounts-and-groups-tenant-to-tenant-migration/)**

Migrating Azure Active Directory (AAD) user accounts and groups from one tenant to another can be a complex process, especially when it involves tenant-to-tenant migration. During AAD user accounts and groups tenant-to-tenant migration, the goal is to transfer user accounts and groups along with their associated attributes, group memberships, and permissions from the source tenant to the target tenant. This ensures that users can seamlessly access resources and collaborate within the new tenant environment without disruption.

**[AAD guests accounts tenant-to-tenant migration](https://o365hq.com/blog/aad-guests-accounts-tenant-to-tenant-migration/)**

AAD guests accounts tenant-to-tenant migration involves migration of guest user accounts from one Azure Active Directory (AAD) tenant to another. It's important to note that migrating guest accounts from one tenant to another can have limitations and challenges. Depending on the nature of the migration and the systems involved, some limitations may arise, such as the loss of certain data or the need to recreate permissions and access configurations in the target tenant. Additionally, guest account migration may require coordination and collaboration with the administrators of both the source and target tenants to ensure a smooth transition. As with any tenant-to-tenant migration, thorough planning, testing, and communication are crucial to minimize disruptions and ensure a successful migration of guest accounts between AAD tenants.

**[Yammer tenant-to-tenant migration](https://o365hq.com/blog/yammer-tenant-to-tenant-migration/)**

Yammer is a social networking platform for organizations that enables communication and collaboration among employees.
Tenant-to-tenant migration of Yammer involves moving Yammer networks, groups, conversations, files, and other data from the source tenant to the target tenant while preserving data integrity and ensuring a seamless user experience. This type of migration is typically necessary during organizational mergers, acquisitions, divestitures, or restructuring that involve transitioning to a new Microsoft 365 tenant. It's important to note that Yammer tenant-to-tenant migration can have limitations and complexities depending on the specific scenario and it is recommended to thoroughly plan and test the migration process in a non-production environment before performing the actual migration.

**[Microsoft Forms tenant-to-tenant migration](https://o365hq.com/blog/microsoft-forms-tenant-to-tenant-migration/)**

Microsoft Forms is an online survey and form creation tool that allows users to create surveys, quizzes, and polls. Microsoft Forms tenant-to-tenant migration involves the process of transferring Microsoft Forms data, including forms, responses, and settings, from one Microsoft 365 tenant to another. When organizations undergo mergers, acquisitions, or restructuring, it may be necessary to migrate Microsoft Forms data from one tenant to another to consolidate data or ensure continued access to existing forms and responses.

**[Azure AD joined devices tenant-to-tenant migration](https://o365hq.com/blog/azure-ad-joined-devices-tenant-to-tenant-migration/)**

Tenant-to-tenant migration of Azure AD joined devices typically occurs during organizational mergers, acquisitions, divestitures, or restructuring that involve transitioning to a new Azure AD tenant. The migration process involves moving the device registrations, configurations, and associated user profiles from the source tenant to the target tenant. During the Azure AD joined devices tenant-to-tenant migration process, devices joined with the source Azure AD tenant are un-joined and re-joined with the Azure AD in the target tenant. This process ensures that the devices are fully integrated and managed under the new tenant.

**Intune configuration tenant-to-tenant migration**

Microsoft Intune is a cloud-based service that enables organizations to manage and secure their mobile devices and applications. Intune configuration tenant-to-tenant migration process involves moving the device management policies, configurations, app deployments, and other Intune settings from the source tenant to the target tenant. This type of migration can have limitations and complexities depending on the specific scenario. Some considerations include the loss of certain data or settings during the migration, the need to re-enroll devices in the target tenant, and potential disruptions to device management during the migration process.

**AAD Applications registrations/thirds party services integration tenant-to-tenant migration**

AAD applications are used to provide access to resources and services in Azure AD. AAD application registrations and third-party services integration tenant-to-tenant migration refers to the process of transferring Azure Active Directory (AAD) application registrations and their associated integrations with third-party services from one AAD tenant to another. During organizational mergers, acquisitions, divestitures, or restructuring, it may be necessary to migrate AAD application registrations and their integrations to ensure continued access and functionality within the new tenant.

### How to perform a tenant-to-tenant migration?

The total amount of services that might require migration is much bigger and can also include Azure services such as Virtual Machines, Database and more. Migration scenarios vary as they depend on the customers` business needs. Though most of scenarios usually consist of the following steps: 

**Step 1. Project planning**

Preparation and planning is an important part of the migration process. This phase should take place two weeks before the actual migration. Scoping identifies potential issues that may occur later on and enables your engineering team to plan for any risks. At this stage it is crucial to choose the right migration strategy, ensure data security and encourage business engagement. 

**Step 2. Preliminary analysis of the source tenant**

At this point you should analyze and map identity objects in the source tenant. Identity objects are users, groups, Teams, and all other objects that need to be migrated. 

**Step 3. Source tenant and target tenant preparation**

Tenant-to-tenant migration means you will have two tenants: the source tenant, from which you are migrating users and data and the target tenant, to which you are migrating. Before performing this type of migration, the primary mail domain should be erased from all objects in the source tenant. At this point it is necessary to ensure you have sufficient space in the target tenant and possibly increase licenses in Target Microsoft 365 organization to guarantee the successful migration from the source tenant. It is important to create Administrator accounts in both tenants. Some migration tools may require more than one admin account in the source tenant to optimize the data throughput. 

**Step 4. Running the pre-migration report before migrating the data**

Before you perform the actual migration, you should run the pre-migration reports to identify Data that can cause problems during data migration and detect Data that requires analysis for migration configuration decisions. 

**Step 5. Validation check and pre-migration testing**

Since data accuracy is a key component in moving data from one tenant to another it is essential to perform migration and data validation testing to ensure all the required data was transferred and verify that there is no data loss. 

**Step 6. Final migration and cutover**

To minimize downtime, bounced emails and user inconvenience, it is important to determine the best method for migration. For migrations with less than 500 users, there can be a cut-off date that can help limit the volume of data migrated, for example, the last 6 months of data.  For migrations with more than 500 users, IT should use a multi-pass approach. A multiple-pass migration is when you migrate older email data before the MX record switchover date, and then run a second pass migration to migrate all Calendars, all Address Books and all Tasks. The users can start functioning on the new target domain while the balance data migration takes place in the background. 

**Step 7. Support**

Once the migration has been completed, it is important to support end users and make sure they have cleared their nickname and auto-completion caches. This is not only for their convenience, but also to prevent them from continuously receiving NDRs when replying to emails that were migrated. 

### How do I get started?

* Learn more about our [Migration services](https://o365hq.com/search?search=migration). 

* Send an email to: sales@itpartner365.com or call our Sales line: +1-844-611-6871 (toll-free). 

* Summarize all the important information about your project with our engineers and sign a Statement of Work. 

* Achieve all the success criteria of the project and close it. 

Migrating Microsoft 365 data during a merger or acquisition can be a challenging task. With [IT Partner](https://o365hq.com/about), you can be sure that the migration process is always secure and goes smoothly.  

IT Partner has migrated [hundreds of organizations](https://o365hq.com/portfolio/ielo-design-pte-ltd/), and our team would be happy to provide you with great support services.