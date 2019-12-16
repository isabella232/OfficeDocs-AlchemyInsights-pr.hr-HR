---
title: Otklanjanje poteškoća s porukama odbijeno za pristup
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 57919e6dbd81a5bf3b17fb067485e8eec23b7d4c
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051417"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="45f6c-102">Otklanjanje poteškoća s porukama odbijeno u centru za administraciju sustava SharePoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="45f6c-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="45f6c-103">Ako primite poruku o odbijanju pristupa prilikom pokušaja pregledavanja u centar za administraciju sustava SharePoint/OneDrive, provjerite jeste li [korisniku dodijelili licencu](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="45f6c-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="45f6c-104">Ako korisnik ima licencu, također biste trebali osigurati da im je [dodijeljena administratorska uloga](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) koja može pristupiti centrima za administraciju.</span><span class="sxs-lookup"><span data-stu-id="45f6c-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="45f6c-105">Taj se problem može pojaviti i kada se korisnik izbriše i ponovno stvori s istim korisničkim nazivom (UPN).</span><span class="sxs-lookup"><span data-stu-id="45f6c-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="45f6c-106">Novi račun kreira se pomoću različite vrijednosti PUID</span><span class="sxs-lookup"><span data-stu-id="45f6c-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="45f6c-107">Kada korisnik pokuša pristupiti zbirci web-mjesta ili svom servisu OneDrive, korisnik ima neispravan PUID.</span><span class="sxs-lookup"><span data-stu-id="45f6c-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="45f6c-108">Drugi scenarij uključuje sinkronizaciju direktorija s organizacijskom jedinicom Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="45f6c-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="45f6c-109">Ako su se korisnici već prijavili u SharePoint, a zatim se premještaju u drugi OU i ponovno sinkroniziraju sa sustavom SharePoint, možda će doživjeti taj problem.</span><span class="sxs-lookup"><span data-stu-id="45f6c-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="45f6c-110">Da biste riješili taj problem, trebali biste vratiti izvorni UPN s koracima u članku, [vratiti korisnika u Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="45f6c-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="45f6c-111">Napomena: Ako servis OneDrive ili SharePoint admin centar nije dostupan više korisnika koji su ranije imali pristup, možda postoji problem privremenog servisa.</span><span class="sxs-lookup"><span data-stu-id="45f6c-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="45f6c-112">[Provjerite nadzornu ploču zdravstvenog stanja usluge](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="45f6c-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


