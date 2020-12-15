---
title: Priključak Google Chrome Extensions na Microsoft Edge (krom)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004032"
- "7102"
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49676996"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a><span data-ttu-id="442f1-102">Priključak Google Chrome Extensions na Microsoft Edge (krom)</span><span class="sxs-lookup"><span data-stu-id="442f1-102">Port Google Chrome extensions to Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="442f1-103">U [programu Microsoft Edge (krom) lako je priključit ekstenzije preglednika Google Chrome](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span><span class="sxs-lookup"><span data-stu-id="442f1-103">It's easy to [port Google Chrome extensions to Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span></span> <span data-ttu-id="442f1-104">U većini slučajeva potrebna su samo minimalna promjena da bi se nastavile ove proširenja u pregledniku Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="442f1-104">In most cases, only minimal changes are needed to run these extensions on Microsoft Edge.</span></span>

<span data-ttu-id="442f1-105">API-jevi proširenja i tipke manifesta podržane u pregledniku Google Chrome kompatibilni su sa sustavom Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="442f1-105">The extension APIs and manifest keys supported by Google Chrome are code-compatible with Microsoft Edge.</span></span> <span data-ttu-id="442f1-106">Međutim, Microsoft Edge ne podržava ekstenziju APIs Chrome. GCM, Chrome. Identity. GETAC, krom. Identity. getAuthToken i Chrome. instanceID.</span><span class="sxs-lookup"><span data-stu-id="442f1-106">However, Microsoft Edge does not support the extension APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, and chrome.instanceID.</span></span>