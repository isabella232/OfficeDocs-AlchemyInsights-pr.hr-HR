---
title: Korištenje komponente PowerShell za pravila zajedničkog korištenja i odnosa tvrtke ili ustanove
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862037"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Korištenje komponente PowerShell za pravila zajedničkog korištenja i odnosa tvrtke ili ustanove


Za odnose tvrtke ili ustanove pregledajte detaljne informacije o sintaksi i parametrima za : [Get- FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New- OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set- OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) AND [Remove- OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Da biste stvorili pravila dijeljenja, [koristite New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Da biste [pravila zajedničkog korištenja primijenili na poštanski sandučić ili korisnik,](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) morate koristiti kombinaciju [set-mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) i [get-mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) s novostvorenim pravilima. Da biste [izmijenili, onemogućili ili uklonili pravilo zajedničkog korištenja,](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) morate koristiti [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) i [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Za potpuno razumijevanje ove teme molimo pročitajte:**

[Zajedničko korištenje u sustavu Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)