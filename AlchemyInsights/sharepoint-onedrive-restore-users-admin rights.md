---
title: Daj korisnicima pristup SharePoint i OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a689769dab24e12832ddc0937bc5ddc3d71dbee3
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34759248"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="cd6af-102">Daj korisnicima pristup SharePoint i OneDrive</span><span class="sxs-lookup"><span data-stu-id="cd6af-102">Give users access to SharePoint and OneDrive</span></span>

<span data-ttu-id="cd6af-103">Problem se najčešće pojavljuje kada korisnik izbrisana i stvorena ponovo s istom korisniku glavni naziv (UPN).</span><span class="sxs-lookup"><span data-stu-id="cd6af-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="cd6af-104">Novi račun stvorena pomoću različite PUID (jedinstveni ID Passport) vrijednost.</span><span class="sxs-lookup"><span data-stu-id="cd6af-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="cd6af-105">Kada korisnik pokuša pristupiti zbirci web-mjesta ili njihovim OneDrive, korisnik ima neispravan PUID.</span><span class="sxs-lookup"><span data-stu-id="cd6af-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="cd6af-106">Drugi scenarij uključuje imenik sinkronizacije s u Active Directory organizacijsku jedinicu (OU).</span><span class="sxs-lookup"><span data-stu-id="cd6af-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="cd6af-107">Ako korisnici imaju već prijavljeni u SharePoint, a zatim su premještene različite OU i resynced SharePoint, može doći taj problem.</span><span class="sxs-lookup"><span data-stu-id="cd6af-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="cd6af-108">Da biste riješili ovaj problem treba vratiti izvornu UPN s korake u članku[Vraćanje korisnika u Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="cd6af-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="cd6af-109">Nakon što je napravljen, možete provjeriti korisnik ima prava administracije web-mjesta OneDrive slijedeći korake za [Dodavanje admin's za korisnika OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="cd6af-109">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="cd6af-110">Dodatne informacije o razinama dozvola potražite u članku [Razumijevanje razine dozvola u programu SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="cd6af-110">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
