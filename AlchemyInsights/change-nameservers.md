---
title: Promjena poslužitelja naziva
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: f295e0d7872a13cf47e386343b159e51bc0504de
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508080"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="4df69-102">Ažuriranje poslužitelja naziva u vašoj domeni da bi upućivali na Microsoft</span><span class="sxs-lookup"><span data-stu-id="4df69-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="4df69-103">Napomena: propagiranje promjena poslužitelja naziva ponekad može potrajati do 48 sati.</span><span class="sxs-lookup"><span data-stu-id="4df69-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="4df69-104">Da biste postavili domenu u okruženju Microsoft 365, moraju se ažurirati poslužitelji naziva pri registraru.</span><span class="sxs-lookup"><span data-stu-id="4df69-104">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="4df69-105">Stvorite ili uredite zapise poslužitelja naziva pri registraru domene.</span><span class="sxs-lookup"><span data-stu-id="4df69-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="4df69-106">Idite na web-mjesto registrara domene i potražite područje u kojemu možete urediti poslužitelje naziva.</span><span class="sxs-lookup"><span data-stu-id="4df69-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="4df69-107">Stvorite ili uredite dva zapisa poslužitelja naziva tako da odgovaraju ovim vrijednostima:</span><span class="sxs-lookup"><span data-stu-id="4df69-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="4df69-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="4df69-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="4df69-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="4df69-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="4df69-110">Spremite promjene.</span><span class="sxs-lookup"><span data-stu-id="4df69-110">Save changes.</span></span>

<span data-ttu-id="4df69-111">Detaljne upute možete pronaći i u ovom članku: [Promjena poslužitelja naziva pri registraru domene](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="4df69-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  