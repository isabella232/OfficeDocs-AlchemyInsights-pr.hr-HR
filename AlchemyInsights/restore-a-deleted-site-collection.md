---
title: Vraćanje izbrisane zbirke
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 1f9a66daf7bee43291b785b6260aec8725ee782f
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753778"
---
# <a name="restore-a-deleted-site-collection"></a><span data-ttu-id="311a1-102">Vraćanje izbrisane zbirke</span><span class="sxs-lookup"><span data-stu-id="311a1-102">Restore a deleted site collection</span></span>

<span data-ttu-id="311a1-103">Kada je admin briše klasični zbirke, smještene u zbirci web-mjesta koš za smeće, gdje čuvati 93 dana prije trajno izbrisane.</span><span class="sxs-lookup"><span data-stu-id="311a1-103">When an admin deletes a classic site collection, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="311a1-104">Vraćanje zbirke web-mjesta:</span><span class="sxs-lookup"><span data-stu-id="311a1-104">To restore the site collection:</span></span>
  
1. <span data-ttu-id="311a1-105">U klasičnom admin centru SharePoint kliknite **Koš za smeće** na vrpci.</span><span class="sxs-lookup"><span data-stu-id="311a1-105">In the classic SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="311a1-106">Odaberite potvrdni okvir uz zbirke web-mjesta koje želite vratiti.</span><span class="sxs-lookup"><span data-stu-id="311a1-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="311a1-107">Kliknite **Vrati izbrisane stavke**.</span><span class="sxs-lookup"><span data-stu-id="311a1-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="311a1-108">Da biste vratili izbrisane komunikacije web-mjesta, možete koristiti novi centar pretpregled admin SharePoint.</span><span class="sxs-lookup"><span data-stu-id="311a1-108">To restore a deleted communication site, you can use the new SharePoint admin center preview.</span></span> <span data-ttu-id="311a1-109">U suprotnom, trebate koristiti PowerShell.</span><span class="sxs-lookup"><span data-stu-id="311a1-109">Otherwise, you need to use PowerShell.</span></span> <span data-ttu-id="311a1-110">Da biste vratili web-mjesto koje pripada grupi Office 365, morate vratiti grupu u Centar za administraciju sustava Exchange.</span><span class="sxs-lookup"><span data-stu-id="311a1-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="311a1-111">Grupe se mogu vratiti za 30 dana nakon što si izbrisan.</span><span class="sxs-lookup"><span data-stu-id="311a1-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

