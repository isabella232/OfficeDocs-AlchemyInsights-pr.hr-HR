---
title: Više korisnika dobiva pogrešku odbijen pristup prilikom dodavanja dodataka u programu Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423360"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="cdce4-102">Više korisnika dobiva pogrešku odbijen pristup prilikom dodavanja dodataka u programu Outlook</span><span class="sxs-lookup"><span data-stu-id="cdce4-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="cdce4-103">Možete odrediti koji administratori u tvrtki ili ustanovi imaju dozvole za instalaciju dodataka i upravljanje njima za Outlook.</span><span class="sxs-lookup"><span data-stu-id="cdce4-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="cdce4-104">Možete odrediti i koji korisnici u vašoj tvrtki ili ustanovi imaju dozvolu za instalaciju dodataka i upravljanje njima za vlastitu upotrebu.</span><span class="sxs-lookup"><span data-stu-id="cdce4-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="cdce4-105">Pojedinosti potražite [u članku Određivanje administratora i korisnika koji mogu instalirati dodatke za Outlook i upravljati njima](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="cdce4-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="cdce4-106">Da biste provjerili jeste li uspješno dodijelili dozvole korisniku, <Role Name> zamijenite nazivom uloge koju želite provjeriti i pokrenite sljedeću naredbu u dodatku PowerShell sustava Exchange Online:</span><span class="sxs-lookup"><span data-stu-id="cdce4-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="cdce4-107">Get-ManagementRoleAssignment -Uloga " <Role Name> " -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="cdce4-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="cdce4-108">Ovaj primjer pokazuje kako provjeriti kome ste dodijelili dozvole za instalaciju dodataka iz Office trgovine za tvrtku ili ustanovu.</span><span class="sxs-lookup"><span data-stu-id="cdce4-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="cdce4-109">Powershell</span><span class="sxs-lookup"><span data-stu-id="cdce4-109">PowerShell</span></span>

<span data-ttu-id="cdce4-110">-Uloga "Org Marketplace Apps" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="cdce4-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="cdce4-111">U rezultatima, Get-ManagementRoleAssignment, pregledajte stavke u stupcu Učinkoviti korisnici.</span><span class="sxs-lookup"><span data-stu-id="cdce4-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="cdce4-112">Detaljne informacije o sintaksi i parametrima [potražite u odjeljku Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="cdce4-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 