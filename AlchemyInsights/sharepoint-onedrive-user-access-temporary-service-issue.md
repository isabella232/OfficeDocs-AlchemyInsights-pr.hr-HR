---
title: Problemi performanse-SharePoint ili OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 880b2bdd7b74f4365bcbff73a709d42e72be0e3a
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36535147"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="98671-102">SharePoint ili OneDrive spora, nedostupni ili nedostupna za više korisnika</span><span class="sxs-lookup"><span data-stu-id="98671-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="98671-103">Ako OneDrive ili SharePoint web-mjesta nije dostupno više korisnike koji su prethodno imali pristup, možda postoji problem privremeni servisa.</span><span class="sxs-lookup"><span data-stu-id="98671-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="98671-104">[Provjerite servisa stanja nadzorne ploče](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="98671-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="98671-105">**Dodajte i licence korisnika**</span><span class="sxs-lookup"><span data-stu-id="98671-105">**Add and license the user**</span></span>

<span data-ttu-id="98671-106">Provjerite koje ste [dodijelili licence korisnicima u Office 365 poslovne](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="98671-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


<span data-ttu-id="98671-107">**Dodijelite dozvole**</span><span class="sxs-lookup"><span data-stu-id="98671-107">**Assign Permissions**</span></span>

<span data-ttu-id="98671-108">Ako korisnik je dodijeljena licenca Sharepoint i još uvijek primanje uskraćen pristup, provjerite je li imati [odgovarajuću razinu dozvole](https://docs.microsoft.com/sharepoint/understanding-permission-levels) dodijeljene.</span><span class="sxs-lookup"><span data-stu-id="98671-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="98671-109">**Razmislite o korištenju značajke zahtjeva pristupa**</span><span class="sxs-lookup"><span data-stu-id="98671-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="98671-110">[Značajka zahtjev access](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) omogućuje korisnicima zatražili pristup sadržaju trenutno nemaju dozvolu za prikaz.</span><span class="sxs-lookup"><span data-stu-id="98671-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="98671-111">**Dopusti Prilagođena skripta može uzrokovati pristup odbijen problemi**</span><span class="sxs-lookup"><span data-stu-id="98671-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="98671-112">Postoje određene scenarije gdje značajka *Dopusti prilagođene skripte* možda biti dosljedna odbijen pristup.</span><span class="sxs-lookup"><span data-stu-id="98671-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="98671-113">Za popis utječe na sljedeće značajke, Sigurnosna razmatranja i onemogućiti značajku.</span><span class="sxs-lookup"><span data-stu-id="98671-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="98671-114">Posjetite [Dopusti ili spriječiti prilagođene skripte](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="98671-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

