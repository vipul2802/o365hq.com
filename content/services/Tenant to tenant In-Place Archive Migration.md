+++
title = "Tenant to tenant In-Place Archive Migration"
description = "Service built to help companies transfer mailbox data from the In-Place Archive of one Office 365 tenant to another Office 365 tenant while maintaining the metadata and folder hierarchy of the data."
date = 2023-04-11

[taxonomies]
products = ["Office 365", "microsoft 365"]
types = ["Migration"]

[extra]
sku = "ITPWW495MIGOT"
price = "$10 per mailbox"
duration = "7 days"
manager = "Roman Sotnik"
+++

### Description

In-Place Archive is a feature in Microsoft Exchange Online that allows users to store older or less frequently accessed messages in a separate mailbox in the same tenant. However, when organizations merge or undergo other changes, there may be a need to move this data to a different tenant. The migration can be done using a variety of tools, including third-party migration tools, PowerShell scripts, and native Office 365 migration tools. 

While Tenant to tenant In-Place Archive migration process involves using various migration tools, scripts, and services, it is recommended to seek expert assistance or use a reliable migration tool to guarantee a successful migration. Our **goal** is to help you ensure that the migration is done correctly to prevent data loss or corruption.

### IT Partner responsibilities 

1. Plan and prepare for the migration by assessing the environment and setting up the target tenant. 
2. Configure the source and target environments for migration, including setting up the necessary permissions and creating a migration batch. 
3. Monitor the progress of the migration. 
4. Verify that all data has been successfully migrated and perform any necessary post-migration tasks, such as updating DNS records or reconfiguring client devices. 
5. Minimize user intervention during the migration process. 

### Client responsibilities 

1. Provide a dedicated point of contact responsible for working with IT Partner. 
2. Coordinate any outside vendor resources and schedules. 
3. Provide temporary access to the existing environment/IT Infrastructure. 
4. Configure all network equipment, such as load balancers, routers, firewalls, and switches. 
5. Perform changes to internal and external DNS, as required. 
6. Inform users about upcoming changes and provide the necessary information. 

### Additional cost items not provided by the project  

1. Other items not listed in the scope.

### Prerequisites 

1. Verify that the target tenant has a valid Office 365 subscription and the necessary licenses for the users being migrated. 
2. Ensure that the source and target environments are properly configured and that the necessary permissions are granted.  
3. The user accounts and mailboxes in both the source and target tenants must be fully synchronized and there is enough available storage space in the target tenant for the migrated data. 
4. Verify that any custom settings or configurations in the source tenant (such as retention policies or transport rules) are properly set up in the target tenant. 
5. Perform a test migration. 
6. Prepare a migration plan that outlines the steps to be taken during the migration, including any necessary downtime, data backup, and verification procedures. 

### Plan

1. Kickoff meeting.
2. Identify the users whose data will be migrated, map the source and target environments, and set up the target tenant. 
3. Create the necessary migration endpoints, set up administrative accounts, grant the necessary permissions, and create a migration batch. 
4. Start the migration batch and monitor the progress of the migration.  
5. Verify that all data has been successfully migrated to the target tenant.  
6. Follow-up / closure conversations. 

### Success criteria 

1. All In-Place Archive data is successfully migrated from the source tenant to the target tenant, including all messages, folders, and metadata. 
2. There is no data loss or corruption. All migrated data is accessible and usable by the users in the target tenant. 
3. The migration has minimal impact on users in both the source and target tenants. Users can access their email accounts and In-Place Archive data throughout the migration process. 