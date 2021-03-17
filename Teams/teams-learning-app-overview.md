---
title: Install, manage, and assign permissions for the Teams Learning app (private preview)
author: ChuckEdmonson
ms.author: chucked
manager: pamgreenMSFT
ms.date: 
audience: Admin
ms.topic: article
ms.service: msteams
ms.reviewer: ChrisArnoldMSFT, LearningDocs2020
localization_priority: Normal
search.appverid: 
ms.collection: 
description: Use the Microsoft Teams Learning app to create a central hub for learning where employees can share, assign, and learn from content libraries across an organization.
f1.keywords:
appliesto: 
  - Microsoft Teams
ms.custom: 
ROBOTS: NOINDEX, NOFOLLOW
---

# Install, manage, and assign permissions for the Teams Learning app (private preview)

*This article contains preliminary content for the Teams Learning app, which is in private preview.*

The Microsoft Teams Learning app (private preview) empowers teams and individuals in your organization to make learning a natural part of their day. The app creates a central hub in Teams where employees can share, assign, and learn from content libraries across your organization. Admins set permissions and allow learning content sources for the app. Learning content can include LinkedIn Learning, Microsoft Learn, Microsoft 365 training, your organization's own content stored in SharePoint online, and third-party providers that are supported by the app.

To set up the Teams Learning app (private preview), you'll need to involve:

-	Teams admin center admin
-	Microsoft 365 admin center admin (that is, a global admin)

## Manage the Teams Learning app (private preview) in the Teams admin center

The Teams admin installs the Teams Learning app (private preview) from the app store and applies app setup, manage, and permissions policies through the Teams admin center.

### Manage the Teams Learning app (private preview)

To manage settings for app, follow these steps:

1. In the left navigation of the Microsoft Teams admin center, go to **Teams apps** > **Manage apps**.

   ![Left navigation in the Teams admin center showing Teams apps and Manage apps section](media/learning-app-teams-manage-apps-nav.png)

2. On the **Manage apps** page, in the search box, type *learning* to search for the Teams Learning app (private preview).

   ![Manage apps page in the Teams admin center showing the search box](media/learning-app-teams-manage-apps-page.png)

3. On the **Learning** page:
   1. Under **Status**, select **Allowed** to turn on the app.
   2. On the **Settings** tab, in the **App settings** section, go to the Microsoft 365 admin center to configure learning content sources.

   ![Learning page in the Teams admin center showing Status and App settings section](media/learning-app-teams-learning-page.png)

4. After **Manage app** settings, go to **Permissions and Set-up policies** to grant permission to employees who should have access to the app as part of your organization's participation in the private preview.

> [!NOTE]
>  If your organization is in Ring 4.0 as part of Teams TAP100 program, you might need to do the following to enable approved users in Ring 3.0 to access the Teams Learning app (private preview).

As part of private preview, the Teams Learning app (private preview) is released in Ring 3.0. If your organization is in Ring 4.0, you won’t see the app in the app store. To test the app, you need to create a custom apps permission policy, set it to **Allow all apps**, and assign it to Ring 3.0 approved users.

   ![TAP-AppsPermission-Plcy page showing Allow all apps selected](media/learning-app-tap-appspermission-plcy.png)

## Configure learning content sources in the Microsoft 365 admin center

The admins for the Microsoft 365 admin center can manage settings related to the Teams Learning app (private preview) and can configure the learning content sources.

The admin can select which additional learning content sources (for example, SharePoint or supported third-party content provider sources) will be available to users of the app. The admin then configures those sources to make sure the content is available for search and discovery and can be browsed by the employees who use the app.

> [!NOTE]
>  Users sign in to non-Microsoft and LinkedIn Learning Pro learnings in a browser or embedded viewer. This configured learning is subject to the separate license, privacy and service terms between your organization and the third party, and not the Learning (Preview) terms. Before selecting this learning in Learning (Preview), verify you have an agreement in place for your organization and users.

### Configure settings for the learning content sources for the app

These steps are to be performed by the Microsoft 365 admin.

1.	In the left navigation of the Microsoft 365 admin center, go to **Settings** > **Org settings**.

2.	On the **Settings** page, on the **Services & add-ins** tab, select **Learning app**.

   ![Settings page in the Microsoft 365 admin center showing the Learning app listed](media/learning-app-365-settings-page.png)

3.	On the **Learning app** panel, select the learning content sources you want to configure for the organization, and then select **Save**.

   ![Learning app panel in the Microsoft 365 admin center showing content sources options](media/learning-app-365-settings-learning-app-panel.png)

Among all the learning sources that exist, some will be enabled by default. These include:

- LinkedIn Learning (free content)
- Microsoft Learn
- Microsoft 365 Training

> [!NOTE]
> If your organization has a LinkedIn Learning Standard or Pro subscription, the content repository will be unlocked for the employees in your organization. Only those employees who have permission will be able to use the entire content repository.

Other sources might need to be enabled or configured manually. Learning sources that are not from Microsoft are separately licensed between your organization and the third party. You’ll need to verify you’ve signed up for their learning for you and your users.

To enable or disable a learning content source, select the check box next to the source. If a source is enabled, a check mark will be visible.

## Configure SharePoint as a learning content source (Coming Soon)

You configure SharePoint as a learning content source for the Teams Learning app (private preview) in the Microsoft 365 admin center.

### Overview

The admin provides a site URL to where the Learning Service can create an empty centralized learning content repository in the form of a structured SharePoint list. This list can be used by the organization to house links to cross-company SharePoint folders that contain learning content. Admins are responsible for collecting and curating a list of URLs for folders. These folders should only include content that can be made available in the Teams Learning app (private preview).

### Permissions

Folder URLs can be collected from any SharePoint site in the organization. Any content within these folders will be searchable, but only content to which the individual employee has permissions can be used.
 
### Learning Service

The Learning Service uses the provided folder URLs to get metadata from all content stored in those folders. Within 24 hours of supplying the folder URL in the centralized repository, employees can search for and use the company’s content within the app. Content deletion from the repository isn't supported at this point. Unintentionally surfaced content can only be removed by supplying a new SharePoint site URL in the Microsoft 365 admin center.

### Configure SharePoint as a source

These steps are to be performed by Microsoft 365 admin.

1.	In the left navigation of the Microsoft 365 admin center, go to **Settings**.
 
2.	On the **Settings** page, on the **Services & add-ins** tab, select **Learning app**.

   ![Settings page in the Microsoft 365 admin center showing the Learning app listed](media/learning-app-365-settings-page.png)

3.	On the **Learning app** panel, provide the site URL to the SharePoint site where you want the app to create a centralized repository.

   ![Learning app panel in the Microsoft 365 admin center showing SharePoint selected](media/learning-app-365-panel-sharepoint-selected.png)

4.	A SharePoint list is created automatically within the provided organization’s SharePoint site. In the left navigation of the SharePoint site, select **Learning App Content Repository**. 

   ![Left navigation in SharePoint showing the Learning App Content Repository section](media/learning-app-content-repository-nav.png)

 
5. On the **Learning App Content Repository** page, populate the SharePoint list with URLs to the learning content folders.

   1.	Select **New** to view the **New item** panel. 

   ![Learning App Content Repository page in SharePoint showing the New option](media/learning-app-content-repository-new.png)
 
   2.	On the **New item** panel, in the **Title** field, add a directory name of your choice. In the **Folder URL** field, add the URL to the learning content folder. Select **Save**.

   ![New item panel in SharePoint showing the Title and Folder URL fields](media/learning-app-new-item-panel.png)

   3. The Learning App Content Repository page is updated with the new learning content.

   ![Learning App Content Repository page in SharePoint showing the updated information](media/learning-app-content-repository-populated.png)


 


