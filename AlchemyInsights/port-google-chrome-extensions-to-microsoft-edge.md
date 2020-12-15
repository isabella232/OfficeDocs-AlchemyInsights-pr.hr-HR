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
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>Priključak Google Chrome Extensions na Microsoft Edge (krom)

U [programu Microsoft Edge (krom) lako je priključit ekstenzije preglednika Google Chrome](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension). U većini slučajeva potrebna su samo minimalna promjena da bi se nastavile ove proširenja u pregledniku Microsoft Edge.

API-jevi proširenja i tipke manifesta podržane u pregledniku Google Chrome kompatibilni su sa sustavom Microsoft Edge. Međutim, Microsoft Edge ne podržava ekstenziju APIs Chrome. GCM, Chrome. Identity. GETAC, krom. Identity. getAuthToken i Chrome. instanceID.