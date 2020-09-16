---
title: Ažuriranje poslužitelja naziva u vašoj domeni da bi upućivali na Microsoft
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734903"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="64bab-102">Ažuriranje poslužitelja naziva u vašoj domeni da bi upućivali na Microsoft</span><span class="sxs-lookup"><span data-stu-id="64bab-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="64bab-103">Napomena: propagiranje promjena poslužitelja naziva ponekad može potrajati do 48 sati.</span><span class="sxs-lookup"><span data-stu-id="64bab-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="64bab-104">Da biste postavili domenu s Microsoftovim, poslužitelji naziva na registraru moraju biti ažurirani.</span><span class="sxs-lookup"><span data-stu-id="64bab-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="64bab-105">Stvorite ili uredite zapise poslužitelja naziva pri registraru domene.</span><span class="sxs-lookup"><span data-stu-id="64bab-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="64bab-106">Idite na web-mjesto registrara domene i potražite područje u kojemu možete urediti poslužitelje naziva.</span><span class="sxs-lookup"><span data-stu-id="64bab-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="64bab-107">Stvorite ili uredite dva zapisa poslužitelja naziva tako da odgovaraju ovim vrijednostima:</span><span class="sxs-lookup"><span data-stu-id="64bab-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="64bab-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="64bab-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="64bab-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="64bab-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="64bab-110">Spremite promjene.</span><span class="sxs-lookup"><span data-stu-id="64bab-110">Save changes.</span></span>

<span data-ttu-id="64bab-111">Detaljne upute možete pronaći i u ovom članku: [Promjena poslužitelja naziva radi postavljanja microsoftova 365 uz bilo koji registrara domena](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="64bab-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  