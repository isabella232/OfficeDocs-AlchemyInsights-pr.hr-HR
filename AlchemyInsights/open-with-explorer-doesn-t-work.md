---
title: Otvori pomoću programa Explorer ne funkcionira
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713026"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="c005f-102">Otvaranje pomoću programa Explorer ne funkcionira</span><span class="sxs-lookup"><span data-stu-id="c005f-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="c005f-103">Ako **otvori pomoću programa Explorer** ili Prikaz u **eksploreru za datoteke** ne funkcionira, provjerite je li servis WebClient postavljen na **Pokrenut** slijedeći korake u nastavku.</span><span class="sxs-lookup"><span data-stu-id="c005f-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="c005f-104">Na primjer, otvaranje biblioteke sustava SharePoint ili OneDrive može potrajati dok servis nije pokrenut.</span><span class="sxs-lookup"><span data-stu-id="c005f-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="c005f-105">U okvir za pretraživanje u sustavu Windows upišite pokreni, odaberite aplikaciju Pokreni radnu površinu, upišite services.msc, a zatim odaberite **Enter**.</span><span class="sxs-lookup"><span data-stu-id="c005f-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="c005f-106">Pomaknite se prema dolje do servisa WebClient i provjerite stupac **Status.**</span><span class="sxs-lookup"><span data-stu-id="c005f-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="c005f-107">Ako status web-klijentskog servisa nije **pokrenut,** dvokliknite servis, zatim **Start**, a potom **U redu**.</span><span class="sxs-lookup"><span data-stu-id="c005f-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="c005f-108">Omogućite uslugu, ako je potrebno, odabirom **ručnog** ili **automatskog** u okviru **Vrsta pokretanja.**</span><span class="sxs-lookup"><span data-stu-id="c005f-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="c005f-109">Da biste otklonili poteškoće s otvaranjem u eksploreru za datoteke, [pročitajte članak Otvori u programu Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="c005f-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="c005f-110">Istražite sinkronizaciju kao bolju alternativu: [sinkronizirajte datoteke sustava SharePoint s novim klijentom za sinkronizaciju sa servisom OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="c005f-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

