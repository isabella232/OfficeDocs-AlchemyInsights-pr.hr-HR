---
title: Otklanjanje poteškoća s otvaranjem programa Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659050"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="5bb16-102">Rješavanje problema s otvaranjem programa Explorer</span><span class="sxs-lookup"><span data-stu-id="5bb16-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="5bb16-103">Riješite česte probleme s otvaranjem biblioteke dokumenata u sustavu SharePoint ili servisa OneDrive pomoću naredbe **Otvori pomoću programa Explorer** :</span><span class="sxs-lookup"><span data-stu-id="5bb16-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="5bb16-104">Koristite Internet Explorer 10 ili Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="5bb16-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="5bb16-105">**OpenBSD sa istraživač** nije kompatibilan sa Microsoft Edge, Google Chrome, Firefox i drugi.</span><span class="sxs-lookup"><span data-stu-id="5bb16-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="5bb16-106">**Otvaranje programom Explorer** onemogućeno je u svim preglednicima osim u pregledniku Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="5bb16-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="5bb16-107">**Otvaranje programom Explorer** nije dostupno u modernom iskustvu za biblioteke sustava SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5bb16-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="5bb16-108">Umjesto toga koristite **Prikaz u eksploreru za datoteke** .</span><span class="sxs-lookup"><span data-stu-id="5bb16-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="5bb16-109">Odaberite prikaz **mogućnosti prikaza** \> **u eksploreru za datoteke**.</span><span class="sxs-lookup"><span data-stu-id="5bb16-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="5bb16-110">Prikaz u eksploreru za datoteke nije kompatibilan s programom Microsoft Edge, Google Chrome, Firefox i drugi.</span><span class="sxs-lookup"><span data-stu-id="5bb16-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="5bb16-111">**Prikaz u eksploreru za datoteke** dostupan samo u pregledniku Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="5bb16-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="5bb16-112">Provjerite je li servis WebClient pokrenut.</span><span class="sxs-lookup"><span data-stu-id="5bb16-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="5bb16-113">U okvir za pretraživanje sustava Windows upišite Pokreni pa odaberite Pokreni aplikaciju za stolna računala, upišite Services. msc, a zatim pritisnite ENTER.</span><span class="sxs-lookup"><span data-stu-id="5bb16-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="5bb16-114">Pomaknite se prema dolje do web-klijentskog servisa i provjerite prikazuje li stupac **status** "pokrenut".</span><span class="sxs-lookup"><span data-stu-id="5bb16-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="5bb16-115">Ako to ne učinite, dvokliknite servis, zatim kliknite **Start**, a potom **u redu**.</span><span class="sxs-lookup"><span data-stu-id="5bb16-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="5bb16-116">(Možda ćete morati najprije omogućiti servis tako da odaberete **ručno** ili **Automatsko** u okviru **Vrsta pokretanja** .)</span><span class="sxs-lookup"><span data-stu-id="5bb16-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="5bb16-117">Otvaranje biblioteke u eksploreru za datoteke korisno je ako jednom morate kopirati ili premještati više datoteka i mapa, no ako želite redovito raditi u biblioteci, preporučujemo da je sinkronizirate.</span><span class="sxs-lookup"><span data-stu-id="5bb16-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="5bb16-118">Upute za otklanjanje poteškoća u eksploreru za datoteke potražite [u članku otvaranje u programu Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="5bb16-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="5bb16-119">Informacije o postavljanju sinkronizacije potražite [u članku sinkronizacija datoteka sustava SharePoint s novim klijentom za sinkronizaciju servisa OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="5bb16-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="5bb16-120">[Upute za otklanjanje poteškoća u sustavu SharePoint Online potražite u članku kako koristiti naredbu "Otvori sa eksplorerom" da biste](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) saznali više o problemima.</span><span class="sxs-lookup"><span data-stu-id="5bb16-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

