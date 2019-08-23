---
title: Vraćanje izbrisane web-mjesta
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
ms.openlocfilehash: 9e4e9ade058c60ecd7a6ce1b2a40c4996ac5676f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36552454"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="c31d3-102">Vraćanje izbrisane web-mjesta</span><span class="sxs-lookup"><span data-stu-id="c31d3-102">Restore a deleted site</span></span>

<span data-ttu-id="c31d3-103">Kada je admin briše web-mjesta, smješta u zbirci web-mjesta koš za smeće, gdje čuvati 93 dana prije trajno izbrisane.</span><span class="sxs-lookup"><span data-stu-id="c31d3-103">When an admin deletes a site , it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="c31d3-104">Za vraćanje na web-mjestu:</span><span class="sxs-lookup"><span data-stu-id="c31d3-104">To restore the site:</span></span>
  
1. <span data-ttu-id="c31d3-105">U novi SharePoint administraciju centar na vrpci kliknite **Koš za smeće** .</span><span class="sxs-lookup"><span data-stu-id="c31d3-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="c31d3-106">Odaberite potvrdni okvir uz zbirke web-mjesta koje želite vratiti.</span><span class="sxs-lookup"><span data-stu-id="c31d3-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="c31d3-107">Kliknite **Vrati izbrisane stavke**.</span><span class="sxs-lookup"><span data-stu-id="c31d3-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="c31d3-108">Da biste vratili izbrisane komunikacije web-mjesta, možete koristiti novi centar za administraciju sustava SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c31d3-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="c31d3-109">U suprotnom, morate koristiti Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c31d3-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="c31d3-110">Da biste vratili web-mjesto koje pripada grupi Office 365, morate vratiti grupu u Centar za administraciju sustava Exchange.</span><span class="sxs-lookup"><span data-stu-id="c31d3-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="c31d3-111">Grupe se mogu vratiti za 30 dana nakon što si izbrisan.</span><span class="sxs-lookup"><span data-stu-id="c31d3-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

