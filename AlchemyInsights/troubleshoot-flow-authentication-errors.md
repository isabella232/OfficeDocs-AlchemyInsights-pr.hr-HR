---
title: Otklanjanje poteškoća s pogreškama provjere autentičnosti toka
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c15fed9f-65c6-422e-9d32-87e889a44b51
ms.openlocfilehash: 3c4ad806ed446803d8c1e0ba17b3a06d591985d9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690559"
---
# <a name="troubleshoot-flow-authentication-errors"></a><span data-ttu-id="43b76-102">Otklanjanje poteškoća s pogreškama provjere autentičnosti toka</span><span class="sxs-lookup"><span data-stu-id="43b76-102">Troubleshoot Flow authentication errors</span></span>

<span data-ttu-id="43b76-103">U mnogim slučajevima tijek nije uspješan zbog pogreške provjere autentičnosti.</span><span class="sxs-lookup"><span data-stu-id="43b76-103">In many cases, flows fail because of an authentication error.</span></span> <span data-ttu-id="43b76-104">Ako imate tu vrstu pogreške, poruka o pogrešci sadrži "neovlašteno" ili se prikazuje kod pogreške 401 ili 403.</span><span class="sxs-lookup"><span data-stu-id="43b76-104">If you have this type of error, the error message contains "Unauthorized," or an error code of 401 or 403 appears.</span></span> <span data-ttu-id="43b76-105">Pogreška provjere autentičnosti obično možete ispraviti ažuriranjem veze:</span><span class="sxs-lookup"><span data-stu-id="43b76-105">You can usually fix an authentication error by updating the connection:</span></span>
  
1. <span data-ttu-id="43b76-106">Pri vrhu web-portala kliknite ili dodirnite ikonu zupčanika da biste otvorili izbornik postavke, a zatim kliknite ili dodirnite **veze**.</span><span class="sxs-lookup"><span data-stu-id="43b76-106">At the top of the web portal, click or tap the gear icon to open the Settings menu, and then click or tap **Connections**.</span></span>
    
2. <span data-ttu-id="43b76-107">Pomaknite se do veze za koju ste vidjeli neautoriziranu poruku o pogrešci.</span><span class="sxs-lookup"><span data-stu-id="43b76-107">Scroll to the connection for which you saw the Unauthorized error message.</span></span>
    
3. <span data-ttu-id="43b76-108">Pokraj veze kliknite ili dodirnite vezu **Potvrdi lozinku** u poruci o vezi koja nije potvrđena.</span><span class="sxs-lookup"><span data-stu-id="43b76-108">Next to the connection, click or tap the **Verify password** link in the message about the connection not being authenticated.</span></span> 
    
4. <span data-ttu-id="43b76-109">Potvrđivanje vjerodajnica slijedite upute koje se prikazuju, vratite se na neuspjeh tijeka rada, a zatim kliknite ili dodirnite **Ponovno pošalji**.</span><span class="sxs-lookup"><span data-stu-id="43b76-109">Verify your credentials by following the instructions that appear, return to your flow-run failure, and then click or tap **Resubmit**.</span></span>
    
<span data-ttu-id="43b76-110">Dodatnu pomoć potražite u članku [Otklanjanje poteškoća s protokom](https://go.microsoft.com/fwlink/?linkid=872110).</span><span class="sxs-lookup"><span data-stu-id="43b76-110">For more help, see [Troubleshooting a flow](https://go.microsoft.com/fwlink/?linkid=872110).</span></span>
  

