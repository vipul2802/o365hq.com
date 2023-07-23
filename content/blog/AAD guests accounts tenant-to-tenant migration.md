+++
title = "AAD guests accounts tenant-to-tenant migration"
description = "AAD (Azure Active Directory) guest accounts tenant-to-tenant migration refers to the process of migrating guest user accounts from one Azure AD tenant to another."
date = 2023-07-10

[taxonomies]
tags = ["microsoft 365", "Office 365", "migration", "azure ad"]
+++

### Introduction

AAD (Azure Active Directory) guest accounts are user accounts that are created in one tenant but are invited to access resources in another tenant. When a guest user account is created, a copy of the user's identity information is stored in the host tenant's directory as a guest user object. This allows the guest user to authenticate and access resources in the host tenant. AAD guests accounts tenant-to-tenant migration can be necessary when an organization undergoes a merger or acquisition, or when resources need to be consolidated into a single tenant for administrative or security reasons.

### Prerequisites   

Before performing a tenant-to-tenant migration for AAD guest accounts, there are several prerequisites that need to be met: 

1. The administrator performing the migration must have Global Administrator permissions in both the source and destination tenants. 
2. The source and destination tenants must have a trust relationship set up between them. 
3. The guest user accounts being migrated must be represented by an external email address. 
4. The email addresses of the migrated guest accounts must be unique in the destination tenant. 
5. Any existing user accounts with the same email addresses as the migrated guest accounts in the destination tenant must be deleted or renamed before the migration. 
6. All relevant Azure AD settings, such as conditional access policies and application assignments, must be configured identically in both the source and destination tenants before the migration. 
7. Any custom attributes or claims used in the source tenant must be created in the destination tenant before the migration. 

It is important to carefully review and ensure that all prerequisites are met before starting the migration to avoid any issues or data loss during the process. 

### Migration process 

**Preparation**. Ensure that both the source and destination tenants are ready for the migration. 

**Export**. Extract the relevant account information from the source tenant using either the Microsoft Graph API or Azure AD PowerShell cmdlets. Clean up the extracted data and format the email addresses correctly. 

**Migration**. Import the cleaned-up data into the destination tenant using Azure AD PowerShell cmdlets. Create new guest accounts in the new tenant and reassign any necessary permissions or roles.
 
**Verification**. Perform thorough testing to ensure that the migrated guest accounts are properly configured and accessible. Notify the guest users that their accounts have been successfully migrated and provide them with instructions on how to access resources in the new tenant. 

It is important to note that the migration process may take some time depending on the number of guest accounts being migrated and the complexity of the associated metadata. Additionally, it is recommended to perform a test migration before migrating all guest accounts to ensure that the process works as expected and identify any potential issues. 

### Challenges and common issues 

When migrating guest accounts from one Azure Active Directory (AAD) tenant to another, there are several challenges and common issues that organizations may face: 

* When moving guest accounts from one AAD tenant to another, authentication and authorization can be a major challenge. This is because the guest account's identity must be verified in both the source and target tenants, which can be complex and time-consuming. 
* Migration of guest accounts can cause a disruption in user experience, especially if the guest account is used for accessing resources or applications in the source tenant. Migrating guest accounts should be performed in a way that minimizes disruption to the user experience. 
* Guest accounts typically have access to certain resources and applications in the source tenant. When migrating guest accounts, it is essential to ensure that access and permissions are properly set up in the target tenant. 
* If the source and target tenants are not in the same Azure AD Connect configuration, directory synchronization can be challenging. This can cause issues such as duplicate accounts, inconsistent attributes, and synchronization errors. 
* If the guest account is integrated with third-party applications, migrating the account can cause disruption to the integration. It is important to ensure that all integrations are properly configured in the target tenant. 

Overall, migrating guest accounts between AAD tenants can be complex and challenging. It's important to note that some limitations may apply to migrating AAD guest accounts between tenants, such as limitations on migrating certain types of guest accounts, or restrictions on migrating guest accounts that have been granted access to certain types of resources. It's recommended to thoroughly review the documentation and seek assistance from Microsoft Partner to ensure a successful migration. 


