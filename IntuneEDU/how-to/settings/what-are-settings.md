---
# required metadata

title: What are settings? | Intune for Education | Microsoft Docs
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
ms.assetid: 91d004c0-8d06-4307-8868-46ac7b119101

---

# What are settings?
<!--intro text-->

## How settings work between different groups

If there's a group above a group, it's inherited. But let's say there's a situation that doesn't work for that, so there's a lab under a group that needs to be different. So this is how we override.

Settings on this group are being inherited from its parent group. Changing any setting on this group will override the inheritance for this group and it's children. Child group = Subgroup; figure definitions for parent group here

Once inheritance is broken, all inheritance is broken - including new settings applied to parent Groups

Reset inheritance will break broken inheritance and restore settings from the parent back to the subgroup. Once you Save Changes, it resets the settings to show what they're looking like.

Any time you have a subgroup, it will naturally inherit from its parent group

## Manage settings

Settings are managed on a per-group basis. You can manage the simple list of useful settings using [Express Configuration](what-are-settings.md#manage-settings-in-express-configuration) or view a full list of settings for a group for fine-tuning from [Groups management](what-are-settings.md#manage-settings-for-groups).

Device settings apply to all devices in their group. Settings that are **Not configured** default to the settings made on the device. Intune for Education settings such as **Block** or **Allow** overrule the device’s settings. For example, if a device has a camera and that camera is enabled by default, but the group setting for that device has Camera set to **Block**, then the camera on the device will be turned off.

Subgroup settings overrule their parent group settings. For example, if a device belongs to the **All Students** group which has **Camera** set to **Not configured** and also belongs to the **Kindergarten** subgroup which has **Camera** set to **Block**, then the camera on devices in the **Kindergarten** group will be turned off.

## Manage settings in Express Configuration

Use the following steps to manage simplified list of settings in Intune for Education:
1. In the [Intune for Education](https://manage.windowsazure.com) console, click **Launch Express Configuration**. Review the **Welcome** page and click **Get started**.
2. Review the **Get school information** page. If you've already added school information, and then click **Next**.
3. Select the group whose settings you want to manage, and then click **Next**.
4. Review the list of apps, and then click **Next**.
5. On the **Settings** page, expand the categories of available settings:
  - [Basic device settings](available-settings.md#basic-device-settings)
  - [Internet browser settings](available-settings.md#internet-browser-settings)
  - [Device update settings](available-settings.md#device-update-settings)
  - [Networking and connection settings](available-settings.md#networking-and-connectivity)
  - [App settings](available-settings.md#app-settings)
  - [Sign in settings](available-settings.md#sign-in-settings)

  Expand a category and toggle the control to modify settings, and then click **Next**.
6. Review your choices and then click **Finish** to save your changes update them on devices in the selected group.

## Manage settings for groups

Use the following steps to manage the full list of settings in Intune for Education:
1. In the [Intune for Education](https://manage.windowsazure.com) console, in the left-side navigation menu, click **Groups**.
2. Select the group whose settings you want to manage. For a complete list, see [Available settings](what-are-settings.md).
3. Click **Settings** at the top of the page to view the full list of available settings.
4. Expand categories and modify individual settings for the selected group.
5. Click **Save** to save the changes for that group. Settings are automatically sent to devices in that group.