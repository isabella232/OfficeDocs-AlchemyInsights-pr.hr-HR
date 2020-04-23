---
title: Ažurirajte poslužitelje naziva domena tako da upućuju na Microsoft
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: b49ca9422f582f906fc6c108c85cc26150474548
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719985"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="bc5b9-102">Ažurirajte poslužitelje naziva domena tako da upućuju na Microsoft</span><span class="sxs-lookup"><span data-stu-id="bc5b9-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="bc5b9-103">Napomena: propagiranje promjena poslužitelja naziva ponekad može potrajati do 48 sati.</span><span class="sxs-lookup"><span data-stu-id="bc5b9-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="bc5b9-104">Da biste postavili domenu s Microsoftom, potrebno je ažurirati poslužitelje naziva kod registrara.</span><span class="sxs-lookup"><span data-stu-id="bc5b9-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="bc5b9-105">Stvorite ili uredite zapise poslužitelja naziva pri registraru domene.</span><span class="sxs-lookup"><span data-stu-id="bc5b9-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="bc5b9-106">Idite na web-mjesto registrara domene i potražite područje u kojemu možete urediti poslužitelje naziva.</span><span class="sxs-lookup"><span data-stu-id="bc5b9-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="bc5b9-107">Stvorite ili uredite dva zapisa poslužitelja naziva tako da odgovaraju ovim vrijednostima:</span><span class="sxs-lookup"><span data-stu-id="bc5b9-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="bc5b9-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="bc5b9-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="bc5b9-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="bc5b9-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="bc5b9-110">Spremite promjene.</span><span class="sxs-lookup"><span data-stu-id="bc5b9-110">Save changes.</span></span>

<span data-ttu-id="bc5b9-111">Detaljne upute potražite u ovom članku: [Promjena poslužitelja naziva za postavljanje sustava Microsoft 365 s bilo kojim registrarom domena](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="bc5b9-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  