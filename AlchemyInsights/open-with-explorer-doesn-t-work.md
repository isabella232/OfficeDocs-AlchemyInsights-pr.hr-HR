---
title: Otvori pomoću programa Explorer ne funkcionira
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694448"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="4c39f-102">Otvaranje pomoću programa Explorer ne funkcionira</span><span class="sxs-lookup"><span data-stu-id="4c39f-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="4c39f-103">Ako je u eksploreru **za datoteke** **otvoreno pomoću programa Explorer** ili prikaz, provjerite je li web-klijent poslužitelj postavljen na **pokretanje** slijedeći korake u nastavku.</span><span class="sxs-lookup"><span data-stu-id="4c39f-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="4c39f-104">Možda će, primjerice, trebati dugo vremena za otvaranje biblioteke sustava SharePoint ili servisa OneDrive kada servis nije pokrenut.</span><span class="sxs-lookup"><span data-stu-id="4c39f-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="4c39f-105">U okvir za pretraživanje sustava Windows upišite Pokreni, odaberite Pokreni aplikaciju za stolna računala, upišite Services. msc, a zatim odaberite **Enter**.</span><span class="sxs-lookup"><span data-stu-id="4c39f-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="4c39f-106">Pomaknite se prema dolje do web-klijentskog servisa i provjerite stupac **status** .</span><span class="sxs-lookup"><span data-stu-id="4c39f-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="4c39f-107">Ako status servisa WebClient nije **pokrenut**, dvokliknite servis, zatim kliknite **Start**, a potom **u redu**.</span><span class="sxs-lookup"><span data-stu-id="4c39f-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="4c39f-108">Ako je potrebno, omogućite servis tako da odaberete **ručno** ili **Automatsko** u okviru **Vrsta pokretanja** .</span><span class="sxs-lookup"><span data-stu-id="4c39f-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="4c39f-109">Upute za otklanjanje poteškoća u eksploreru za datoteke potražite [u članku otvaranje u programu Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="4c39f-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="4c39f-110">Istražite sinkronizaciju kao bolju alternativu: [Sinkronizacija datoteka sustava SharePoint s novim klijentom za sinkronizaciju servisa OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="4c39f-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

