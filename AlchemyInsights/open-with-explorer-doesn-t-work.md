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
ms.openlocfilehash: 7680766b53bd5e85789375d3f9e9ab635780ec6c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538457"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="8130d-102">Otvori pomoću programa Explorer ne radi</span><span class="sxs-lookup"><span data-stu-id="8130d-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="8130d-103">**Otvori pomoću programa Explorer** ili **Prikaz Explorer datoteka** ne radi Provjerite je li servis WebClient je postavljeno na **izvodi** slijedeći dolje navedene korake.</span><span class="sxs-lookup"><span data-stu-id="8130d-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="8130d-104">Na primjer, ga potrajati dugo otvorite biblioteku SharePoint ili OneDrive kada servis nije pokrenut.</span><span class="sxs-lookup"><span data-stu-id="8130d-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="8130d-105">U okvir za pretraživanje Windows vrsta pokrenuti, odaberite Pokreni radne površine app, vrsta services.msc i zatim odaberite **Enter**.</span><span class="sxs-lookup"><span data-stu-id="8130d-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="8130d-106">Pomaknite WebClient servisa i provjerite stupac **Stanje** .</span><span class="sxs-lookup"><span data-stu-id="8130d-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="8130d-107">Servis stanja WebClient nije **pokrenut**, dvaput kliknite servis, kliknite **Start**, a zatim kliknite **u redu**.</span><span class="sxs-lookup"><span data-stu-id="8130d-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="8130d-108">Omogućiti servis, ako je potrebno, odabirom **ručno** ili **Automatsko** u okviru **Vrsta pokretanja** .</span><span class="sxs-lookup"><span data-stu-id="8130d-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="8130d-109">Za rješavanje problema s otvaranjem datoteka Explorer vidjeti [otvorene u programu Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="8130d-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="8130d-110">Istražite sinkronizaciju kao bolja alternativa: [SharePoint sinkronizaciju datoteke s novom klijentu sinkronizaciju OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="8130d-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

