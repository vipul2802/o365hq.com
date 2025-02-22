+++
title = "Microsoft 365 Tenant-to-Tenant Cutover Email Migration Without Downtime and Bounced Email"
description = "Mailbox migration from one Microsoft 365 tenant to another. Usually, you will need this type of migration when a company merges or acquires another company, or you would like to migrate to a different geographic region. This service is an advanced migration with additional service that avoids bounced emails, NDR, or any downtime for incoming email."
date = 2019-06-03

[taxonomies]
products = ["Office 365", "microsoft 365"]
types = ["Migration"]

[extra]
sku = "ITPWW380MIGOT"
price = "$1,400 + $25 per mailbox"
duration = "1 week"
manager = "Roman Sotnik"
+++

Occasionally, a customer needs a migration inside the Microsoft 365 cloud
platform. For example, if one company acquires another company and both
are using Microsoft 365, there may be many reasons to start merging. 

Our objective is to provide planning, design, and migration of email
service from one Microsoft 365 tenant to another. 

This service is an **advanced migration** with additional service that
 **avoids bounced emails, NDR, or any downtime**
for incoming mail. During domain transferring between tenants, there may
be delays in mail receipt for about 3-5 minutes, which depends on the
volume of incoming emails.

If short-term downtime and the possibility of losing some emails is
acceptable to you, please see another service we offer, Microsoft 365
Tenant-to-Tenant Cutover Email Migration

### IT Partner responsibilities

1.  Export resources (mailbox-enabled users, contacts, groups, etc.)
    from the source tenant
2.  Import resources to the destination tenant via AD Connect
    or CSV import
3.  Do pre-stage migration (only emails and email folders older than 30
    days)
4.  Proxy services setup, which allows receiving all incoming emails
    during a domain transfer
5.  Final mailbox migration with calendars, contacts, rules, and other
    data
6.  Change records in domain zones to accommodate migration needs

### Client responsibilities

1.  Provide a dedicated point of contact responsible for working with IT
    Partner
2.  Coordinate any outside vendor resources and schedules
3.  Configure all network equipment, such as load balancers, routers,
    firewalls, and switches
4.  If Microsoft Outlook or other desktop email clients are used to
    connect to Microsoft 365, deploy email software on client workstations
5.  Perform changes to internal and external DNS, as required
6.  Assist with identification of high-risk users (top executives
    and VIP users, users with 50 GB mailboxes or larger and/or
    30 GB deleted folders or larger)
7.  Recreate new Outlook profile on all client workstations, if desktop
    version of Outlook is used
8.  Inform users about upcoming changes and provide the necessary
    information

### Additional cost items not provided by the project

1.  Informing users about upcoming changes
2.  Customer team training (could be added as an additional service)
3.  Migration of corporate documents to SharePoint Online (could be
    added as an additional service)
4.  Desktop software settings

Upon completion of the project, we will provide a project closeout
report. This document will indicate the final project status, including
evidence of matching acceptance criteria, outstanding issues, if any, and the
final budget. If you require more extensive documentation, it can be
provided for an additional fee.  

### Prerequisites

1.  You must have global admin level access to the source Microsoft 365
    tenant
2.  You must have global admin level access to the destination Microsoft
    365 tenant, with Exchange Online licenses available
3.  You must have access to your email domain DNS zone

### Plan

The plan may vary depending on your needs.

1.  Kickoff meeting
2.  Pre-migration source system health check
3.  Creating users or configuring AD Connect tool
4.  Email migration start
5.  Verification of email migration
6.  Changing MX record to new Microsoft 365 tenant
7.  Final email migration
8.  Post-migration tasks

### Success criteria

1.  Users can access Exchange Online on their desktop PCs, mobile phones,
    and tablets from any place, any time
2.  Old Microsoft 365 tenant successfully migrated to new Microsoft 365 tenant
    and is accessible by all users
3.  All necessary Transport rules are created and working
4.  Mail can be sent and received using Exchange Online
5.  Exchange Online Protection is configured and working
6.  No incoming message loss during the migration process
