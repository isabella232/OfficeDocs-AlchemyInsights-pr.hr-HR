---
title: Otklanjanje poteškoća s porukama odbijeno za web-mjesta OneDrive za tvrtke
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 3c40ad76a8961a3d0b4963483291c2a1364c51d3
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/15/2019
ms.locfileid: "37766703"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="f4865-102">Otklanjanje poteškoća s porukama odbijeno za web-mjesta OneDrive za tvrtke</span><span class="sxs-lookup"><span data-stu-id="f4865-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="f4865-103">Taj se problem najčešće pojavljuje kada se korisnik izbriše i ponovno stvori s istim korisničkim nazivom (UPN).</span><span class="sxs-lookup"><span data-stu-id="f4865-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="f4865-104">Novi račun kreira se pomoću različite vrijednosti PUID</span><span class="sxs-lookup"><span data-stu-id="f4865-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="f4865-105">Kada korisnik pokuša pristupiti zbirci web-mjesta ili svom servisu OneDrive, korisnik ima neispravan PUID.</span><span class="sxs-lookup"><span data-stu-id="f4865-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="f4865-106">Drugi scenarij uključuje sinkronizaciju direktorija s organizacijskom jedinicom Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="f4865-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="f4865-107">Ako su se korisnici već prijavili u SharePoint, a zatim se premještaju u drugi OU i ponovno sinkroniziraju sa sustavom SharePoint, možda će doživjeti taj problem.</span><span class="sxs-lookup"><span data-stu-id="f4865-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="f4865-108">Da biste riješili taj problem, trebali biste vratiti izvorni UPN s koracima u članku, [vratiti korisnika u Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="f4865-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="f4865-109">Ako ne možete vratiti izvornog korisnika, morate ukloniti starog korisnika s web-mjesta OneDrive pomoću ovih koraka, [ukloniti korisnika s popisa korisničkih informacija]().</span><span class="sxs-lookup"><span data-stu-id="f4865-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="f4865-110">Nakon što je to učinjeno, možete provjeriti korisnik ima administratorska prava na OneDrive web-mjesta slijedeći korake za [Dodavanje admin-a za user ' s OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="f4865-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="f4865-111">Dodatne informacije o razinama dozvola potražite u članku, [razumijevanje razina dozvola u sustavu SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="f4865-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
