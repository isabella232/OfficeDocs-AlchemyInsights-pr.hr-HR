---
title: Problemi s performansama – SharePoint ili OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771236"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="ebd8d-102">SharePoint ili OneDrive spori, nedostupni ili nedostupni za više korisnika</span><span class="sxs-lookup"><span data-stu-id="ebd8d-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="ebd8d-103">Ako web-mjesto servisa OneDrive ili SharePoint nije dostupno većem broju korisnika koji su prethodno imali pristup, možda postoji privremeni problem s servisom.</span><span class="sxs-lookup"><span data-stu-id="ebd8d-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="ebd8d-104">[Provjerite nadzornu ploču zdravstvenog stanja servisa](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="ebd8d-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="ebd8d-105">**Dodavanje i licenciranje korisnika**</span><span class="sxs-lookup"><span data-stu-id="ebd8d-105">**Add and license the user**</span></span>

<span data-ttu-id="ebd8d-106">Provjerite jeste li [korisnicima dodijelili licence u programu Microsoft 365 za tvrtke](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="ebd8d-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="ebd8d-107">**Dodjela dozvola**</span><span class="sxs-lookup"><span data-stu-id="ebd8d-107">**Assign Permissions**</span></span>

<span data-ttu-id="ebd8d-108">Ako je korisniku dodijeljena licenca za SharePoint i još uvijek dobiva poruku o uskraćenom pristupu, provjerite ima li dodijeljenu [odgovarajuću razinu dozvola](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .</span><span class="sxs-lookup"><span data-stu-id="ebd8d-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="ebd8d-109">**Razmislite o korištenju značajke zahtjeva za Access**</span><span class="sxs-lookup"><span data-stu-id="ebd8d-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="ebd8d-110">[Značajka zahtjeva za pristup](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) omogućuje korisnicima da zatraže pristup sadržaju koji trenutno nemaju dozvolu za pregled.</span><span class="sxs-lookup"><span data-stu-id="ebd8d-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="ebd8d-111">**Omogućivanje prilagođene skripte može uzrokovati probleme s uskraćanjem programa Access**</span><span class="sxs-lookup"><span data-stu-id="ebd8d-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="ebd8d-112">Postoje određeni scenariji u kojima značajka *Dopusti prilagođenu skriptu* može prikazati zabranjen pristup.</span><span class="sxs-lookup"><span data-stu-id="ebd8d-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="ebd8d-113">Popis značajki koje su zahvaćene sigurnosnim razmišljanjima i mogućnost onemogućivanja značajke.</span><span class="sxs-lookup"><span data-stu-id="ebd8d-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="ebd8d-114">Posjetite [Dopusti ili spriječi prilagođenu skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="ebd8d-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

