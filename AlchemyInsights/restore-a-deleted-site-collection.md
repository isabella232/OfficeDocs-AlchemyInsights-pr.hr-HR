---
title: Vraćanje izbrisanog web-mjesta
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: d37fd903c91c8cd6ac6137e815cb253f7edb4494
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912667"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="868a2-102">Vraćanje izbrisanog web-mjesta</span><span class="sxs-lookup"><span data-stu-id="868a2-102">Restore a deleted site</span></span>

<span data-ttu-id="868a2-103">Kada administrator izbriše SharePoint web-mjesto, on se nalazi u koš za smeće zbirke web-mjesta, gdje se čuva 93 dana prije trajnog brisanja.</span><span class="sxs-lookup"><span data-stu-id="868a2-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="868a2-104">Da biste vratili web-mjesto:</span><span class="sxs-lookup"><span data-stu-id="868a2-104">To restore the site:</span></span>
  
1. <span data-ttu-id="868a2-105">U novom centru za administratore sustava SharePoint na vrpci kliknite **Koš za smeće.**</span><span class="sxs-lookup"><span data-stu-id="868a2-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="868a2-106">Potvrdite okvir pokraj zbirke web-mjesta koju želite vratiti.</span><span class="sxs-lookup"><span data-stu-id="868a2-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="868a2-107">Kliknite **Vrati izbrisane stavke**.</span><span class="sxs-lookup"><span data-stu-id="868a2-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="868a2-108">Da biste vratili izbrisano web-mjesto za komunikaciju, možete koristiti novi centar za administratore sustava SharePoint.</span><span class="sxs-lookup"><span data-stu-id="868a2-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="868a2-109">U suprotnom morate koristiti Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="868a2-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="868a2-110">Da biste vratili web-mjesto koje pripada grupi sustava Microsoft 365, morate vratiti grupu u centru za administratore sustava Exchange.</span><span class="sxs-lookup"><span data-stu-id="868a2-110">To restore a site that belongs to an Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="868a2-111">Grupe se mogu vratiti 30 dana nakon brisanja.</span><span class="sxs-lookup"><span data-stu-id="868a2-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

