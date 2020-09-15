---
title: Otklanjanje poteškoća s zabranom pristupa porukama web-mjesta servisa OneDrive za tvrtke
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670608"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="a51c6-102">Otklanjanje poteškoća s zabranom pristupa porukama web-mjesta servisa OneDrive za tvrtke</span><span class="sxs-lookup"><span data-stu-id="a51c6-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="a51c6-103">Taj se problem najčešće pojavljuje kada je korisnik izbrisan i ponovno stvoren pomoću istog glavnog naziva korisnika (UPN).</span><span class="sxs-lookup"><span data-stu-id="a51c6-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="a51c6-104">Novi se račun stvara pomoću različite vrijednosti za PUID (jedinstveni ID putovnice).</span><span class="sxs-lookup"><span data-stu-id="a51c6-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="a51c6-105">Kada korisnik pokuša pristupiti zbirci web-mjesta ili njihovom servisu OneDrive, korisnik ima pogrešan PUID.</span><span class="sxs-lookup"><span data-stu-id="a51c6-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="a51c6-106">Drugi scenarij obuhvaća sinkronizaciju direktorija s organizacijom Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="a51c6-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="a51c6-107">Ako su se korisnici već prijavili u SharePoint, a zatim se premještaju u drugi OU i ponovno sinkroniziraju sa sustavom SharePoint, možda će doživjeti taj problem.</span><span class="sxs-lookup"><span data-stu-id="a51c6-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="a51c6-108">Da biste riješili taj problem, trebali biste vratiti originalni UPN pomoću koraka u članku, [vratiti korisnika u programu Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="a51c6-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="a51c6-109">Ako ne možete vratiti izvornog korisnika, trebali biste ukloniti starog korisnika s web-mjesta servisa OneDrive pomoću ovih koraka, [ukloniti korisnika s popisa korisnički info]().</span><span class="sxs-lookup"><span data-stu-id="a51c6-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="a51c6-110">Kada je to gotovo, možete potvrditi da korisnik ima administratorska prava na web-mjesto servisa OneDrive prateći korake za [Dodavanje administratora za korisnički OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles) .</span><span class="sxs-lookup"><span data-stu-id="a51c6-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="a51c6-111">Dodatne informacije o razinama dozvola potražite u članku [razumijevanje razina dozvola u sustavu SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="a51c6-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
