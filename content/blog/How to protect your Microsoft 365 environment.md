+++
title = "How to protect your Microsoft 365 environment"
description = "Microsoft 365 is a complete solution for businesses that brings together Office 365, Windows 10, and Enterprise Mobility + Security (EMS). Securing Microsoft 365 has become crucial, especially as rates of cyberattacks targeting enterprise cloud platforms are increasing each day."
date = 2022-02-02

[taxonomies]
tags = ["microsoft 365", "security", "tenant security", "security links", "modern security", "cloud security", "advanced threat protection"]
+++

With Covid-2019 businesses are forced to rapidly adopt modern technologies to implement an entirely new working environment and support remote employees. By investing in security, you ensure your organization has a safe and productive remote workforce in a Microsoft 365 environment. 

We recommend that you start with these **10 ESSENTIAL QUICK STEPS** to help you protect your own Microsoft 365 environment:

### Step 1. Enable Security Defaults

[MFA](https://docs.microsoft.com/en-us/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication?view=o365-worldwide) is a valuable tool for slowing down attackers. It is also called 2-step verification and it requires a code from your phone to get access to Microsoft 365 when you log in. MFA is easy to set up and at the same time it is one of the most effective ways to increase the security of your organization. To set up multifactor authentication, you turn on Security defaults: 

1. Sign in to the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home)
   with global admin credentials. 
2. In the left nav choose **Show All** and under **Admin centers**, choose **Azure Active Directory**.
3. In the **Azure Active Directory admin center** choose **Azure Active Directory**>**Properties**.
4. At the bottom of the page, choose **Manage Security defaults**.
5. Choose **Yes** to enable security defaults or **No** to disable security defaults, and then 
   choose **Save**.

### Step 2. Implement Internal Trainings 

It is important to establish high security awareness in your organization to prevent modern cyberattacks. Make sure all your users, including security professionals, understand the new environment after you have moved it to the cloud. There are several actions your staff should take to prevent various phishing attacks: 

* Enable security features. 
* Use a strong password. 
* Protect devices. 

### Step 3. Enforce Multifactor Authentication

It is also recommended to enable per-user Azure AD Multi-Factor Authentication to secure sign-in events and better protect your users. All users always start out *Disabled*. When you enroll users in per-user Azure AD Multi-Factor Authentication, their state changes to *Enabled*. When enabled users sign in and complete the registration process, their state changes to *Enforced*. Administrators may move users between states, including from *Enforced* to *Enabled* or *Disabled*. With Zero Trust policies, you can require that users log in to certain applications with specific types of multifactor authentication (MFA) methods. Microsoft 365 admins can easily enforce MFA for all users and keep secure anyone sharing their Microsoft 365 business subscription. 

To enforce MFA across all your Microsoft 365 accounts: 

1. Sign in to your [Microsoft 365 admin account](https://portal.azure.com/#home).
2. Choose **Azure AD Security**. 
3. In the left nav choose **Conditional Access**.
4. Choose **New Policy** and name your policy, for example, **Enforce MFA**.
5. In the **Assignment Section** choose **Users and groups**>**New**  
6. Choose **All users** and **Done** if you want to enforce MFA across your entire organization.

### Step 4. Check Office 365 Secure Score

Office 365 Secure Score analyzes your organization's security based on your regular activities and security settings and assigns a score. Taking notes of your current score and adjusting some tenant-wide settings will increase your score. The goal is to be aware of the capabilities to secure your environment that do not negatively affect productivity for your users. Check [Microsoft Secure Score](https://learn.microsoft.com/en-us/microsoft-365/security/defender/microsoft-secure-score?view=o365-worldwide) for more information.

### Step 5. Use dedicated admin accounts

The administrative accounts are the top targets for hackers and cybercriminals as they include a lot of sensitive data and elevated privileges. The admin accounts should be created only for administrative purposes and should be used only when performing tasks associated with their job function. 

### Step 6. Use a highly secure Windows device for admin accounts 

Microsoft works closely with OEM partners to help them build Secured-core PCs to ensure enhanced security for devices, identities and information. Secured-core PCs provide advanced protection against sophisticated attacks. 

Windows in S mode offers an additional layer of security with flexibility. S mode is a configuration that’s available on all Windows editions. This comes with some cost in terms of compatibility, but Intune also allows customers to install applications on an S mode system, while maintaining the S mode protections against running non-trusted applications. 

### Step 7. Enable Azure Active Directory Identity Protection 

The number of attacks on the identity systems is increasing each day. Leveraging a dedicated backup solution for your Microsoft 365 environment will allow you to reduce costs by moving data to Azure. Enabled Identity Protection discovers various risks, including anonymous IP address use, atypical travel, malware linked IP address, unfamiliar sign-in properties, leaked credentials, password spray and more. 

With AAD Identity Protection tool you can successfully accomplish these three key tasks: 

* [Automate the detection and remediation of identity-based risks](https://docs.microsoft.com/en-us/azure/active-directory/identity-protection/howto-identity-protection-configure-risk-policies).
* [Investigate risks](https://docs.microsoft.com/en-us/azure/active-directory/identity-protection/howto-identity-protection-investigate-risk) using data in the portal.
* [Export risk detection data to your SIEM](https://learn.microsoft.com/en-us/azure/sentinel/data-connectors-reference).

[Risk investigation](https://docs.microsoft.com/en-us/azure/active-directory/identity-protection/howto-identity-protection-investigate-risk) allows administrators to review detections and take manual action on them if needed. 

### Step 8. Configure your Microsoft 365 tenant for increased security 

Every day people receive numerous documents, presentations and attachments related to their work, links in emails, or any other activity. The improved [Microsoft 365 Defender portal](https://security.microsoft.com/homepage) brings Defender for Endpoint, Defender for Office 365, Microsoft 365 Defender into one single platform and includes various capabilities that protect your environment based on your organization`s security needs. You should use these recommendations as a starting point: 

#### Create a Safe Attachment Policy

It is usually difficult to define whether an attachment is safe or not by just looking at the email. Creating a safe attachment policy will help you protect files and attachments from malicious attacks. You need to [Connect Microsoft 365 to Microsoft Defender for Cloud Apps](https://docs.microsoft.com/en-us/defender-cloud-apps/connect-office-365) to enable this feature. 

To create a Safe attachment policy, complete the following steps: 

1. Go to [https://protection.office.com](https://protection.office.com) and sign in with your admin account.
2. In the Security & Compliance Center, in the left navigation pane, under **Threat management**, 
   select **Policy**.
3. On the Policy page, select **Safe Attachments**.
4. On the Safe attachments page, apply this protection broadly by selecting the **Turn on ATP for**
   **SharePoint, OneDrive, and Microsoft Teams** check box. 
5. Select + to create a new policy.   
6. Apply the settings in the following table. 
7. After you have reviewed your settings, select **Create this policy** or **Save**, as appropriate. 

For additional information, see [Set up anti-phishing policies in Defender for Office 365](https://docs.microsoft.com/en-us/microsoft-365/security/office-365-security/configure-mdo-anti-phishing-policies?view=o365-worldwide).

#### Use Safe Links Policy

Safe Links can help protect your organization from malicious phishing attacks by providing time-of-click verification of web addresses (URLs) in email messages and Office documents. Protection is defined through Safe Links policies. 

To get to Safe Links, complete the following steps: 

1. Go to [https://protection.office.com](https://protection.office.com) and sign in with your admin   
   account.
2. In the Security & Compliance Center, in the left navigation pane, under **Threat management**, 
   select **Policy**.
3. On the Policy page, select **Safe Links**. 

#### Create an anti-phishing policy

Anti-phishing protection is a part of Microsoft Defender for Office 365. It helps you protect your organization from malicious impersonation-based phishing attacks. If you haven't configured a custom domain yet, you do not need to do this. You should enable targeted anti-phishing protection only if you have configured one or more custom domains for your Microsoft 365 environment. You can get started with this protection by creating a policy to secure your most important users and your custom domain. 

To create an anti-phishing policy in Defender for Office 365, complete the following steps: 

1. Go to [Microsoft 365 Defender portal](https://security.microsoft.com/homepage?tid=4ed6ea8d-6f86-411d-b7e0-37401bdb9b68).
2. Go to **Email & collaboration** >**Policies & rules** > **Threat policies** > **Anti-phishing** in 
   the **Policies** section.
3. On the Anti-phishing page, select + **Create**.
4. Specify the name, description, and settings for your policy as recommended in the chart below.

For more information, see [Learn about anti-phishing policy in Microsoft Defender for Office 365 options](https://docs.microsoft.com/en-us/microsoft-365/security/office-365-security/set-up-anti-phishing-policies?view=o365-worldwide).

#### Configure the default anti-malware policy

Microsoft 365 environment includes protection against malware, but it is also possible to increase this protection by blocking attachments with file types that are commonly used for malware.   

To configure [anti-malware protection](https://docs.microsoft.com/en-us/microsoft-365/security/office-365-security/anti-malware-protection?view=o365-worldwide) settings, complete the following steps: 

1. In the [Microsoft 365 Defender portal](https://security.microsoft.com/homepage), go to **Email &**
   **collaboration** > **Policies & rules** > **Threat policies** > **Anti-malware** in the **Policies** section.
2. On the **Anti-malware** page, double-click on **Default (Default)**. A flyout appears. 
3. Select **Edit protection settings** at the bottom of the flyout. 
4. In the next page, under **Protection settings**, select the checkbox next to **Enable the common**
   **attachments filter**. The file types that are blocked are listed directly below this option. To add or delete file types, select **Customize file types** at the end of the list. 

#### Set up mail flow rules

Ransomware can be hidden inside macros. It is crucial to block file types that could contain ransomware or other malicious URLs and warn your users not to open such files from people they do not know. Creating a mail flow rule can help you protect your users against ransomware. You can also use the mail transport rules to stop auto-forwarding for email.  

Follow these steps below to create a mail transport rule: 

1. Go to the [Exchange admin center](https://outlook.office365.com/ecp/).
2. In the **mail flow** category, select **rules**. 
3. Select +, and then **Create a new rule**. 
4. Select **** at the bottom of the dialog box to see the full set of options. 
5. Apply the settings in the following table for each rule. Leave the rest of the settings at the
   default, unless you want to change them.  

#### Set up Office message Encryption

Included in Microsoft 365, Office message encryption allows organizations to [manage internal and external encrypted emails](https://support.microsoft.com/en-us/office/send-view-and-reply-to-encrypted-messages-in-outlook-for-pc-eaa43495-9bbb-4fca-922a-df90dee51980). Email message encryption enables you to use protection options, such as *Do not Forward*, *Encrypt and Confidential* when sending an email and helps you ensure that only certain intended recipients can view message content. You should consider purchasing these licenses below to implement Office message Encryption (OME): 

*  Office 365 Enterprise E3 / E5, or Microsoft 365 Enterprise E3 / E5, or Microsoft 365
   Business Premium.
*  Azure Information Protection Plan 1 added to the following plans to receive the new 
   Office 365 Message Encryption capabilities: Exchange Online Plan 1, Exchange Online  Plan 2, Office 365 F1, Microsoft 365 Business Basic, Microsoft 365 Business Standard, or Office 365 Enterprise E1. 

![How to protect your Microsoft 365 environment](/img/HTprotect1.png)

### Step 9. Secure and optimize your Teams 

Microsoft Teams is a secure platform that is used by millions of users on a regular basis. So, it is important to configure additional meaningful steps up in Teams protection. Microsoft offers three tiers of protection for data, identities, and devices: 

* Baseline protection.
* Sensitive protection.
* Highly sensitive protection.

Baseline protection includes public and private teams. Public teams can be accessed by anybody in the organization. While private teams can only be discovered and accessed by members of the team.  
Teams for sensitive and highly sensitive protection are only private teams in which sharing is limited and sensitivity labels are used to set policies around guest sharing, device access, and content encryption. 

Learn more about [Security and compliance in Microsoft Teams](https://docs.microsoft.com/en-us/microsoftteams/security-compliance-overview).

### Step 10. Enable Office 365 Information Protection for GDPR 

Microsoft 365 offers a rich set of capabilities to help you achieve compliance with the General Data Protection Regulation (GDPR). The General Data Protection Regulation (GDPR) introduces new rules for organizations that offer goods and services to people in the European Union (EU), or that collect and analyze data for EU residents no matter where you or your enterprise is located. A [Recommended action plan for GDPR](https://docs.microsoft.com/en-us/compliance/regulatory/gdpr-action-plan) and [Accountability Readiness Checklists](https://docs.microsoft.com/en-us/compliance/regulatory/gdpr-arc) provide additional resources for assessing and implementing GDPR compliance. 

![How to protect your Microsoft 365 environment](/img/HTprotect2.png)

### Advanced protection capabilities to increase security in your business 

These enhanced security features will help your organization improve its cyber-attack prevention. These tasks take a bit more time to plan and implement but they greatly increase your security posture: 

#### Microsoft Compliance Manager.

[Compliance Manager](https://docs.microsoft.com/en-us/microsoft-365/compliance/compliance-manager?view=o365-worldwide) is available to organizations with Office 365 and Microsoft 365 licenses, and to US Government Community Cloud (GCC) Moderate, GCC High, and Department of Defense (DoD) customers. It helps organizations test and monitor compliance activities as well as simplify compliance and reduce risk. The Compliance Manager dashboard reflects your current compliance score and guides you to key improvement actions. 

#### Attack simulation training.

Attack stimulations test your organization`s security policies and train your employees to increase their awareness and reduce cyberattack vulnerability. These simulated attacks can help you identify high-risk users before a real attack affects your bottom line. 

There are multiple types of social engineering techniques available in Attack simulation training:

* Credential harvest. 
* Malware attachment. 
* Link in attachment. 
* Link to malware. 
* Drive-by-URL. 

[To launch a simulated phishing attack](https://docs.microsoft.com/en-us/microsoft-365/security/office-365-security/attack-simulation-training?view=o365-worldwide) do the following steps: 

1. In the Microsoft 365 Defender portal at 
   [https://security.microsoft.com](https://security.microsoft.com), go to **Email & collaboration** > **Attack simulation training** > **Simulations** tab.
2. To go directly to the Simulations tab, use
   [https://security.microsoft.com/attacksimulator?viewid=simulations](https://security.microsoft.com/attacksimulator?viewid=simulations).
3. On the **Simulations** tab, select **Launch a simulation** icon. 

![How to protect your Microsoft 365 environment](/img/HTprotect3.png)

It is crucial to configure advanced protections for admin accounts because once attackers compromise a device, they can impersonate or steal credentials for all accounts that use it, undermining many or all other security assurances. 

We recommend that you start with these enhanced security features: 

#### Privileged Access Workstations (PAWs) for admin activity. 

The [PAW](https://docs.microsoft.com/en-us/security/compass/privileged-access-devices) is the highest security configuration designed for extremely sensitive roles in organizations. The PAW configuration includes security controls and policies that restrict local administrative access and productivity tools to minimize the attack surface to only what is absolutely required for performing sensitive job tasks. It blocks the most common vector for phishing attacks: email and web browsing. The workstation uses credential guard, device guard, app guard, and exploit guard to protect the host from malicious behavior. 

#### Azure AD Privileged Identity Management.

[Privileged Identity Management (PIM)](https://docs.microsoft.com/en-us/azure/active-directory/privileged-identity-management/pim-configure) helps you manage and monitor access to important resources in your organization. PIM offers time-based and approval-based role activation to mitigate the risks of excessive, unnecessary, or misused access permissions on resources that you care about. 

![How to protect your Microsoft 365 environment](/img/HTprotect4.png)

Understanding the capabilities of your Microsoft 365 platform can be a challenging and time-consuming task to achieve. Adoption of Microsoft 365 will allow your organization to keep confidential and personal data safe and secure. [IT Partner Team](https://o365hq.com/about) is always ready to discuss your business needs and help you strengthen your IT security. Check our services below and [contact us](https://o365hq.com/contacts) today. Our cloud services experts will do their best to help you get the most out of your Microsoft 365 environment. 

<iframe src="https://onedrive.live.com/embed?cid=6BBFDD038E0969FD&resid=6BBFDD038E0969FD%215892&authkey=ACIe4fBLrqm7c4g&em=2" width="100%" height="600px" frameborder="0" scrolling="no"></iframe>
