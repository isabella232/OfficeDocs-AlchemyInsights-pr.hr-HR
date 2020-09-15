---
title: Vraćanje izbrisanog web-mjesta
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 570284765f32212b4ef2062db5b70f427b28c121
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47692035"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="63913-102">Vraćanje izbrisanog web-mjesta</span><span class="sxs-lookup"><span data-stu-id="63913-102">Restore a deleted site</span></span>

<span data-ttu-id="63913-103">Kada administrator izbriše web-mjesto sustava SharePoint, ona će se smjestiti u koš za smeće zbirke web-mjesta, gdje se čuva za 93 dana prije nego što ga trajno izbrišete.</span><span class="sxs-lookup"><span data-stu-id="63913-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="63913-104">Da biste vratili web-mjesto, učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="63913-104">To restore the site:</span></span>
  
1. <span data-ttu-id="63913-105">U novom centru za administratore sustava SharePoint kliknite **Koš za** smeće na vrpci.</span><span class="sxs-lookup"><span data-stu-id="63913-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="63913-106">Potvrdite okvir pokraj zbirke web-mjesta koju želite vratiti.</span><span class="sxs-lookup"><span data-stu-id="63913-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="63913-107">Kliknite **Vrati izbrisane stavke**.</span><span class="sxs-lookup"><span data-stu-id="63913-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="63913-108">Da biste vratili izbrisano web-mjesto za komunikaciju, možete koristiti novi centar za administratore sustava SharePoint.</span><span class="sxs-lookup"><span data-stu-id="63913-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="63913-109">U suprotnom morate koristiti Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="63913-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="63913-110">Da biste vratili web-mjesto koje pripada grupi Microsoft 365, morate vratiti grupu u centar za administratore sustava Exchange.</span><span class="sxs-lookup"><span data-stu-id="63913-110">To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="63913-111">Grupe se mogu vratiti 30 dana nakon brisanja.</span><span class="sxs-lookup"><span data-stu-id="63913-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

