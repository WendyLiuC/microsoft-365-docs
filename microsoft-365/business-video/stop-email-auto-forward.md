---
title: "Stop auto-forwarding emails"
f1.keywords:
- NOCSH
ms.author: kwekua
author: kwekua
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ms.localizationpriority: medium
ms.collection: 
- M365-subscription-management 
- Adm_O365
ms.custom: 
- AdminSurgePortfolio
- adminvideo
- AdminTemplateSet
- admindeeplinkMAC
monikerRange: 'o365-worldwide'
search.appverid:
- BCS160
- MET150
- MOE150
description: "Learn how to stop auto-forwarding emails by creating a mail flow rule to avoid theft of proprietary info."
---

# Stop email auto-forward

## Watch: Stop auto-forwarding emails

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE2W6kS?autoplay=false]

If a hacker gains access to a user's mailbox, they can auto-forward the user's email to an outside address and steal proprietary information. You can stop this by creating a mail flow rule.

## Try it!

1. From the <a href="https://go.microsoft.com/fwlink/p/?linkid=2024339" target="_blank">Microsoft 365 admin center</a>, select **Exchange**, **mail flow**, and on the **rules** tab, select the plus sign and choose **create a new rule**.
1. Select **More options**. Name your new rule.
1. Then open the drop-down for **apply this rule if**, select **the sender**, and then **is external internal**.
1. Select **Inside the organization**, and then **OK**.
1. Choose **add condition**, open the drop-down, select **The message properties**, then **include the message type**.
1. Open the **select message type** drop-down, choose **Auto-forward**, then **OK**.
1. Open the **Do the following** drop-down, select **Block the message**, then **reject the message and include an explanation**.
1. Enter the message text for your explanation, then select **OK**.
1. Scroll to the bottom and select **Save**.

    Your rule has been created, and hackers will no longer be able to auto-forward messages.

## Related content

[Add another email alias for a user](../admin/email/add-another-email-alias-for-a-user.md) (article)\
[Configure email forwarding in Microsoft 365](../admin/email/configure-email-forwarding.md) (article)\
[Find and fix email delivery issues as an Office 365 for business admin](/exchange/troubleshoot/email-delivery/email-delivery-issues) (article)