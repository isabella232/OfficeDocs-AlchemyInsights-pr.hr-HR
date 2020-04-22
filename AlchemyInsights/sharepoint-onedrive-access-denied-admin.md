---
title: Otklanjanje poteškoća s porukama odbijenim pristupom
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758377"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="81b38-102">Otklanjanje poteškoća s porukama u kojima je odbijen pristup u centru za administratore sustava Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="81b38-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="81b38-103">Ako prilikom pokušaja pregleda u centru za administratore sustava Sharepoint/OneDrive primite poruku odbijenog pristupa, svakako [dodijelite licencu korisniku](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="81b38-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="81b38-104">Ako korisnik ima licencu, provjerite im [dodijeljenu administratorsku ulogu](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) koja može pristupiti centrima za administratore.</span><span class="sxs-lookup"><span data-stu-id="81b38-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="81b38-105">Taj se problem može pojaviti i kada se korisnik izbriše i ponovno stvori s istim korisničkim glavnim nazivom (UPN).</span><span class="sxs-lookup"><span data-stu-id="81b38-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="81b38-106">Novi račun stvara se pomoću različite VRIJEDNOSTI PUID (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="81b38-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="81b38-107">Kada korisnik pokuša pristupiti zbirci web-mjesta ili na servisu OneDrive, korisnik ima pogrešan PUID.</span><span class="sxs-lookup"><span data-stu-id="81b38-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="81b38-108">Drugi scenarij uključuje sinkronizaciju direktorija s organizacijskom jedinicom servisa Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="81b38-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="81b38-109">Ako su se korisnici već prijavili u SharePoint, a zatim se premještaju u drugi OU i ponovno sinkroniziraju sa sustavom SharePoint, mogu se pojaviti taj problem.</span><span class="sxs-lookup"><span data-stu-id="81b38-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="81b38-110">Da biste riješili taj problem, trebali biste vratiti izvorni UPN s koracima iz članka, [Vraćanje korisnika u Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="81b38-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="81b38-111">Napomena: ako centar za administratore servisa OneDrive ili Sustava SharePoint nije dostupan većem broju korisnika koji su prethodno imali pristup, možda postoji problem s privremenim servisom.</span><span class="sxs-lookup"><span data-stu-id="81b38-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="81b38-112">[Provjerite nadzornu ploču stanja servisa](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="81b38-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


