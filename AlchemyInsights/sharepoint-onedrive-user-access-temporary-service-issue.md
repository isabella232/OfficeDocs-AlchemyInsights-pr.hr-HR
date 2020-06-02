---
title: Problemi s performansama- SharePoint ili OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 2dc0cd5f1641298853443d364eb9434ec1d9cd5a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511140"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="e12c6-102">Spor, nedostupan ili nedostupan za više korisnika sustava SharePoint ili OneDrive</span><span class="sxs-lookup"><span data-stu-id="e12c6-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="e12c6-103">Ako web-mjesto servisa OneDrive ili SharePoint nije dostupno većem broju korisnika koji su prethodno imali pristup, možda postoji problem s privremenim servisom.</span><span class="sxs-lookup"><span data-stu-id="e12c6-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="e12c6-104">[Provjerite nadzornu ploču stanja servisa](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="e12c6-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="e12c6-105">**Dodavanje i licenciranje korisnika**</span><span class="sxs-lookup"><span data-stu-id="e12c6-105">**Add and license the user**</span></span>

<span data-ttu-id="e12c6-106">Provjerite dodijelite li [licence korisnicima u sustavu Microsoft 365 za tvrtke](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="e12c6-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="e12c6-107">**Dodijeli dozvole**</span><span class="sxs-lookup"><span data-stu-id="e12c6-107">**Assign Permissions**</span></span>

<span data-ttu-id="e12c6-108">Ako je korisniku dodijeljena licenca za Sharepoint i još uvijek prima poruku odbijenog pristupa, provjerite je li dodijeljena [odgovarajuća razina dozvole.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)</span><span class="sxs-lookup"><span data-stu-id="e12c6-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="e12c6-109">**Razmislite o korištenju značajke zahtjeva za pristup**</span><span class="sxs-lookup"><span data-stu-id="e12c6-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="e12c6-110">[Značajka zahtjeva za pristup](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) omogućuje korisnicima da zatraže pristup sadržaju za koji trenutno nemaju dozvolu za prikaz.</span><span class="sxs-lookup"><span data-stu-id="e12c6-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="e12c6-111">**Dopusti prilagođenu skriptu može uzrokovati probleme s odbijenim pristupom**</span><span class="sxs-lookup"><span data-stu-id="e12c6-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="e12c6-112">Postoje određeni scenariji u kojima značajka *Dopusti prilagođenu skriptu* možda predstavlja pristup odbijen.</span><span class="sxs-lookup"><span data-stu-id="e12c6-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="e12c6-113">Za popis značajki na koje se to odnosi, sigurnosna razmatranja i mogućnost onemogućivanja značajke.</span><span class="sxs-lookup"><span data-stu-id="e12c6-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="e12c6-114">Posjetite [Dopusti ili spriječite prilagođenu skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="e12c6-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

