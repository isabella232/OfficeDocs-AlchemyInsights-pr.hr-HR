---
title: Pretraživanje sadržaja bez rezultata
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816840"
---
# <a name="no-results-from-content-searchexports"></a>Nema rezultata pretraživanja/izvoza sadržaja

Problemi s pretraživanjem/izvozom sadržaja koji ne vraćaju podatke mogu biti uzrokovani određenim sigurnosnim filtrom usklađenosti koji je e-poštu e-pošte mogao vratiti.

Da biste riješili taj problem, provjerite postoje li sigurnosni filtri za usklađenost koji uzrokuju sljedeće:
1. Povezivanje s ljuskom Powershell centra za sigurnost i usklađenost
2. Pokrenite sljedeće naredbenelete:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org