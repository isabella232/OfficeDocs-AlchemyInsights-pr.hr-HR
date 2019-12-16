---
title: Otklanjanje poteškoća s porukama odbijeno za pristup
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 05d12aee49b449e8a29e84021b41298fb9983859
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050697"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="7d196-102">Otklanjanje poteškoća s porukama odbijeno za pristup</span><span class="sxs-lookup"><span data-stu-id="7d196-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="7d196-103">Ako je netko dobio poruku "pristup je odbijen" u zajedničku mapu u sustavu SharePoint, administrator zbirke web-mjesta možda je omogućio način zaključavanja dopuštenja korisnika s ograničenim pristupom.</span><span class="sxs-lookup"><span data-stu-id="7d196-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="7d196-104">Da biste to isključili:</span><span class="sxs-lookup"><span data-stu-id="7d196-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="7d196-105">Prijeđite na web-mjesto, kliknite ikonu Postavke, a zatim kliknite **Postavke web-mjesta**.</span><span class="sxs-lookup"><span data-stu-id="7d196-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="7d196-106">U odjeljku **Administracija zbirke web-** mjesta kliknite **značajke zbirke web-mjesta**.</span><span class="sxs-lookup"><span data-stu-id="7d196-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="7d196-107">Pored **načina zaključavanja dopuštenja korisnika s ograničenim pristupom**kliknite **Deaktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="7d196-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="7d196-108">Poruka odbijeni pristup može se pojaviti i za zajedničke mape ako je web-mjesto objavljivanje.</span><span class="sxs-lookup"><span data-stu-id="7d196-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="7d196-109">Informacije potražite u [programu pristup odbijen prilikom pristupa zajedničkoj mapi](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="7d196-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="7d196-110">Ako je netko dobio poruku "pristup je odbijen" prilikom pokušaja prikaza zahtjeva za pristup, korisnik mora biti dodan kao administrator zbirke web-mjesta ili član grupe vlasnici za web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="7d196-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="7d196-111">Dodatne informacije potražite u okviru [popis zahtjeva za pristup koji je odbijen](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="7d196-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="7d196-112">Ako korisnik dobio poruku "pristup je odbijen" nakon što su uklonjeni iz Active Directory lokalno i zatim dodan natrag, pogledajte [pristup odbijen kada korisnički račun sinkroniziran na Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="7d196-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

