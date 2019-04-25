---
title: Nasljeđivanje dozvola
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 8/7/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bb5c440a-ca70-4dc6-b517-688e80551101
ms.openlocfilehash: 5a72a74710a01cf958fa468b80ee67a4034c4383
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32372336"
---
# <a name="how-permissions-inheritance-works-in-sharepoint"></a><span data-ttu-id="341ec-102">Kako funkcionira nasljeđivanje dozvola u programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="341ec-102">How permissions inheritance works in SharePoint</span></span>

<span data-ttu-id="341ec-103">Po zadanom, dozvole u SharePoint nasljeđuju od gore viši u hijerarhiji.</span><span class="sxs-lookup"><span data-stu-id="341ec-103">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="341ec-104">Stoga datoteku svoje dozvole nasljeđuju od mapa nasljeđuje dozvole iz biblioteke koji svoje dozvole nasljeđuju od web-mjesta, koji svoje dozvole nasljeđuju iz zbirke web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="341ec-104">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site, which inherits its permissions from the site collection.</span></span>
  
<span data-ttu-id="341ec-105">Info o uklanjanju jedinstvene dozvole i vraćanju nasljeđivanje pogledajte u [Uređivanje i upravljanje dozvolama za popis ili biblioteku](https://go.microsoft.com/fwlink/?linkid=869946).</span><span class="sxs-lookup"><span data-stu-id="341ec-105">For info about removing unique permissions and restoring inheritance, see [Edit and manage permissions for a list or library](https://go.microsoft.com/fwlink/?linkid=869946).</span></span>
  

