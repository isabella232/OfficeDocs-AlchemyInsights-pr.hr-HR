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
ms.openlocfilehash: 23d49c734148739ede0d5e5b53430a42b606c831
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742162"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="7e22c-102">Ažuriranje poslužitelja naziva u vašoj domeni na Office 365</span><span class="sxs-lookup"><span data-stu-id="7e22c-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="7e22c-103">Napomena: propagiranje promjena poslužitelja naziva ponekad može potrajati do 48 sati.</span><span class="sxs-lookup"><span data-stu-id="7e22c-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="7e22c-104">Da biste postavili domenu u sustavu Office 365, moraju se ažurirati poslužitelji naziva pri registraru.</span><span class="sxs-lookup"><span data-stu-id="7e22c-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="7e22c-105">Stvorite ili uredite zapise poslužitelja naziva pri registraru domene.</span><span class="sxs-lookup"><span data-stu-id="7e22c-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="7e22c-106">Idite na web-mjesto registrara domene i potražite područje u kojemu možete urediti poslužitelje naziva.</span><span class="sxs-lookup"><span data-stu-id="7e22c-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="7e22c-107">Stvorite ili uredite dva zapisa poslužitelja naziva tako da odgovaraju ovim vrijednostima:</span><span class="sxs-lookup"><span data-stu-id="7e22c-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="7e22c-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="7e22c-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="7e22c-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="7e22c-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="7e22c-110">Spremite promjene.</span><span class="sxs-lookup"><span data-stu-id="7e22c-110">Save changes.</span></span>

<span data-ttu-id="7e22c-111">Detaljne upute možete pronaći i u ovom članku: [Promjena poslužitelja naziva radi postavljanja sustava Office 365 pri registraru domene](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="7e22c-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  