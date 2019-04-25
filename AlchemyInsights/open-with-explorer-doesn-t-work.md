---
title: Otvori pomoću programa Explorer ne radi
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 73d33e50449345c312abdd39afcc36e0c95fd1c4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32419858"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="5de36-102">Otvori pomoću programa Explorer ne radi</span><span class="sxs-lookup"><span data-stu-id="5de36-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="5de36-103">**Otvori pomoću programa Explorer** ili **Prikaz Explorer datoteka** ne radi Provjerite je li servis WebClient je postavljeno na **izvodi** slijedeći dolje navedene korake.</span><span class="sxs-lookup"><span data-stu-id="5de36-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="5de36-104">Na primjer, ga potrajati dugo otvorite biblioteku SharePoint ili OneDrive kada servis nije pokrenut.</span><span class="sxs-lookup"><span data-stu-id="5de36-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="5de36-105">U okvir za pretraživanje Windows vrsta pokrenuti, odaberite Pokreni radne površine app, vrsta services.msc i zatim odaberite **Enter**.</span><span class="sxs-lookup"><span data-stu-id="5de36-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="5de36-106">Pomaknite WebClient servisa i provjerite stupac **Stanje** .</span><span class="sxs-lookup"><span data-stu-id="5de36-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="5de36-107">Servis stanja WebClient nije **pokrenut**, dvaput kliknite servis, kliknite **Start**, a zatim kliknite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="5de36-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="5de36-108">Omogućiti servis, ako je potrebno, odabirom **ručno** ili **Automatsko** u okviru **Vrsta pokretanja** .</span><span class="sxs-lookup"><span data-stu-id="5de36-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="5de36-109">Za rješavanje problema s otvaranjem datoteka Explorer vidjeti [otvorene u programu Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="5de36-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="5de36-110">Istražite sinkronizaciju kao bolja alternativa: [SharePoint sinkronizaciju datoteke s novom klijentu sinkronizaciju OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="5de36-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

