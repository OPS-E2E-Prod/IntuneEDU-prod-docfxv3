---
# required metadata

title: Add apps
titleSuffix: Intune for Education
description:
keywords:
author: barlanmsft
ms.author: barlan
manager: angrobe
ms.date: 03/24/2017
ms.topic: article
ms.prod:
ms.service:
ms.technology:
ms.assetid: 24ab6547-aa65-428a-b184-06b806e95bd1
searchScope:
 - IntuneEDU

# optional metadata

#ROBOTS:
#audience:
#ms.devlang:
ms.reviewer:
#ms.suite: ems
#ms.tgt_pltfrm:
#ms.custom:

---

# Add apps in Intune for Education

Before you can install apps to your school's devices with Intune for Education, those apps must be added to your Intune for Education account.

Intune for Education supports the following types of apps:
- Web apps, such as [Microsoft Word Online](https://office.live.com/start/Word.aspx)
- Windows Store for Business apps, which are any [Universal apps distributed through the Store](https://technet.microsoft.com/itpro/windows/manage/apps-in-windows-store-for-business)
- Desktop (Win32) applications, such as [standalone Microsoft Office](https://products.office.com/products)

After you add apps, you can [install the apps](install-apps.md) on groups of devices.

## Add web apps

A _web app_ is an app that is accessed by users exclusively in a browser. They are easy to assign because all you have to send to users are links to websites, rather than sending any install files to their devices.

You can assign web apps as links in the Start menu of Windows 10 devices using Intune for Education. To assign an app, you must first add it to Intune for Education in the **Manage apps** section.

  ![The add a new web app page, which prompts users for the information described in the procedure below.](./media/apps-001-add-webapp.png)

1. In the [Intune for Education](https://intuneeducation.portal.azure.com) console, choose **Apps** > **Add apps** > **New app**.
2. Under **Web apps**, select **+ New app**, then enter the following details:
 - **URL** - The URL of the app that you want to assign
 - **App name** - The name of the app displayed in the Start menu on devices
 - **Icon** - Upload a PNG or JPG from your computer to use as an icon for the app
3. Choose **Save**. Your web app is now ready.
4. You can now [install the app on devices](install-apps.md).

You can edit the app at any time by choosing **Edit**, which re-opens its details page.

## Add Windows Store for Business apps

Apps that you've acquired from the Windows Store for Business are automatically available in Intune for Education. Any time you make changes to your app ownership, such as buying new apps or revoking purchases, that change is reflected in Intune for Education.

1. In the [Intune for Education](https://intuneeducation.portal.azure.com) console, choose **Apps**.

2. Under **Windows Store apps**, select **+ New app** to open your Windows Store for Business account. You can search for apps that you want to add using the search bar at the top right corner of the screen.

> [!Note]
> If you have not added Intune for Education as a management tool, you will need to [activate it before you can take any actions](https://technet.microsoft.com/itpro/windows/manage/apps-in-windows-store-for-business#licensing-model).

  ![The search screen in the Windows Store for Business, showing two results for the search term 'Socrative', one for the Socrative app and the other for the Socrative Student app.](./media/apps-002-search-for-wsfb-app.png)

  After you find it, go ahead and acquire the required number of licenses for the app. Unlimited licenses are the standard for all free apps.

  ![The Socrative app screen in the Windows Store for Business.](./media/apps-003-get-wsfb-app.png)

  Once you've acquired the licenses, you'll see a confirmation message that lets you know you've acquired the app.

3. Intune for Education will update to show your purchase in the list of **Windows Store apps**. This could take up to 12 hours, but usually is complete within a couple of minutes.

  ![The sidebar of the apps page, which shows the Socrative app successfully added to the list of Windows Store apps.](./media/apps-004-sidebar-list-of-wsfb-apps.png)

4. You can now [install the app on devices](install-apps.md).

## Add popular apps

You can install popular educational apps with a single click. Our goal is to make it easy for you to find and install your favorite apps for your users. We recommend these apps because they are frequently useful to educators. You can find these apps in Express Configuration, or under the **Manage apps** tile.

  ![A selection of popular apps during the add apps process in Express Configuration.](./media/apps-005-popular-apps.png)

The Intune for Education portal shows the top 12 educational web apps and top 12 educational Windows Store for Business apps that you haven’t added under **Apps** management.

1. In the [Intune for Education](https://intuneeducation.portal.azure.com) console, choose  **Manage Apps** > **Add apps** > **Quick add popular apps**. A list of **Web apps** and **Windows Store apps** is displayed.

  ![The quick add popular apps screen.](./media/apps-006-add-popular-apps.png)

2. Select the apps you want to add, then choose **Add apps**.

  ![Selecting multiple popular apps to add to the portal.](./media/apps-007-select-multiple-popular-apps.png)

3. Your apps will add in the background and appear in the left hand sidebar when ready.

  ![Your apps are being added screen.](./media/apps-008-your-popular-apps-are-being-added.png)

><!-- [&larr; **Add apps**](.\add-apps.md)      [**Install apps** &rarr;](.\install-apps.md) -->