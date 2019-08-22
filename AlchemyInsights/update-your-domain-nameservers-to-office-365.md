---
title: Ažuriranje poslužitelja naziva u vašoj domeni na Office 365
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 2447a3300782204b32d3c47325e1e987f6168be7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506039"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="8a6c9-102">Ažuriranje poslužitelja naziva u vašoj domeni na Office 365</span><span class="sxs-lookup"><span data-stu-id="8a6c9-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="8a6c9-103">Napomena: propagiranje promjena poslužitelja naziva ponekad može potrajati do 48 sati.</span><span class="sxs-lookup"><span data-stu-id="8a6c9-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="8a6c9-104">Da biste postavili domenu u sustavu Office 365, moraju se ažurirati poslužitelji naziva pri registraru.</span><span class="sxs-lookup"><span data-stu-id="8a6c9-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="8a6c9-105">Stvorite ili uredite zapise poslužitelja naziva pri registraru domene.</span><span class="sxs-lookup"><span data-stu-id="8a6c9-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="8a6c9-106">Idite na web-mjesto registrara domene i potražite područje u kojemu možete urediti poslužitelje naziva.</span><span class="sxs-lookup"><span data-stu-id="8a6c9-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="8a6c9-107">Stvorite ili uredite dva zapisa poslužitelja naziva tako da odgovaraju ovim vrijednostima:</span><span class="sxs-lookup"><span data-stu-id="8a6c9-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="8a6c9-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="8a6c9-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="8a6c9-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="8a6c9-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="8a6c9-110">Spremite promjene.</span><span class="sxs-lookup"><span data-stu-id="8a6c9-110">Save changes.</span></span>

<span data-ttu-id="8a6c9-111">Detaljne upute možete pronaći i u ovom članku: [Promjena poslužitelja naziva radi postavljanja sustava Office 365 pri registraru domene](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="8a6c9-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  