---
title: Rješavanje problema s porukama pristup odbijen
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3973f5bf584343d3353e7389f22bc727827b5c35
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28280304"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="44c4b-102">Rješavanje problema s porukama pristup odbijen</span><span class="sxs-lookup"><span data-stu-id="44c4b-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="44c4b-p101">Ako netko dobio poruku "Pristup je odbijen" zajedničke mape, administrator zbirke web-mjesta možda imaju omogućen "ograničeni pristup korisnika dozvolu lockdown način." Da biste to isključili:</span><span class="sxs-lookup"><span data-stu-id="44c4b-p101">If someone got an "Access Denied" message to a shared folder, the site collection administrator might have enabled "Limited-access user permission lockdown mode." To turn this off:</span></span> 
  
1. <span data-ttu-id="44c4b-105">Otiđite na web-mjesto, kliknite ikonu postavke i kliknite **Postavke web-mjesta**.</span><span class="sxs-lookup"><span data-stu-id="44c4b-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="44c4b-106">U sekciji **Administracija zbirke web-mjesta**pritisnite **značajke zbirke web-mjesta**.</span><span class="sxs-lookup"><span data-stu-id="44c4b-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="44c4b-107">Uz **način rada lockdown dozvole Ograničeni pristup korisnika**, kliknite **Deaktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="44c4b-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="44c4b-p102">Pristup odbijen poruke mogu se pojaviti za zajedničke mape ako web-mjesto je web-mjesto za objavljivanje. Info, potražite [Pristup odbijen prilikom pristupanja zajedničkoj mapi](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="44c4b-p102">An Access Denied message can also occur for shared folders if the site is a publishing site. For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="44c4b-p103">Ako je netko dobio poruku "Pristup je odbijen" prilikom pokušaja prikaz zahtjeve za pristup, korisnik treba dodati kao administrator zbirke web-mjesta ili član grupe vlasnika web-mjesta. Za dodatne informacije pogledajte [Odbijen pristup zahtjeve za pristup popisu](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="44c4b-p103">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site. For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="44c4b-112">Ako korisnik dobio poruku "Pristup je odbijen" nakon što su uklonjene iz servisa Active Directory lokalno i dodali natrag, pogledajte [Pristup odbijen kada korisnički račun je sinkronizirana Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="44c4b-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

