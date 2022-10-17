+++
title = "How to delete former employees` Microsoft 365 accounts and properly preserve their mailbox data"
description = "Employees resign from time to time, often leaving behind a great amount of information in their email correspondence. To ensure productivity and avoid workplace disruption, an organization should effectively manage new emails that keep arriving in the former employees` mailboxes as well as consider archiving the data."
date = 2022-10-14

[taxonomies]
tags = ["microsoft 365", "howto"]
+++

One of the questions that businesses have to face when employees leave the organization is what to do with their mailboxes: how to keep the data secure and block their access to Microsoft 365. In this case, companies should consider certain steps such as access control, data preservation or removal and informing other employees and partners about the upcoming changes in order to protect the organization's data. 

When employees resign, you will need to remove them from Microsoft 365 for business. First, you should block them from accessing company files, preserve the documents they created, and complete several other admin tasks associated with removing a user. 

We recommend that you complete these steps below to secure the organization's data, and at the same time allow other employees to access email and OneDrive data. 

1.  Block access to Microsoft 365 and employees’ mobile devices. 
2.  Either set up an OOF Email Autoresponder OR set up an email forwarding OR move the user’s email address(es) to a different user as an email alias(es) to preserve the mail flow. 
3.  Archive the mailbox. 
4.  [Give another employee access to OneDrive and Outlook data](https://learn.microsoft.com/en-us/microsoft-365/admin/add-users/remove-former-employee-step-5?view=o365-worldwide).
5.  [Remove and delete the Microsoft 365 license from a former employee](https://learn.microsoft.com/en-us/microsoft-365/admin/add-users/remove-former-employee-step-6?view=o365-worldwide).
6.  [Delete a former employee's user account](https://learn.microsoft.com/en-us/microsoft-365/admin/add-users/remove-former-employee-step-7?view=o365-worldwide).

![How to delete former employees` Microsoft 365 accounts and properly preserve their mailbox data](/img/HTdelete1.png)

### What is the proper way of preserving mailbox data? 

Once you decide you really need to preserve the mailbox data, there are certain factors you will have to examine. The first step is to identify if the user has archived data. Another factor you must consider is whether the mailbox should continue receiving new email messages or you can just stop the mail flow. You will also need to inform senders about the user`s departure especially if the employee was engaged in an important business project. It is also necessary to decide if you should keep the user account together with all files saved in OneDrive for Business, or you can just remove everything. Taking all these factors into consideration, we recommend that you choose one of these options below: 

### Option 1. Use shared mailboxes

Converting a mailbox to a shared one is the most common and recommended approach for companies that want to take over the responsibility for the work of a departed staff member. 

To perform the User -> Shared mailbox conversion, first you must properly disable access to the mailbox. And only after this step has been completed, you can perform the conversion to shared mailbox and reclaim the license. 

Transforming a user`s mailbox to a shared one has several advantages: 

* There is no need to forward the email to an appropriate person. Every user assigned to the shared mailbox has full access to it. 
* Possibility to share Outlook calendar information. 
* You can always convert the shared mailbox to a regular one.  

To use a shared mailbox, the mailbox must have a license assigned to it. Once a user mailbox becomes shared, it no longer needs an Exchange Online license unless it is larger than 50 GB or has an archive. 

**To convert the mailbox of a departed employee to a shared one**, follow these steps below: 

1. Recover the deleted account and make sure it has an assigned Microsoft 365 license.
2. Reset the password and check if the mailbox has been created again.
3. Convert it to a shared mailbox and delete the license from the user mailbox.
4. Start adding members.

Admins can now convert a cloud-based user mailbox to a shared mailbox with a single click in the Exchange Admin Center (EAC). No need to use PowerShell anymore. A cloud-based shared mailbox can be converted to user mailbox with a single click, as well. 

![How to delete former employees` Microsoft 365 accounts and properly preserve their mailbox data](/img/HTdelete2.png)

### Option 2. Create and manage inactive mailboxes 

To make a mailbox inactive, it must be assigned an Exchange Online Plan 2 license (or an Exchange Online Plan 1 license with an Exchange Online Archiving add-on license) so that a hold can be applied to the mailbox before it is deleted. After the user account is deleted, any Exchange Online license associated with the user account will be available to assign to a new user. 

**Making a mailbox inactive** involves two steps: 

1.  *Put the mailbox on "In-Place Hold" or "Litigation Hold"*. 
Once you complete this step, you will be able to retain all the contents of the mailbox before deleting it. All the deleted and modified items will remain in the inactive mailbox for a certain time, or until you delete the mailbox. 
2.  *Delete the mailbox*. 
If you no longer need to retain the contents of an inactive mailbox, you can permanently delete the inactive mailbox by removing the hold applied to the inactive mailbox. 

Inactive mailboxes let you retain former employees' email after they resign and can be accessed by authorized people who have been granted [eDiscovery permissions](https://learn.microsoft.com/en-us/microsoft-365/compliance/assign-ediscovery-permissions?view=o365-worldwide) for compliance or legal reasons.   

![How to delete former employees` Microsoft 365 accounts and properly preserve their mailbox data](/img/HTdelete3.png)

### Management of inactive mailboxes 

Inactive mailboxes are self-managing and remain in place until the holds expire. Here are some tips you can use to manage your inactive mailboxes: 

* **Search and export the contents of an inactive mailbox**. 
Microsoft Purview compliance portal provides you with the Content Search tool that you can use to [search](https://learn.microsoft.com/en-us/microsoft-365/compliance/content-search?view=o365-worldwide) and [export](https://learn.microsoft.com/en-us/microsoft-365/compliance/export-search-results?view=o365-worldwide) the contents of an inactive mailbox. It is also possible to build a keyword search query if you want to look for specific items or return the entire contents of the inactive mailbox.

* **Change the hold duration for an inactive mailbox**. 
Once a mailbox is made inactive, you can change the duration of the hold applied to the inactive mailbox.

* **Recover an inactive mailbox**. 
You can easily [Recover an inactive mailbox](https://learn.microsoft.com/en-us/microsoft-365/compliance/recover-an-inactive-mailbox?view=o365-worldwide) in case a departed employee returns to the company. When you recover an inactive mailbox, the mailbox is converted to a new mailbox, the contents and folder structure of the inactive mailbox are retained, and the mailbox is linked to a new user account. After it is recovered, the inactive mailbox no longer exists. 

* **Restore the contents of an inactive mailbox to another mailbox**. 
Sometimes a new employee is hired to take on the job responsibilities of a former employee. In this case you can [restore (or merge) the contents of the inactive mailbox](https://learn.microsoft.com/en-us/microsoft-365/compliance/restore-an-inactive-mailbox?view=o365-worldwide) to an existing mailbox and copy the contents to another mailbox. The inactive mailbox remains inactive and can still be searched using eDiscovery, its contents can be restored to another mailbox, or it can be recovered or deleted later. 

* **Delete an inactive mailbox**. 
You can always remove the hold applied and permanently [delete an inactive mailbox](https://learn.microsoft.com/en-us/microsoft-365/compliance/delete-an-inactive-mailbox?view=o365-worldwide) if you do not need to preserve the contents of an inactive mailbox. Once you remove the hold, the mailbox will be retained for 183 days before it becomes non-recoverable. 
<<<<<<< HEAD
 
![How to delete former employees` Microsoft 365 accounts and properly preserve their mailbox data](/img/HTdelete4.png)
=======
  
![How to delete former employees` Microsoft 365 accounts and properly preserve their mailbox data](https://o365hq.com/images/HTdelete4.png)
>>>>>>> 03a6ed3495f83c7b86003f825f0f2e032c9214f2

To summarize, there is no single solution that can fit all your needs although our personal recommendation is to use shared mailboxes as a preferred method or preserving the mailbox data. Our experienced IT Partner team will help you better understand and improve the whole data preservation process. 
