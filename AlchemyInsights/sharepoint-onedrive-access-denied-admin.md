---
title: Rješavanje problema s porukama pristup odbijen
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c204f1889e03886fdfd3d1c760a4a2beb82b0836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760333"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="e60f9-102">Pristup odbijen poruke u centru Sharepoint OneDrive Admin rješavanje problema</span><span class="sxs-lookup"><span data-stu-id="e60f9-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="e60f9-103">Ako primate uskraćen prilikom pokušaja Pregledaj centar Admin Sharepoint OneDrive pristup, provjerite je li taj [dodeljivanje licence korisniku](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="e60f9-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="e60f9-104">Ako korisnik ima licencu, također provjerite su [dodijeljeni ulogu administratora](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) koji može pristupiti admin centre.</span><span class="sxs-lookup"><span data-stu-id="e60f9-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="e60f9-105">Ovaj se problem može pojaviti kada korisnik izbrisana i stvorena ponovo s istom korisniku glavni naziv (UPN).</span><span class="sxs-lookup"><span data-stu-id="e60f9-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="e60f9-106">Novi račun stvorena pomoću različite PUID (jedinstveni ID Passport) vrijednost.</span><span class="sxs-lookup"><span data-stu-id="e60f9-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="e60f9-107">Kada korisnik pokuša pristupiti zbirci web-mjesta ili njihovim OneDrive, korisnik ima neispravan PUID.</span><span class="sxs-lookup"><span data-stu-id="e60f9-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="e60f9-108">Drugi scenarij uključuje imenik sinkronizacije s u Active Directory organizacijsku jedinicu (OU).</span><span class="sxs-lookup"><span data-stu-id="e60f9-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="e60f9-109">Ako korisnici imaju već prijavljeni u SharePoint, a zatim su premještene različite OU i resynced SharePoint, može doći taj problem.</span><span class="sxs-lookup"><span data-stu-id="e60f9-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="e60f9-110">Da biste riješili taj problem, trebali biste vratiti izvornu UPN s korake u članku [Vraćanje korisnika u Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="e60f9-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="e60f9-111">Napomena: Ako centar za OneDrive ili SharePoint administraciju nije dostupno više korisnike koji su prethodno imali pristup, možda postoji problem privremeni servisa.</span><span class="sxs-lookup"><span data-stu-id="e60f9-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="e60f9-112">[Provjerite servisa stanja nadzorne ploče](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="e60f9-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


