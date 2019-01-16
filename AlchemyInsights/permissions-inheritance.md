---
title: Nasljeđivanje dozvola
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 8/7/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: bb5c440a-ca70-4dc6-b517-688e80551101
ms.openlocfilehash: e3e3ff0343b2e24e56d3e9b0355f291a3779e855
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28280453"
---
# <a name="how-permissions-inheritance-works-in-sharepoint"></a><span data-ttu-id="bb89f-102">Kako funkcionira nasljeđivanje dozvola u programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="bb89f-102">How permissions inheritance works in SharePoint</span></span>

<span data-ttu-id="bb89f-p101">Po zadanom, dozvole u SharePoint nasljeđuju od gore viši u hijerarhiji. Stoga datoteku svoje dozvole nasljeđuju od mapa nasljeđuje dozvole iz biblioteke koji svoje dozvole nasljeđuju od web-mjesta, koji svoje dozvole nasljeđuju iz zbirke web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="bb89f-p101">By default, permissions in SharePoint are inherited from higher up in the hierarchy. So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site, which inherits its permissions from the site collection.</span></span>
  
<span data-ttu-id="bb89f-105">Info o uklanjanju jedinstvene dozvole i vraćanju nasljeđivanje pogledajte u [Uređivanje i upravljanje dozvolama za popis ili biblioteku](https://go.microsoft.com/fwlink/?linkid=869946).</span><span class="sxs-lookup"><span data-stu-id="bb89f-105">For info about removing unique permissions and restoring inheritance, see [Edit and manage permissions for a list or library](https://go.microsoft.com/fwlink/?linkid=869946).</span></span>
  

