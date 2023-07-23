+++
title = "Microsoft 365 Data Protection"
description = "During the past few years, our traditional workplace has irrevocably changed to more flexible hybrid working environment, with organizations having been forced to adapt to the modern business approach. Companies must ensure that all the sensitive data is secure and protected, especially now when millions of employees work from home."
date = 2022-05-10

[taxonomies]
tags = ["modern security", "microsoft 365", "cloud security", "data protection"]
+++

The key principles of data protection are to keep data safe and make it available under all circumstances, using two main data protection strategies: data availability and data management.

#### Data availability

Given the complex nature of cloud computing, Microsoft is mindful that it's not a case of if things will go wrong, but rather when. Microsoft has worked hard to keep up with the customers` changing needs to design cloud services that maximize reliability and minimize the negative effects on businesses if things do go wrong. There is no traditional strategy of relying on complex physical infrastructure, and redundancy is built directly into the cloud services. A combination of less complex physical infrastructure is used to build data resiliency into Microsoft services as well as to deliver high availability to customers.

Based on this, Microsoft Cloud Services architecture provides a redundant environment which can only be disrupted in the event of Armageddon therefore customers expect continuous innovation from Microsoft without compromising quality, and this is one of the reasons why Microsoft's services and software are built with resiliency and recoverability in mind. Resilience refers to the ability of cloud-based service to withstand certain types of failures and yet remain fully functional from the customers’ perspective. In that sense, Microsoft 365 services are designed based on the following core principles:

**Critical and non-critical data**.     
Non-critical data can be dropped in rare failure scenarios. Critical data must be protected at extreme cost. As a design objective, delivered mail messages are always critical, and things like whether a message has been read is non-critical.

**Data backups and archiving**.     
Copies of customer data must be segregated into different fault zones or as many fault sites as possible, such as datacenters, accessible by single credentials to provide failure isolation.

**Monitoring**.     
Critical data must be monitored for failing any part of Atomicity, Consistency, Isolation, Durability (ACID model).

**Data corruption**.     
Customer data must be protected from corruption or accident deletion. In this case snapshots can be used to set things right.

Through the building of the cloud service to the principles above surrounding this with robust testing and validation, Microsoft 365 can deliver and exceed the requirements of customers.

#### Data damage or accident deletion

Microsoft 365 is the most popular productivity application suite that allows you to easily share and collaborate with stakeholders on everything from crucial business and operational documents to daily emails and files. With a huge volume of information moving around on Microsoft 365, what happens if you delete data by accident? Can you recover it if it’s beyond the retention period? Long story short – YES. Microsoft 365 data handling standard policy provides the following instances of customer data deletion:

**Active deletion** when your tenant has active subscription and an administrator, or a user deletes the data or in some cases a user is deleted by an administrator. 

**Passive deletion** when your subscription is expired. 

By implementing the right data retention policy alongside Microsoft 365 Protection Center or the audit log report you can always check whether the item was moved or deleted. If many of your OneDrive or SharePoint files were deleted, overwritten, corrupted, or infected by malware, you can simply restore your entire OneDrive to a previous time.  

Microsoft provides a few options on how to rescue your data effortlessly within a couple of clicks. Alternatively, you can always outsource such activities to [IT Partner Team](https://www.microsoft.com/en-us/microsoft-teams/microsoft-teams-phone) and our experts will handle this up to the highest standard. 

#### Data retention

Even though Microsoft provides quite commonly used data retention mechanisms, you always have flexibility and can implement your own data retention policy to comply with certain regulations or requirements which require longer periods. 

Data retention policies define what data should be stored or archived, where the data should be kept, and for how long. Once the applicable retention period has expired for a particular type of information, it can be deleted or removed to secondary storage, depending on the requirements. These features below help organizations stay compliant and keep their primary storage clean: 

**Microsoft 365 version control**. 

SharePoint is one of the strongest Microsoft 365 features that allows users to track the activity of any item (document, event, task, etc.) and follow the audit trail. Subsequently, it enables quite robust versioning feature to help you with your daily routine. Any time you change a document in a document library or edit any list time – a new version is created. Each change is recorded, whether it is a physical change to the document or just a metadata change.  

Below is an example how it looks in practice. 

![Microsoft 365 Data Protection](/img/m365DP1.png)

Versioning is usually enabled by default in a document library and you can provide additional services as required. The major benefits of versioning are: 

* Ability to audit the history of an item.
* Ability to track metadata changes.
* Ability to track content changes.
* Ability to restore previous versions.
* Ability to compare SharePoint versions.

**Data Backups**. 

Microsoft offers several protections against corruption, deletion, and disaster scenarios, which can be enhanced further using features such as retention policies and litigation hold. You can also use third-party solutions to protect data against common issues like file corruption and everyday human error.  

![Microsoft 365 Data Protection](/img/m365DP2.png)

**Litigation hold**. 

You can place a mailbox on Litigation hold to retain all mailbox content, including deleted items and the original versions of modified items. When creating a litigation hold, you can simply define a hold duration, or you can just retain content until the Litigation hold is removed. 

To place a mailbox on hold, you can follow these steps below: 

1. Go to the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home?ref=users) and then click **Users** > **Active users**. 
2. Select the user that you want to place on Litigation hold. 
3. On the properties flyout page, click the **Mail** tab, and then under **More actions**, click **Manage          litigation hold**. 
4. On the **Manage litigation hold** flyout page, select the **Turn on litigation hold** checkbox. 

![Microsoft 365 Data Protection](/img/m365DP3.png)

Microsoft provides a versatile facility out of the box which in most cases is super easy to implement and start using if you have a defined requirement. Microsoft 365 data protection solutions will help you minimize downtime, boost productivity, and stay compliant with the ability to quickly recover lost data.