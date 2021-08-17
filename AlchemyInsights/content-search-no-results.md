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
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057994"
---
# <a name="no-results-from-content-searchexports"></a>Nema rezultata pretraživanja/izvoza sadržaja

Problemi s pretraživanjem/izvozom sadržaja koji ne vraćaju podatke mogu biti uzrokovani određenim sigurnosnim filtrom usklađenosti koji je e-poštu e-pošte mogao vratiti.

Da biste riješili taj problem, provjerite postoje li sigurnosni filtri za usklađenost koji uzrokuju sljedeće:
1. Povezivanje powershell centra za sigurnost i usklađenost
2. Pokrenite sljedeće naredbenelete:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org