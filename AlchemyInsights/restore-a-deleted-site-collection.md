---
title: Vraćanje izbrisanog web-mjesta
ms.author: kaarins
author: kaarins
manager: scotv
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: a1fb15869b9f576696de4eda4c0b2101bd6cca17
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768540"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="962b3-102">Vraćanje izbrisanog web-mjesta</span><span class="sxs-lookup"><span data-stu-id="962b3-102">Restore a deleted site</span></span>

<span data-ttu-id="962b3-103">Kada administrator izbriše SharePoint web-mjesto, smješta se u koš za smeće zbirke web-mjesta, gdje se čuva 93 dana prije nego što se trajno izbriše.</span><span class="sxs-lookup"><span data-stu-id="962b3-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="962b3-104">Da biste vratili web-mjesto:</span><span class="sxs-lookup"><span data-stu-id="962b3-104">To restore the site:</span></span>
  
1. <span data-ttu-id="962b3-105">U novom SharePoint centru za administraciju kliknite **Koš za smeće** na vrpci.</span><span class="sxs-lookup"><span data-stu-id="962b3-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="962b3-106">Potvrdite okvir pokraj zbirke web-mjesta koju želite vratiti.</span><span class="sxs-lookup"><span data-stu-id="962b3-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="962b3-107">Kliknite **Vrati izbrisane stavke**.</span><span class="sxs-lookup"><span data-stu-id="962b3-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="962b3-108">Da biste vratili izbrisano web-mjesto za komunikaciju, možete koristiti novi centar za administraciju sustava SharePoint.</span><span class="sxs-lookup"><span data-stu-id="962b3-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="962b3-109">Inače, morate koristiti Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="962b3-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="962b3-110">Da biste vratili web-mjesto koje pripada grupi sustava Office 365, morate vratiti grupu u centar za administraciju sustava Exchange.</span><span class="sxs-lookup"><span data-stu-id="962b3-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="962b3-111">Grupe se mogu obnoviti 30 dana nakon što se brišu.</span><span class="sxs-lookup"><span data-stu-id="962b3-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

