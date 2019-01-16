---
title: Vraćanje izbrisane zbirke
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: b3c72033dfcc093dd0c2837d2866c6a78d64449c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28280088"
---
# <a name="restore-a-deleted-site-collection"></a><span data-ttu-id="3a417-102">Vraćanje izbrisane zbirke</span><span class="sxs-lookup"><span data-stu-id="3a417-102">Restore a deleted site collection</span></span>

<span data-ttu-id="3a417-p101">Kada je admin briše klasični zbirke, smještene u zbirci web-mjesta koš za smeće, gdje čuvati 93 dana prije trajno izbrisane. Vraćanje zbirke web-mjesta:</span><span class="sxs-lookup"><span data-stu-id="3a417-p101">When an admin deletes a classic site collection, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted. To restore the site collection:</span></span>
  
1. <span data-ttu-id="3a417-105">U klasičnom admin centru SharePoint kliknite **Koš za smeće** na vrpci.</span><span class="sxs-lookup"><span data-stu-id="3a417-105">In the classic SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="3a417-106">Odaberite potvrdni okvir uz zbirke web-mjesta koje želite vratiti.</span><span class="sxs-lookup"><span data-stu-id="3a417-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="3a417-107">Kliknite **Vrati izbrisane stavke**.</span><span class="sxs-lookup"><span data-stu-id="3a417-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="3a417-p102">Da biste vratili izbrisane komunikacije web-mjesta, možete koristiti novi centar pretpregled admin SharePoint. U suprotnom, trebate koristiti PowerShell. Da biste vratili web-mjesto koje pripada grupi Office 365, morate vratiti grupu u Centar za administraciju sustava Exchange. Grupe se mogu vratiti za 30 dana nakon što si izbrisan.</span><span class="sxs-lookup"><span data-stu-id="3a417-p102">To restore a deleted communication site, you can use the new SharePoint admin center preview. Otherwise, you need to use PowerShell. To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center. Groups can be restored for 30 days after they're deleted.</span></span>
  

