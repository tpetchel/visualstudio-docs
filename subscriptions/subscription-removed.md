---
title: What happens when your Visual Studio subscription is removed | Microsoft Docs
author: evanwindom
ms.author: amast
manager: shve
ms.assetid: 34eaceda-f5db-41d6-bc23-ecf55fe1768e
ms.date: 07/25/2023
ms.topic: troubleshooting
ms.custom: kr2b-contr-experiment
description: Learn what happens when your admin removes your Visual Studio subscription. This information includes how your benefits change and support resources.
---

# What happens when an admin removes my subscription?

If your Visual Studio subscription was assigned to you by an admin in your work or school organization, they may remove it at some point.  Reasons may include changes to job roles or to your organization's purchase plans.  This article outlines what you can expect if an admin removes your subscription.  

> [!TIP]
> If your admin removes your subscription, they may be planning to issue you a different subscription.  If you receive a notification that your subscription has been removed, you may wish to reach out to your admin to see if another subscription is available. Visit the [subscriber portal](https://my.visualstudio.com) and select the **Contact my admin** button in the top right.

## How do my benefits change?

The changes you see for a specific benefit depend on the benefit itself.  This article looks at some examples, and discusses steps you need to take to make sure you have access to things like your Azure assets. 

### Visual Studio IDE

The license for the Visual Studio IDE is dependent on a subscription being assigned to you.  If your subscription is removed, you lose access to any version of the IDE provided in a paid subscription.  If you still need Visual Studio, consider installing the free version: [Visual Studio Code](https://code.visualstudio.com/).  

### Individual Azure credits

When your subscription is removed, you no longer accrue individual Azure credits.  The credits you've already accrued remain available for 30 days.  After that time, your assets will no longer be available. 

To avoid losing your assets, make sure to take one of the following steps if your subscription is removed:

+ Convert the subscription to pay-as-you-go.  For details, visit our [Azure DevTest Pay-As-You-Go subscriptions page](https://azure.microsoft.com/offers/ms-azr-0023p/).  You need to attach a payment instrument such as a credit card to this subscription. 
+ Move your assets to another Azure subscription if one is available to you.  For example, if you have an Azure subscription as part of a different Visual Studio subscription.  Instructions for [moving resources to a new subscription](/azure/devtest/offer/how-to-change-directory-tenants-visual-studio-azure) are included in Azure's documentation.  

  > [!IMPORTANT]
  > It's important that you move your Azure assets to another Azure subscription or change the existing Azure subscription to pay-as-you-go to avoid loss of your existing Azure assets. 

### Software downloads and product keys

Access to software downloads and product keys from within the subscriptions portal is lost. 

### Azure DevOps

Access to Azure DevOps requires a license and is lost.

### Other benefits

The effects of having a subscription removed vary.  

+ Benefits with a fixed length

  Many of the benefits provided by our partners are offers that have a fixed length.  If you've activated them prior to the removal of your subscription, many of them are unaffected and remain available to you until the end of their normal term.  If you've been accessing those benefits through the subscriber portal, you need to access them directly on the partner site.  For example, let's say you received a Pluralsight subscription as part of a Visual Studio subscription.  When your Visual Studio subscription is removed, you still have any remaining time on the training subscription, but you need to sign in to Pluralsight's website directly.

+ Benefits that require sign-in for each use are no longer available.

+ Upon removal of your subscription, you lose the ability to activate any more benefits.  

## Visual Studio subscription assignments deleted by Microsoft

If you're a subscriptions admin, you might occasionally see in your dashboard that Microsoft has removed a subscription.  The reason says that the account is closed. 

### Why an account may be removed  

+ Subscribers request closure of their Microsoft accounts. If a subscriber requests closure of a Microsoft account (MSA), subscriptions associated with that MSA are removed.  For more information including important things to consider before closing an account, see [How to close your Microsoft account](https://support.microsoft.com/account-billing/how-to-close-your-microsoft-account-c1b2d13f-4de6-6e1b-4a31-d9d668849979).
+ Subscribers are removed from Azure Active Directory tenant.  Subscriptions can automatically assign subscriptions through an Azure Active Directory group.  When they're removed from the group, their subscriptions are removed.

### What happens when the account is closed?

If the subscription is removed, the subscriber loses access to the subscription.  If a subscriber is removed from an Azure AD group, their subscription information is permanently removed within 180 days.  If a subscriber closes their MSA, their information is removed immediately.  

## Support resources

+ For assistance with sales, subscriptions, accounts and billing for Visual Studio Subscriptions, contact [Visual Studio subscriptions support](https://my.visualstudio.com/gethelp).
+ Have a question about Visual Studio IDE, Azure DevOps, or other Visual Studio products or services?  Visit [Visual Studio support](https://visualstudio.microsoft.com/support/).

## See also

+ [Visual Studio documentation](/visualstudio/)
+ [Azure DevOps Services documentation](/azure/devops/)
+ [Azure documentation](/azure/)
+ [Microsoft 365 documentation](/microsoft-365/)

## Next steps

+ Learn about [Azure DevOps](https://azure.microsoft.com/services/devops/) features
+ Learn about [Visual Studio IDE features by edition](https://visualstudio.microsoft.com/vs/compare/)
