---
title: Blokiranje preuzimanja na vezama za zajedničko korištenje
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 8cb53754125cedf4a3d0426d6c3bf70297eb3d74
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/23/2020
ms.locfileid: "44357448"
---
# <a name="block-download-on-sharing-links"></a>Blokiranje preuzimanja na vezama za zajedničko korištenje

**Blokiranje preuzimanja** dostupno je za **veze samo** za prikaz na dokumente sustava Office. Kada odaberete tu mogućnost, osobe koje dobiju pristup datoteci putem veze koju ste stvorili neće vidjeti mogućnosti za preuzimanje, ispis ili kopiranje datoteke.

Administratori mogu kontrolirati pojavljuje li se postavka "block download" samo za datoteke sustava Office ili ne promjenom `BlockDownloadLinksFileType` postavke u cmdletima [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) ili [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell.
