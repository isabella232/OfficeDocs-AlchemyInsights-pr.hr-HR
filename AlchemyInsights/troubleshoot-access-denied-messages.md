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
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704886"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="370b3-102">Otklanjanje poteškoća s zabranom pristupa porukama</span><span class="sxs-lookup"><span data-stu-id="370b3-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="370b3-103">Ako je netko dobio poruku "pristup je odbijen" u zajedničku mapu u sustavu SharePoint, administrator zbirke web-mjesta mogao je omogućiti "ograničen pristup korisniku dozvola za zaključavanje."</span><span class="sxs-lookup"><span data-stu-id="370b3-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="370b3-104">Da biste isključili ovu stavku, učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="370b3-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="370b3-105">Dođite do web-mjesta, kliknite ikonu Postavke, a zatim **Postavke web-mjesta**.</span><span class="sxs-lookup"><span data-stu-id="370b3-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="370b3-106">U odjeljku **Administracija zbirke web-mjesta** kliknite **značajke zbirke web-mjesta**.</span><span class="sxs-lookup"><span data-stu-id="370b3-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="370b3-107">Pokraj funkcije **zaključavanje korisničkih dozvola za ograničen pristup** kliknite **Deaktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="370b3-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="370b3-108">Ako je web-mjesto web-mjesto za objavljivanje, može se pojaviti i poruka o uskraćenog pristupa.</span><span class="sxs-lookup"><span data-stu-id="370b3-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="370b3-109">Informacije potražite u članku [zabranjen pristup prilikom pristupanja zajedničkoj mapi](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span><span class="sxs-lookup"><span data-stu-id="370b3-109">For info, see [Access Denied when accessing a shared folder](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span></span>
  
<span data-ttu-id="370b3-110">Ako je netko dobio poruku "pristup je odbijen" prilikom pokušaja pregledavanja zahtjeva za pristup, korisnik mora biti dodan kao administrator zbirke web-mjesta ili član grupe vlasnici za web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="370b3-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="370b3-111">Dodatne informacije potražite u članku [zabranjen pristup popisu zahtjeva za pristup](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="370b3-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="370b3-112">Ako je korisnik dobio poruku "pristup je odbijen" nakon uklanjanja iz lokalnih servisa Active Directory, a zatim dodan natrag, pročitajte članak [zabranjen je kada se korisnički račun sinkronizira sa sustavom Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="370b3-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

