---
title: 'RBAC uloge '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583240"
---
# <a name="rbac-rules"></a><span data-ttu-id="2598d-102">RBAC pravila</span><span class="sxs-lookup"><span data-stu-id="2598d-102">RBAC rules</span></span>

<span data-ttu-id="2598d-103">Ako vam se prikaže pogreška s dozvolom:</span><span class="sxs-lookup"><span data-stu-id="2598d-103">If you get the permission error:</span></span> 

- <span data-ttu-id="2598d-104">**Naručitelj s ID-om objekta nema ovlaštenje za izvršavanje akcije nad optikom (kod: Autorizacija nije ispunilo proročanstvo)**: kada pokušate stvoriti resurs, provjerite jeste li trenutno prijavljeni uz korisnika kojem je dodijeljena uloga koja sadrži dozvolu za zapisivanje resursa u odabranom opsegu.</span><span class="sxs-lookup"><span data-stu-id="2598d-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="2598d-105">Da biste, primjerice, upravljali virtualnim strojevima u grupi resursa, trebali biste imati ulogu [suradnika virtualnog stroja](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) u grupi resursa (ili nadređenom opsegu).</span><span class="sxs-lookup"><span data-stu-id="2598d-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="2598d-106">Popis dozvola za svaku ugrađenu ulogu potražite [u članku ugrađene uloge za resurse Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="2598d-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="2598d-107">Nemate **dozvolu za stvaranje zahtjeva za podršku**: kada pokušate stvoriti ili ažurirati ulaznicu za podršku, provjerite jeste li trenutno prijavljeni uz korisnika kojem je dodijeljena uloga koja sadrži dozvolu Microsoft. support/supportTickets/Write, kao što je [suradnik zahtjeva za podršku](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span><span class="sxs-lookup"><span data-stu-id="2598d-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="2598d-108">**Nema više dodjela uloga koje je moguće stvoriti (kod: Roledodjela vrijednosti)**: kada pokušate dodijeliti ulogu, pokušajte smanjiti broj dodjela uloga tako da dodijelite uloge grupama.</span><span class="sxs-lookup"><span data-stu-id="2598d-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="2598d-109">Azure podržava do **2000** dodjela uloga po pretplati.</span><span class="sxs-lookup"><span data-stu-id="2598d-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="2598d-110">Dodatne informacije o ulogama Azure RBAC potražite u članku [Azure RBAC uloge](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="2598d-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
