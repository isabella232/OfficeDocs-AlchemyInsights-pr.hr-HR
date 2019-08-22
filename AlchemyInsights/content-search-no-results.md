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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516771"
---
# <a name="no-results-from-content-searchexports"></a>Nema rezultata iz sadržaja pretraživanja/izvozi

Problemi s sadržaja pretraživanja/izvozi ne daje nikakve podatke možda određene usklađenosti sigurnost filtar koji je postavljanje određene Admin i nije je komunikacija sve administratori.

Da biste riješili taj problem, provjerite postoje filtre usklađenosti sigurnosti koji uzrokuje ovo:
1. Povezivanje s sigurnost i usklađenosti centar Powershell
2. Pokreni Cmdlete sljedeće:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-$org organizacije