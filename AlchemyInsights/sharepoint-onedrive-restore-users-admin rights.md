---
title: Otklanjanje poteškoća s pristupom odbijenim porukama na web-mjestima servisa OneDrive za tvrtke
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a83936acf969926c113b28ceb22b006cdb96e2b4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692793"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="778f6-102">Otklanjanje poteškoća s pristupom odbijenim porukama na web-mjestima servisa OneDrive za tvrtke</span><span class="sxs-lookup"><span data-stu-id="778f6-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="778f6-103">Taj se problem najčešće pojavljuje kada se korisnik izbriše i ponovno stvori s istim korisničkim glavnim nazivom (UPN).</span><span class="sxs-lookup"><span data-stu-id="778f6-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="778f6-104">Novi račun stvara se pomoću različite VRIJEDNOSTI PUID (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="778f6-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="778f6-105">Kada korisnik pokuša pristupiti zbirci web-mjesta ili na servisu OneDrive, korisnik ima pogrešan PUID.</span><span class="sxs-lookup"><span data-stu-id="778f6-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="778f6-106">Drugi scenarij uključuje sinkronizaciju direktorija s organizacijskom jedinicom servisa Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="778f6-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="778f6-107">Ako su se korisnici već prijavili u SharePoint, a zatim se premještaju u drugi OU i ponovno sinkroniziraju sa sustavom SharePoint, mogu se pojaviti taj problem.</span><span class="sxs-lookup"><span data-stu-id="778f6-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="778f6-108">Da biste riješili taj problem, trebali biste vratiti izvorni UPN s koracima iz članka, [Vraćanje korisnika u microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="778f6-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="778f6-109">Ako ne možete vratiti izvornog korisnika, trebali biste ukloniti starog korisnika s web-mjesta servisa OneDrive pomoću ovih [koraka, uklonite korisnika s popisa korisničkih podataka]().</span><span class="sxs-lookup"><span data-stu-id="778f6-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="778f6-110">Nakon toga možete provjeriti ima li korisnik administratorska prava na web-mjesto servisa OneDrive slijedeći korake za [dodavanje administratora za web-pogon servisa OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles) korisnika</span><span class="sxs-lookup"><span data-stu-id="778f6-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="778f6-111">Dodatne informacije o razinama dozvola potražite u članku [Objašnjenje razina dozvola u sustavu SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="778f6-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
