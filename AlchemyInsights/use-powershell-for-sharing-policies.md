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
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="86714-102">Korištenje komponente PowerShell za pravila zajedničkog korištenja i odnosa tvrtke ili ustanove</span><span class="sxs-lookup"><span data-stu-id="86714-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="86714-103">Za odnose tvrtke ili ustanove pregledajte detaljne informacije o sintaksi i parametrima za : [Get- FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New- OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set- OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) AND [Remove- OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="86714-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="86714-104">Da biste stvorili pravila dijeljenja, [koristite New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="86714-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="86714-105">Da biste [pravila zajedničkog korištenja primijenili na poštanski sandučić ili korisnik,](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) morate koristiti kombinaciju [set-mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) i [get-mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) s novostvorenim pravilima.</span><span class="sxs-lookup"><span data-stu-id="86714-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="86714-106">Da biste [izmijenili, onemogućili ili uklonili pravilo zajedničkog korištenja,](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) morate koristiti [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) i [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="86714-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="86714-107">**Za potpuno razumijevanje ove teme molimo pročitajte:**</span><span class="sxs-lookup"><span data-stu-id="86714-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="86714-108">Zajedničko korištenje u sustavu Exchange Online</span><span class="sxs-lookup"><span data-stu-id="86714-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)