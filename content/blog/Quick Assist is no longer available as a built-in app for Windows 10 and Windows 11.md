+++
title = "Quick Assist is no longer available as a built-in app for Windows 10 and Windows 11"
description = "Since May 16, 2022, the remote support Quick Assist for Windows 10/11 is an app out of support. Microsoft moved Quick Assist to the Store to increase the app's security, reduce application errors and achieve significant improvement in passcode generation times."
date = 2022-10-18

[taxonomies]
tags = ["microsoft 365", "quick assist", "microsoft 365 business apps", "windows 10", "office 365"]
+++

### What is Quick Assist? 

[Quick Assist](https://learn.microsoft.com/en-us/windows/client-management/quick-assist) is a Microsoft app that allows you to share your device with another person over a remote connection. It can remotely connect to a user's device and then view its display, make annotations, or take full control. With Quick Assist, your support team can easily diagnose and troubleshoot technical issues and instruct users directly on their devices. But since April 27, 2022, the remote assistance with Quick Assist has changed, and it will no longer be a built-in tool integrated into Windows 10/11. To keep your remote assistance sessions secure, you must download the new Quick Assist from the [Microsoft Store](https://apps.microsoft.com/store/detail/quick-assist/9P7BP5VNWKX5?hl=en-us&gl=us), which will also be retired in the first quarter of 2023. 

### How to deploy the new Quick Assist tool with Intune? 

Since Quick Assist moved to Microsoft, we have noticed that Windows admins and users are having numerous issues with the new Store version of Quick Assist. For example, installing the new app requires local administrator rights and runs next to the outdated version on Windows machines. We strongly recommend that you follow the steps below to distribute Quick Assist via Intune: 

**Step 1. Install Quick Assist as an [offline version](https://learn.microsoft.com/en-us/microsoft-store/distribute-offline-apps) from the Windows Store for Business**: 

1. From the Quick Assist prompt, select **Open Microsoft Store**. You will be taken to the Microsoft Store to get the latest version. 

2. In Microsoft Store, select **Get**. Then give permission to install Quick Assist. When the installation is complete, you will see **Get** changes to **Open**.

![Quick Assist is no longer available as a built-in app for Windows 10 and Windows 11](/img/QA1.png)

**Step 2. Activate the sync of Intune with the Windows Store for Business**.

Intune can always pull the latest version of quick assist from the store. Follow these steps to add offline apps to Intune:

* Open the [Microsoft Endpoint Manager Admin Center](https://login.microsoftonline.com/organizations/oauth2/v2.0/authorize?redirect_uri=https%3a%2f%2fendpoint.microsoft.com%2fsignin%2findex%2f&response_type=code+id_token&scope=https%3a%2f%2fmanagement.core.windows.net%2f%2fuser_impersonation+openid+email+profile&state=OpenIdConnect.AuthenticationProperties%3dXjcd4Q6EHnBtm8fMiQGBd-8iYfjyuD9KnUUTA8dseDo_KooXVhYp5sQsK9IxglMqqePqscB5EUkK7c3vSwltvpUOvMDXY8rkehEDPQYEwOBOywPpvH5Lzy-ZosbkGUyWNSmsKtl35uS_uDy5Jq0YJPuS0cC6NOcziO2v4ue6lmza91Tc1ufG1MlXwh90iB-WX0WUsVy9LMzK70KUUobV1aKJli1tq2xhO-faRUGUxc2GdCPTzQCHKUlrgUdhxkXFGtzxRrF_ndSbqhEJWvUpmtSGo54zKWe3mHJQNLIZgFeK9UffuiyFY-6gl5Ix4saMiPVtm5CrmW0pZ0IIFXE2GvJcViZvBzkJIiDDJrxCuDGAT5J3KoHSFr0WI7JbOMfYcCIVaQoo1kbmOfBv_u3EYg&response_mode=form_post&nonce=638016826921346637.YmFiNzllMjItNjJjOC00NjY2LTlmOTItZTE5NjY1ODdmZTRlY2VmNzc3ZDEtOGQzYi00MTkyLWI1ZTQtMWE5MmY2ODQzYjNh&client_id=c44b4083-3bb0-49c1-b47d-974e53cbdf3c&site_id=501430&client-request-id=6ec29551-aeb6-4f5c-ab44-879f6961bf56&x-client-SKU=ID_NET472&x-client-ver=6.22.1.0&sso_nonce=AwABAAEAAAACAOz_BAD0_9vPQi0lwMiL_9tZnUwIe6Q7dgItdWrDwTDvk7Zpeb_RO3PcBqW_WaCj4L0rekdmiJ37GnK2t4tlFJa_5tXgT8MgAA&mscrid=6ec29551-aeb6-4f5c-ab44-879f6961bf56). 
* Go to **Tenant administration** -> **Connectors and tokens** -> **Microsoft Store for Business**. 
* Enable **"Microsoft Store for Business sync"**. 
* Open [Microsoft Store for Business](https://businessstore.microsoft.com/en-us/store?signin=) and navigate to **Manage** -> **Settings** to ensure **offline apps** are activated. 
* Go to **Distribution** to activate Microsoft **Intune** and **Microsoft Intune Enrollment**. If necessary, click **+ Add management tool**. 

![Quick Assist is no longer available as a built-in app for Windows 10 and Windows 11](/img/QA2.png)

![Quick Assist is no longer available as a built-in app for Windows 10 and Windows 11](/img/QA3.png)

**Step 3. Add and deploy Quick assist as an offline app via Intune**. 

* Find Quick Assist in the Windows Store for Business and choose the Offline app. 
* Go to **Intune** and click **Sync** in the WSfB connector to speed up the process and wait until you see the **Quick Assist (Offline)** in the App list. 
* To add an assignment to the app, go to **Quick Assist (Offline)** -> **Properties** -> **Edit**, click **+ Add group** and select a group.  

![Quick Assist is no longer available as a built-in app for Windows 10 and Windows 11](/img/QA4.png)

![Quick Assist is no longer available as a built-in app for Windows 10 and Windows 11](/img/QA5.png)

![Quick Assist is no longer available as a built-in app for Windows 10 and Windows 11](/img/QA6.png)

**Step 4. Install WebView2 via Intune**.

Once you install Quick Assist you may need to install and run WebView2 on your computer. WebView2 is required to run the Store app and helps improve security and performance. If you use Windows 11 or the Edge browser, you probably already have WebView2 installed.  

If WebView2 is not already installed, it will be installed automatically the first time you launch Quick Assist. If you see a prompt for WebView2 it could indicate that the initial installation was not successful. Then you should go to the [Microsoft Endpoint Manager admin center](https://endpoint.microsoft.com/) and follow the instructions below: 
 
* Navigate to **Devices** -> **Windows** -> **Configuration profiles** and choose **+ Create profile**. 
* Select **Windows 10 and later platform as Platform** -> **Templates** as Profile type and **Administrative templates** as Template name. 
* Enter **Name** and Navigate to **Computer Configuration/Microsoft Edge Update/Microsoft Edge WebView** -> **Allow installation (2.0)** -> **Always allow installs**. 
* Choose **Always allow updates (recommended)** as Update Policy and assign the policy to a **group**. 

With these policies applied, WebView2 will be always updated automatically when the latest version is available. 

![Quick Assist is no longer available as a built-in app for Windows 10 and Windows 11](/img/QA7.png)

![Quick Assist is no longer available as a built-in app for Windows 10 and Windows 11](/img/QA9.png)

![Quick Assist is no longer available as a built-in app for Windows 10 and Windows 11](/img/QA10.png)

![Quick Assist is no longer available as a built-in app for Windows 10 and Windows 11](/img/QA11.png)

Quick Assist is a great product that helps IT teams view a remote Windows device over internet connection to troubleshoot technical issues and provide instructions to fix them. There remain some installation issues, but fortunately, Microsoft is aware of them and constantly working to resolve them. In the meantime, we strongly recommend that you download and use the offline version of Quick Assist and avoid using the keyboard shortcut to launch the app. 