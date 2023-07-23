+++
title = "Move your RDS deployment to Azure"
description = "Business environment is changing extremely fast and companies are struggling to quickly adjust to new ways of working. And having a workforce that can be accessible anytime from anywhere is becoming increasingly important."
date = 2021-03-29

[taxonomies]
tags = ["windows virtual desktop", "microsoft azure"]
+++

A remote desktop experience to employees is often delivered through Remote Desktop Services (RDS). However, as an on-premises solution, RDS does not realize the full value of modernization or the benefits of a cloud VDI.  

Windows Virtual Desktop not only supports Windows Server but also provides Windows 10 enterprise multi-session, combining the Windows 10 experience with the ability to run multiple concurrent user sessions. It allows you to get an optimized experience for Microsoft 365 Apps including Microsoft Teams and enhanced security for users, company apps, and data. With WVD you can easily enable remote work, save on infrastructure, and reduce the total cost of ownership (TCO). Windows Virtual Desktop also helps bring other benefits to your business, including simplified IT management, security capabilities that help keep your users, data, organization safe and protection against outages with integrated Azure Site Recovery and Azure Backup technologies.  

![Move your RDS deployment to Azure](/img/movetords1.png)

If you have RDS you can consider either moving to an infrastructure as a service (IaaS) approach with Azure or migrate directly to Windows Virtual Desktop. WVD on Azure allows you to migrate your existing virtual workloads to Azure and focus on what`s really important to you, the perceived end user experience.  The migration process involves several steps.

![Move your RDS deployment to Azure](/img/movetords2.png)

### Step 1: Environment Assessment

During the migration, you will need permissions to work with storage and networking components, and of course VMs. You can ensure you have configured your Azure subscription, resource group, project name, and geography within the Azure Portal. With Azure Migrate: Server Migration as the migration tool you can easily start the discovery process and gather a lot of information about your current infrastructure. It is highly recommended that you do this at least once for each RD Session Host server before you migrate it. 

![Move your RDS deployment to Azure](/img/movetords3.png)

### Step 2: Server migration

After you have verified that the test migration works as expected, you can migrate the on-premises RD Session Host servers. By default, Azure Migrate shuts down the on-premises VM and runs an on-demand replication to synchronize any VM changes that occurred since the last replication occurred. You can use the Stop migration option to stop replication for the on-premises machine and remove the machine from the Replicating servers count in Azure Migrate.

![Move your RDS deployment to Azure](/img/movetords4.png)

### Step 3: Windows Virtual Desktop deployment and infrastructure configuration

Once you have migrated to Windows Virtual Desktop, you should investigate the usage and the Windows Virtual Desktop health of your environment to rescale your session host servers as needed. It is also good to monitor that health on an on-going basis. Security is an important part of Windows Virtual Desktop. Now is the right time to consider adding Conditional Access to your deployment. Windows Virtual Desktop can also be leveraged by your administrators by providing secure access to a central management (jump host) server. It is important to plan continuous autoscaling and updates to the session host VMs as part of your host pool. Azure Advisor provides you with information about your Windows Virtual Desktop environment and guides you to best practices you might have missed during your deployment.  

![Move your RDS deployment to Azure](/img/movetords5.png)

### Step 4: RDS deployment cleanup

After you have successfully migrated your RDS deployment to Windows Virtual Desktop, it is advised to also clean up your RDS deployment. It’s important to investigate, plan, and execute this cleanup thoroughly to make sure no components or configurations are left behind. This step involves removing the VMs of your RDS deployment (such as RD Connection Broker, RD Web Access, and RD Gateway), various DNS records and the corresponding AD computer objects. 

The migration from RDS to WVD is designed to be as seamless as possible and gives you the following benefits:
* Windows 10 Enterprise multiple session capabilities.
* Free Windows 7 Extended Security Updates till 2023.
* WVD comes as a Platform-as-a-Service (PaaS) meaning, it is Microsoft which runs the show completely without the need of end-user involvement.




