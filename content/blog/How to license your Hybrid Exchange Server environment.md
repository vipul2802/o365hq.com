+++
title = "How to license your Hybrid Exchange Server environment"
description = "Hybrid enables rich co-existence between your on-premises Exchange server and Microsoft 365 / Exchange Online in the cloud. A hybrid deployment combines an on-premises Exchange organization and Exchange Online to create one single Exchange organization and can serve as a next step to moving completely to an Exchange Online organization in the future."
date = 2022-11-30

[taxonomies]
tags = ["microsoft 365", "office 365", "howto", "exchange server"]
+++

To successfully configure your hybrid environment, you need to know how to properly license your on-premises server used for hybrid. If you have an Exchange Server 2010, 2013, 2016, or 2019, then you should have everything you need and there is no need to license Hybrid Servers. The process of acquiring an Exchange Hybrid license has changed. Previously, you would use Microsoft's self-service site to validate your Microsoft 365 tenant and get the key to license your on-premises server used for hybrid purposes. But Microsoft has recently presented a feature that allows the Hybrid Configuration Wizard (HCW) to detect and license your designated on-premises “hybrid server”. Since April 2022, HCW also provides a 'hybrid key' for Exchange Server 2019. Remember that for Exchange Server 2019, you need Exchange Server 2019 CU12 or higher. Otherwise, the Exchange Hybrid license will not be downloaded. 

![How to license your Hybrid Exchange Server environment](/img/ExSrv1.png)

### When do I need a Hybrid license? 

Sometimes organizations that have recently migrated to Microsoft 365 discover the need to install at least one Exchange Hybrid Server and employ the free Hybrid license. There are several scenarios when you may consider utilizing a hybrid exchange license: 

1.  If you have Exchange Server 2003 or 2007 and require a part-migration to a newer version of Exchange Server.
To complete your Hybrid migration to Microsoft 365, you will need to add Exchange 2010 or 2013 servers to implement co-existence with the newer version and utilize a free Exchange Hybrid license for Exchange Server. 

2.  After the migration from Exchange Server 2010 to Microsoft 365.
Once the migration has been completed, you may want to decommission your Exchange Server 2010. When you move all the mailboxes to Exchange Online – Microsoft 365, and you have an Active Directory on-premises, you may need to install Exchange Hybrid servers for attribute management within your local AD. To manage hybrid identity and the attributes, you will require an Exchange 2016 server or higher.  

3.  If you want to have a local Autodiscover service in Exchange Server.
The Autodiscover service minimizes user configuration and deployment steps by providing clients access to Exchange features. For Exchange Web Services (EWS) clients, Autodiscover is typically used to find the EWS endpoint URL. Autodiscover makes it easy to retrieve the information that you need to connect to mailboxes on Exchange servers. To deploy Autodiscover, we strongly recommend you install an Exchange 2016 server and higher. 

### What are the steps to acquire the Exchange Hybrid license? 

**1. Download and access the Hybrid Configuration Wizard (HCW).**

Now to license your new Exchange Servers for Hybrid, you will use Office 365 Hybrid Wizard. HCW was released to simplify the configuration of hybrid deployment, and guarantee you are always running the most up-to-date versions of the experience. You can download Hybrid Configuration Wizard (HCW) from the following link: [https://aka.ms/HybridWizard](https://aka.ms/HybridWizard).

**2. Run the HCW and apply the license to the appropriate Exchange Hybrid server.**

When you run the wizard and choose the “Detect the optimal Exchange server” option, HCW will allow you to use the “license this server now” option, if the server is currently not licensed. 

![How to license your Hybrid Exchange Server environment](/img/ExSrv2.png)

**3. Verify the license and make sure you have successfully licensed the Exchange Hybrid server.**

When you select the “license this server now” link, you will need to confirm your online administrator credentials to validate and obtain the key. Once HCW applies the server license to your on-premises server, you will get confirmation that the server has been licensed. It is also possible to copy the product key and the CMDlet needed to use it. 

![How to license your Hybrid Exchange Server environment](/img/ExSrv3.png)

To check that your Exchange Hybrid server has been properly licensed, sign in to **Exchange admin center -> servers -> Exchange Hybrid server -> Hybrid Deployment Licensed.**

### Hybrid Exchange License FAQs

**1. Which versions of Exchange support the new Hybrid Configuration wizard?**

To remain in a supported hybrid configuration, you need to make sure you are running the latest available released CU for your Exchange version. You can use a combination of one or more of the following versions of Exchange: 

* Exchange 2010 SP3. 
* Exchange 2013 CU1 or later. 
* Exchange 2016 and Exchange 2019. 

**2. What if I have Exchange Server 2003 or 2007?**

If you are running Exchange Server 2003 or 2007, you would need to deploy at least one server running Exchange 2013 that meets the requirements above to qualify for a “free” Exchange Hybrid license.

**3. If my organization is Hybrid with Microsoft 365, do I still need to license Exchange Server?**

If you do not host any mailboxes on-premises, you can license them using the Microsoft 365 Hybrid Configuration Wizard (HCW). The HCW will validate your Microsoft 365 subscription and install the appropriate licenses on your servers. 