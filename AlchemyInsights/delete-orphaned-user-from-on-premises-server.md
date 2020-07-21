---
title: Brisanje sirotišnog korisnika s lokalnog poslužitelja
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/20/2020
ms.locfileid: "45197822"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="e8025-102">Brisanje sirotišnog korisnika s lokalnog poslužitelja</span><span class="sxs-lookup"><span data-stu-id="e8025-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="e8025-103">Da biste uklonili napuštenog korisnika, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="e8025-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="e8025-104">Prisilno sinkronizacija direktorija slijedeći upute u odjeljku [Što je hibridni identitet servisa Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="e8025-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="e8025-105">Da biste provjerili sinkronizaciju direktorija, pročitajte [što je hibridni identitet servisa Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="e8025-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="e8025-106">Ako sinkronizacija ispravno funkcionira, ali brisanje objekta servisa Active Directory ne propagira Azure AD, ručno uklonite napušteni objekt pomoću jednog od sljedećih cmdleta Azure Active Directory Module za Windows PowerShell:</span><span class="sxs-lookup"><span data-stu-id="e8025-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="e8025-107">Ukloni-MsolKontakt</span><span class="sxs-lookup"><span data-stu-id="e8025-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="e8025-108">Ukloni-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="e8025-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="e8025-109">Ukloni-MsolUser</span><span class="sxs-lookup"><span data-stu-id="e8025-109">Remove-MsolUser</span></span>

    <span data-ttu-id="e8025-110">Na primjer, da biste uklonili john.smith@contoso.com za napušteni korisnički ID, izvorno stvoren pomoću sinkronizacije direktorija, pokrenite cmdlet:</span><span class="sxs-lookup"><span data-stu-id="e8025-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="e8025-111">Maknuti-MsolUser – UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="e8025-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>