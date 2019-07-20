---
title: Nema rezultata pretraživanja sadržaja
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800234"
---
# <a name="no-results-from-content-searchexports"></a>Nema rezultata iz sadržaja pretraživanja/izvozi

Problemi s sadržaja pretraživanja/izvozi ne daje nikakve podatke možda određene usklađenosti sigurnost filtar koji je postavljanje određene Admin i nije je komunikacija sve administratori.

Da biste riješili taj problem, provjerite postoje filtre usklađenosti sigurnosti koji uzrokuje ovo:
1. Povezivanje s sigurnost i usklađenosti centar Powershell
2. Pokreni Cmdlete sljedeće:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-$org organizacije