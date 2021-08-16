---
title: Nema rezultata koji se vraćaju tijekom pretraživanja/izvoza sadržaja
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: 5c04364f98dccbcad0f011df866f137d79c166ad3839b408d6be447d50a87ac3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101258"
---
# <a name="no-results-returned-during-content-searchexport"></a>Nema rezultata koji se vraćaju tijekom pretraživanja/izvoza sadržaja

Ako nailazite na probleme sa sljedećim scenarijima predočavanja elektroničkih elektroničkih podataka:

- Pretraživanje/izvoz sadržaja ne vraća podatke ni neočekivane podatke.
- Pretraživanje ili izvoz predočavanja elektroničkih elektroničkih podataka ne uspijeva

To može biti zbog određenih sigurnosnih filtara za usklađenost koje je e-pošte moguće postaviti od određenog administratora, a koji nisu priopćani svim administratorima.

Da biste riješili taj problem, provjerite postoje li sigurnosni filtri za usklađenost koji uzrokuju sljedeće probleme:

1. Povezivanje powershell centra za sigurnost i usklađenost
2. Pokrenite sljedeće naredbenelete:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Dodatne informacije o sigurnosnim filtrima usklađenosti potražite [u članku Filtriranje dozvola za pretraživanje sadržaja](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
