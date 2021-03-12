---
title: Upotrijebite Windows PowerShell za pravilnike za zajedničko korištenje i odnose u tvrtki ili ustanovi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: cd1d34e4dae474e61c799ca9234b2f18c718f27b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709458"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="aa5be-102">Upotrijebite Windows PowerShell za pravilnike za zajedničko korištenje i odnose u tvrtki ili ustanovi</span><span class="sxs-lookup"><span data-stu-id="aa5be-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="aa5be-103">Za odnose u tvrtki ili ustanovi pregledajte detaljnu sintaksu i podatke o parametru za: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  I  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="aa5be-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="aa5be-104">Za stvaranje pravilnika o zajedničkom korištenju upotrijebite [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="aa5be-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="aa5be-105">Za [primjenu pravilnika o zajedničkom korištenju na poštanski sandučić ili korisnika](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) morate upotrijebiti kombinaciju [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) i [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) s novostvorenim pravilnikom.</span><span class="sxs-lookup"><span data-stu-id="aa5be-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="aa5be-106">Za [izmjenu, onemogućivanje ili uklanjanje pravilnika o zajedničkom korištenju](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  morate upotrijebiti[Set-Sharing Policy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) i [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="aa5be-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="aa5be-107">**Za potpuno razumijevanje ove teme pročitajte:**</span><span class="sxs-lookup"><span data-stu-id="aa5be-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="aa5be-108">Zajedničko korištenje u sustavu Exchange Online</span><span class="sxs-lookup"><span data-stu-id="aa5be-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)