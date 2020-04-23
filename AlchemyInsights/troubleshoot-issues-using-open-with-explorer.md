---
title: Otklanjanje poteškoća s pomoću značajke Otvori pomoću programa Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: cb26876d93a110b3b0addd7821206215c783f959
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759684"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="41d72-102">Rješavanje problema s otvori pomoću programa Explorer</span><span class="sxs-lookup"><span data-stu-id="41d72-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="41d72-103">Riješite uobičajene probleme s otvaranjem biblioteke dokumenata u sustavu SharePoint ili OneDrive pomoću naredbe **Otvori pomoću programa Explorer:**</span><span class="sxs-lookup"><span data-stu-id="41d72-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="41d72-104">Koristite Internet Explorer 10 ili Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="41d72-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="41d72-105">**Otvoreno s preglednikom Explorer** nije kompatibilno s preglednikom Microsoft Edge, Google Chrome, Firefox i drugima.</span><span class="sxs-lookup"><span data-stu-id="41d72-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="41d72-106">**Otvori s explorerom** onemogućen je u svim preglednicima osim preglednika Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="41d72-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="41d72-107">**Otvoreno pomoću programa Explorer** nije dostupno u modernom doživljaju za biblioteke sustava SharePoint.</span><span class="sxs-lookup"><span data-stu-id="41d72-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="41d72-108">Umjesto toga koristite **Prikaz u eksploreru za datoteke.**</span><span class="sxs-lookup"><span data-stu-id="41d72-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="41d72-109">Odaberite **Prikaz mogućnosti** \> **Prikaz u eksploreru za datoteke**.</span><span class="sxs-lookup"><span data-stu-id="41d72-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="41d72-110">View in File Explorer nije kompatibilan s microsoft edge, Google Chrome, Firefox i drugima.</span><span class="sxs-lookup"><span data-stu-id="41d72-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="41d72-111">**Prikaz u eksploreru za datoteke** dostupan je samo u pregledniku Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="41d72-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="41d72-112">Provjerite je li pokrenut servis WebClient.</span><span class="sxs-lookup"><span data-stu-id="41d72-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="41d72-113">U okvir za pretraživanje u sustavu Windows upišite pokreni, odaberite aplikaciju Pokreni radnu površinu, upišite services.msc, a zatim pritisnite tipku Enter.</span><span class="sxs-lookup"><span data-stu-id="41d72-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="41d72-114">Pomaknite se prema dolje do servisa WebClient i provjerite prikazuje li se u stupcu **Status** "Running".</span><span class="sxs-lookup"><span data-stu-id="41d72-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="41d72-115">Ako se to ne događa, dvokliknite servis, kliknite **Start**, a zatim **U redu**.</span><span class="sxs-lookup"><span data-stu-id="41d72-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="41d72-116">(Možda ćete prvo morati omogućiti uslugu tako da u okviru **Vrsta pokretanja** odaberete **Ručno** ili **Automatsko.)**</span><span class="sxs-lookup"><span data-stu-id="41d72-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="41d72-117">Otvaranje biblioteke u eksploreru za datoteke praktično je ako morate jednom kopirati ili premjestiti više datoteka i mapa, ali ako želite redovito raditi u biblioteci, preporučujemo da je sinkronizirate.</span><span class="sxs-lookup"><span data-stu-id="41d72-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="41d72-118">Da biste otklonili poteškoće s otvaranjem u eksploreru za datoteke, [pročitajte članak Otvori u programu Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="41d72-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="41d72-119">Informacije o postavljanju sinkronizacije potražite u [odjeljku Sinkronizacija datoteka sustava SharePoint s novim klijentom za sinkronizaciju sa servisom OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="41d72-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="41d72-120">Dodatne informacije potražite u članku [Korištenje naredbe "Otvori pomoću programa Explorer" za otklanjanje poteškoća u sustavu SharePoint Online.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)</span><span class="sxs-lookup"><span data-stu-id="41d72-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

