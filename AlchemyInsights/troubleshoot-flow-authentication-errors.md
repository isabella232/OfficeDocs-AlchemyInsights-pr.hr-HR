---
title: Otklanjanje poteškoća s pogreškama provjere autentičnosti tijeka
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c15fed9f-65c6-422e-9d32-87e889a44b51
ms.openlocfilehash: 70451f074a65a4454faeadd188a31783be8e6c7e
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759720"
---
# <a name="troubleshoot-flow-authentication-errors"></a><span data-ttu-id="639ff-102">Otklanjanje poteškoća s pogreškama provjere autentičnosti tijeka</span><span class="sxs-lookup"><span data-stu-id="639ff-102">Troubleshoot Flow authentication errors</span></span>

<span data-ttu-id="639ff-103">U mnogim slučajevima tokovi ne uspijevaju zbog pogreške provjere autentičnosti.</span><span class="sxs-lookup"><span data-stu-id="639ff-103">In many cases, flows fail because of an authentication error.</span></span> <span data-ttu-id="639ff-104">Ako imate ovu vrstu pogreške, pojavljuje se poruka o pogrešci "Neovlašteno" ili šifra pogreške 401 ili 403.</span><span class="sxs-lookup"><span data-stu-id="639ff-104">If you have this type of error, the error message contains "Unauthorized," or an error code of 401 or 403 appears.</span></span> <span data-ttu-id="639ff-105">Pogrešku provjere autentičnosti obično možete ispraviti ažuriranjem veze:</span><span class="sxs-lookup"><span data-stu-id="639ff-105">You can usually fix an authentication error by updating the connection:</span></span>
  
1. <span data-ttu-id="639ff-106">Pri vrhu web-portala kliknite ili dodirnite ikonu zupčanika da biste otvorili izbornik Postavke, a zatim kliknite ili dodirnite **Veze**.</span><span class="sxs-lookup"><span data-stu-id="639ff-106">At the top of the web portal, click or tap the gear icon to open the Settings menu, and then click or tap **Connections**.</span></span>
    
2. <span data-ttu-id="639ff-107">Pomaknite se do veze za koju ste vidjeli poruku o pogrešci Neovlašteno.</span><span class="sxs-lookup"><span data-stu-id="639ff-107">Scroll to the connection for which you saw the Unauthorized error message.</span></span>
    
3. <span data-ttu-id="639ff-108">Pored veze kliknite ili dodirnite vezu **Potvrdi lozinku** u poruci o vezi koja nije provjerena.</span><span class="sxs-lookup"><span data-stu-id="639ff-108">Next to the connection, click or tap the **Verify password** link in the message about the connection not being authenticated.</span></span> 
    
4. <span data-ttu-id="639ff-109">Potvrdite vjerodajnice slijedeći upute koje se pojavljuju, vratite se na neuspjeh tijeka, a zatim kliknite ili dodirnite **Ponovno pošalji**.</span><span class="sxs-lookup"><span data-stu-id="639ff-109">Verify your credentials by following the instructions that appear, return to your flow-run failure, and then click or tap **Resubmit**.</span></span>
    
<span data-ttu-id="639ff-110">Dodatne informacije potražite u [odjeljku Otklanjanje poteškoća s protokom](https://go.microsoft.com/fwlink/?linkid=872110).</span><span class="sxs-lookup"><span data-stu-id="639ff-110">For more help, see [Troubleshooting a flow](https://go.microsoft.com/fwlink/?linkid=872110).</span></span>
  

