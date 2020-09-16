---
title: Prilikom dodavanja dodataka u programu Outlook više je korisnika došlo do odbijanja programa Access
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 611a4df473458abc0ab0c65442f2141763f7b868
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724355"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="a18d9-102">Prilikom dodavanja dodataka u programu Outlook više je korisnika došlo do odbijanja programa Access</span><span class="sxs-lookup"><span data-stu-id="a18d9-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="a18d9-103">Možete odrediti koji administratori u tvrtki ili ustanovi imaju dozvole za instalaciju i upravljanje dodacima za Outlook.</span><span class="sxs-lookup"><span data-stu-id="a18d9-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="a18d9-104">Možete i odrediti koje korisnike u tvrtki ili ustanovi imaju dozvolu za instalaciju i upravljanje dodacima za vlastitu upotrebu.</span><span class="sxs-lookup"><span data-stu-id="a18d9-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="a18d9-105">Pojedinosti potražite u članku [određivanje administratora i korisnika koji mogu instalirati dodatke za Outlook i upravljati njima](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="a18d9-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="a18d9-106">Da biste potvrdili da ste uspješno dodijelili dozvole za korisnika, zamijenite <Role Name> naziv uloge koju želite provjeriti, a zatim pokrenite sljedeću naredbu u komponenti Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="a18d9-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="a18d9-107">Get-Managementroledodjeljivanje-uloga " <Role Name> "-geteffectiveusers</span><span class="sxs-lookup"><span data-stu-id="a18d9-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="a18d9-108">U ovom se primjeru prikazuje kako potvrditi kome ste dodijelili dozvole za instalaciju dodataka iz trgovine sustava Office za tvrtku ili ustanovu.</span><span class="sxs-lookup"><span data-stu-id="a18d9-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="a18d9-109">PowerShell</span><span class="sxs-lookup"><span data-stu-id="a18d9-109">PowerShell</span></span>

<span data-ttu-id="a18d9-110">-Uloga "aplikacije tvrtke org Marketplace"-GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="a18d9-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="a18d9-111">U rezultatima Get-Managelmentroledodjela Pregledajte unose u stupcu efektivni korisnici.</span><span class="sxs-lookup"><span data-stu-id="a18d9-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="a18d9-112">Detaljne informacije o sintaksi i parametrima potražite [u članku Get-Managelmentrolezadatak](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="a18d9-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 