---
title: Promjena dozvola za javnu mapu
ms.author: dmaguire
author: msdmaguire
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "633"
- "3500007"
ms.assetid: 0c37ab75-c81c-44e7-bda8-ea43263f9fdf
ms.openlocfilehash: a2a902e8fdfd8628772364c173979c633d25a169
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47714239"
---
# <a name="changing-public-folder-permissions"></a><span data-ttu-id="314c0-102">Promjena dozvola za javnu mapu</span><span class="sxs-lookup"><span data-stu-id="314c0-102">Changing public folder permissions</span></span>

<span data-ttu-id="314c0-103">Dozvole za javnu mapu mogu promijeniti korisnici i administratori u programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="314c0-103">Public folder permissions can be changed by users and administrators in Outlook.</span></span> <span data-ttu-id="314c0-104">Administratori mogu i upravljati dozvolama iz centra za administratore sustava Exchange (IAC), na sljedeći način:</span><span class="sxs-lookup"><span data-stu-id="314c0-104">Administrators can also control permissions from the Exchange Admin Center (EAC), by doing the following:</span></span>
  
1. <span data-ttu-id="314c0-105">U centru za administratore sustava Microsoft 365 otvorite odjeljak **administrator centara za administratore** \> **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="314c0-105">In the Microsoft 365 admin center, go to **Admin centers** \> **Exchange**.</span></span>

2. <span data-ttu-id="314c0-106">Odaberite **javne mape**.</span><span class="sxs-lookup"><span data-stu-id="314c0-106">Select **Public folders**.</span></span>

3. <span data-ttu-id="314c0-107">Od tamo možete promijeniti dozvole za pojedinačne javne mape tako da dodijelite sigurnosne grupe dozvolama.</span><span class="sxs-lookup"><span data-stu-id="314c0-107">From there, you can change permissions for individual public folders by assigning security groups to permissions.</span></span> <span data-ttu-id="314c0-108">Da bi krajnji korisnik mogao promijeniti dozvole za javnu mapu, korisnik mora imati prava vlasnika u mapi.</span><span class="sxs-lookup"><span data-stu-id="314c0-108">For an end user to change public folder permissions, the user needs to have Owner rights on the folder.</span></span>

<span data-ttu-id="314c0-109">Slijedite postupak opisan u članku [dijagnosticiranje i rješavanje problema s dozvolama javnih mapa](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) radi otklanjanja problema s dozvolama javne mape.</span><span class="sxs-lookup"><span data-stu-id="314c0-109">Please follow the procedure described in [How to diagnose and fix public folder permission issues](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) to troubleshoot public folder permission issues.</span></span>

<span data-ttu-id="314c0-110">**Pažnja**: postoji nekoliko poznatih problema na koje možete naići kada pokušate promijeniti dozvole za javne mape.</span><span class="sxs-lookup"><span data-stu-id="314c0-110">**Note**: There are several known issues you might encounter when you try to change permissions on public folders.</span></span> <span data-ttu-id="314c0-111">Dodatne informacije potražite u sljedećim člancima.</span><span class="sxs-lookup"><span data-stu-id="314c0-111">See the following articles for more information.</span></span>

- [<span data-ttu-id="314c0-112">Nije moguće primijeniti dozvole za podmape javnih mapa u sustavu IAC</span><span class="sxs-lookup"><span data-stu-id="314c0-112">Can't apply permissions to public folder subfolders in EAC</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/can%E2%80%99t-apply-permissions-public-folder-subfolders)

- [<span data-ttu-id="314c0-113">Pogreška "poštanski sandučić nije pronađen u lokalnoj šumi" kada pristupate javnim mapama</span><span class="sxs-lookup"><span data-stu-id="314c0-113">"The mailbox is not found in the local forest" error when you access public folders</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/mailbox-not-found-local-forest-public-folder)
