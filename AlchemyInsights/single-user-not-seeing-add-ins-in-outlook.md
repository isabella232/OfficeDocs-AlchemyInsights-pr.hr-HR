---
title: Jedan korisnik koji ne prikazuje dodatke u programu Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 8c99b443a2d83f3ac24362d63cd6363a66a81393
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719657"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="e2ebe-102">Jedan korisnik koji ne prikazuje dodatke u programu Outlook</span><span class="sxs-lookup"><span data-stu-id="e2ebe-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="e2ebe-103">Korisnik može biti dio uloge koja nema ispravni parametar AppsForOfficeEnabled.</span><span class="sxs-lookup"><span data-stu-id="e2ebe-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="e2ebe-104">Pokrenite ovaj cmdlet da biste saznali je li ispravna uloga povezana s korisnikom:</span><span class="sxs-lookup"><span data-stu-id="e2ebe-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="e2ebe-105">Get-Managelmentroledodjeljivanje-Rojesignee user@domain.com-deleating $false | Format-table-auto uloga, Rojesigneename, Rojesigneetype</span><span class="sxs-lookup"><span data-stu-id="e2ebe-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="e2ebe-106">Dodatne informacije potražite u članku [određivanje administratora i korisnika koji mogu instalirati dodatke za Outlook i upravljati njima](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="e2ebe-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
