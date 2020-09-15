---
title: Nema rezultata pretraživanja sadržaja
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680639"
---
# <a name="no-results-from-content-searchexports"></a>Nema rezultata pretraživanja sadržaja/izvoza

Problemi s pretraživanjem sadržaja/izvozom koji ne vraća podatke možda je razlog za određeni sigurnosni filtar za usklađenost koji je postavio određeni administrator i nije ga mogao komunicirati sa svim administratorima.

Da biste riješili taj problem, provjerite postoje li neki sigurnosni filtri za usklađenost koji mogu prouzročiti sljedeće:
1. Spojite se na PowerShell centra za sigurnost i usklađenost
2. Pokrenite sljedeće cmdlets:
<br>$org = "yourdomain.com"
<br>Filtar za dohvaćanje i usklađenost $org