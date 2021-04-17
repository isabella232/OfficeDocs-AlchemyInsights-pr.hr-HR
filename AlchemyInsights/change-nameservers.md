---
title: Promjena poslužitelja naziva
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 67680a6fa514d31ccb88cc8691a199cd1f58a402
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818604"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="ed3c3-102">Ažuriranje poslužitelja naziva u vašoj domeni da bi upućivali na Microsoft</span><span class="sxs-lookup"><span data-stu-id="ed3c3-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="ed3c3-103">Napomena: propagiranje promjena poslužitelja naziva ponekad može potrajati do 48 sati.</span><span class="sxs-lookup"><span data-stu-id="ed3c3-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="ed3c3-104">Da biste postavili domenu u okruženju Microsoft 365, moraju se ažurirati poslužitelji naziva pri registraru.</span><span class="sxs-lookup"><span data-stu-id="ed3c3-104">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="ed3c3-105">Stvorite ili uredite zapise poslužitelja naziva pri registraru domene.</span><span class="sxs-lookup"><span data-stu-id="ed3c3-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="ed3c3-106">Idite na web-mjesto registrara domene i potražite područje u kojemu možete urediti poslužitelje naziva.</span><span class="sxs-lookup"><span data-stu-id="ed3c3-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="ed3c3-107">Stvorite ili uredite dva zapisa poslužitelja naziva tako da odgovaraju ovim vrijednostima:</span><span class="sxs-lookup"><span data-stu-id="ed3c3-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="ed3c3-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="ed3c3-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="ed3c3-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="ed3c3-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="ed3c3-110">Spremite promjene.</span><span class="sxs-lookup"><span data-stu-id="ed3c3-110">Save changes.</span></span>

<span data-ttu-id="ed3c3-111">Detaljne upute možete pronaći i u ovom članku: [Promjena poslužitelja naziva pri registraru domene](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="ed3c3-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  