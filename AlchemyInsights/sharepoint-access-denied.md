---
title: Otklanjanje poteškoća s zabranom pristupa porukama
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: f49cfc50142b3d98a5f431a38e9a943eb5624523
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691675"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="b87b1-102">Otklanjanje poteškoća s zabranom pristupa porukama</span><span class="sxs-lookup"><span data-stu-id="b87b1-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="b87b1-103">Ako prilikom pokušaja pregledavanja web-mjesta sustava SharePoint Online primate poruku o uskraćenog pristupa, pročitajte članak u nastavku.</span><span class="sxs-lookup"><span data-stu-id="b87b1-103">If you are receiving an access denied message when attempting to browse a Sharepoint Online site, please see the below articles.</span></span>

<span data-ttu-id="b87b1-104">**Dodavanje i licenciranje korisnika**</span><span class="sxs-lookup"><span data-stu-id="b87b1-104">**Add and License the user**</span></span>

<span data-ttu-id="b87b1-105">Provjerite jeste li [korisnicima dodijelili licence u programu Microsoft 365 za tvrtke](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="b87b1-105">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>

<span data-ttu-id="b87b1-106">**Dodjela dozvola**</span><span class="sxs-lookup"><span data-stu-id="b87b1-106">**Assign Permissions**</span></span>

<span data-ttu-id="b87b1-107">Ako je korisniku dodijeljena licenca za SharePoint i još uvijek dobiva poruku o uskraćenom pristupu, provjerite ima li [dodijeljenu odgovarajuću razinu dozvola](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="b87b1-107">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level assigned](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>

<span data-ttu-id="b87b1-108">**Razmislite o korištenju značajke zahtjeva za Access**</span><span class="sxs-lookup"><span data-stu-id="b87b1-108">**Consider using the access request feature**</span></span>

<span data-ttu-id="b87b1-109">Značajka [zahtjeva za pristup](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) omogućuje korisnicima da zatraže pristup sadržaju koji trenutno nemaju dozvolu za pregled.</span><span class="sxs-lookup"><span data-stu-id="b87b1-109">The [access request](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) feature allows people to request access to content that they do not currently have permission to see.</span></span> 

<span data-ttu-id="b87b1-110">**Omogućivanje prilagođene skripte može uzrokovati probleme s uskraćanjem programa Access**</span><span class="sxs-lookup"><span data-stu-id="b87b1-110">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="b87b1-111">Postoje određeni scenariji u kojima značajka "Dopusti prilagođenu skriptu" možda predstavlja zabranjen pristup.</span><span class="sxs-lookup"><span data-stu-id="b87b1-111">There are certain scenarios where the "Allow custom script" feature may be presenting an access denied.</span></span> <span data-ttu-id="b87b1-112">Popis značajki koje su zahvaćene sigurnosnim razmišljanjima i mogućnost onemogućivanja značajke.</span><span class="sxs-lookup"><span data-stu-id="b87b1-112">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="b87b1-113">Posjetite, [omogućite ili onemogućite prilagođenu skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="b87b1-113">Please visit , [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span></span>

<span data-ttu-id="b87b1-114">Pažnja: Ako web-mjesto servisa OneDrive ili SharePoint nije dostupno većem broju korisnika koji su prethodno imali pristup, možda postoji privremeni problem s servisom.</span><span class="sxs-lookup"><span data-stu-id="b87b1-114">Note: If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="b87b1-115">[Provjerite nadzornu ploču zdravstvenog stanja servisa](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="b87b1-115">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


  

