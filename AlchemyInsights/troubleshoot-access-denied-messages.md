---
title: Otklanjanje poteškoća s porukama odbijenim pristupom
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 1930edcfd14acc48ea77b66e2793654a3e6332cc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759792"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="0590b-102">Otklanjanje poteškoća s porukama odbijenim pristupom</span><span class="sxs-lookup"><span data-stu-id="0590b-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="0590b-103">Ako je netko u zajedničku mapu u sustavu SharePoint dobio poruku "Pristup je odbijen", administrator zbirke web-mjesta možda je omogućio "Način zaključavanja korisničkih dozvola s ograničenim pristupom".</span><span class="sxs-lookup"><span data-stu-id="0590b-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="0590b-104">Da biste to isključili:</span><span class="sxs-lookup"><span data-stu-id="0590b-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="0590b-105">Pronađite web-mjesto, kliknite ikonu Postavke, a zatim **Postavke web-mjesta**.</span><span class="sxs-lookup"><span data-stu-id="0590b-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="0590b-106">U **odjeljku Administracija zbirke web-mjesta**kliknite **Značajke zbirke web-mjesta**.</span><span class="sxs-lookup"><span data-stu-id="0590b-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="0590b-107">Uz **način zaključavanja dopuštenja korisnika s ograničenim pristupom**kliknite **Deaktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="0590b-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="0590b-108">Poruka odbijenog pristupa može se pojaviti i za zajedničke mape ako je web-mjesto za objavljivanje.</span><span class="sxs-lookup"><span data-stu-id="0590b-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="0590b-109">Dodatne informacije potražite u [odjeljku Pristup je odbijen prilikom pristupa zajedničkoj mapi](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="0590b-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="0590b-110">Ako je netko prilikom pokušaja prikaza zahtjeva za pristup dobio poruku "Pristup je odbijen", korisnika treba dodati kao administrator zbirke web-mjesta ili član grupe Vlasnici za web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="0590b-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="0590b-111">Dodatne informacije potražite [u odjeljku Pristup je odbijen pristupu zahtjevima](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="0590b-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="0590b-112">Ako je korisnik dobio poruku "Pristup je odbijen" nakon što je uklonjen iz lokalnog servisa Active Directory, a zatim ponovno dodan, pročitajte članak [Pristup je odbijen kada se korisnički račun sinkronizira sa sustavom Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="0590b-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

