---
title: Brisanje korisnika koji su napušteni s lokalnog poslužitelja
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 537ae7edebfa5a4ab71c2141d549d732ed4f883f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680127"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="11e45-102">Brisanje korisnika koji su napušteni s lokalnog poslužitelja</span><span class="sxs-lookup"><span data-stu-id="11e45-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="11e45-103">Da biste uklonili siroog korisnika, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="11e45-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="11e45-104">Prisilno Sinkroniziranje direktorija slijedite upute u odjeljku [što je hibridni identitet sa servisom Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="11e45-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="11e45-105">Da biste potvrdili sinkronizaciju direktorija, pročitajte članak [što je hibridni identitet sa servisom Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="11e45-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="11e45-106">Ako sinkronizira funkcionira ispravno, no Brisanje objekta servisa Active Directory ne prenosi se na Azure AD, ručno uklonite napušteni objekt pomoću jednog od sljedećih modula za Azure Active Directory za Windows PowerShell za cmdlete:</span><span class="sxs-lookup"><span data-stu-id="11e45-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="11e45-107">Uklanjanje-MsolContact</span><span class="sxs-lookup"><span data-stu-id="11e45-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="11e45-108">Uklanjanje-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="11e45-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="11e45-109">Uklanjanje-MsolUser</span><span class="sxs-lookup"><span data-stu-id="11e45-109">Remove-MsolUser</span></span>

    <span data-ttu-id="11e45-110">Da biste, primjerice, uklonili john.smith@contoso.com ID korisnika, izvorno stvoren pomoću sinkronizacije direktorija, pokrenite cmdlet:</span><span class="sxs-lookup"><span data-stu-id="11e45-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="11e45-111">Uklanjanje-MsolUser – UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="11e45-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>