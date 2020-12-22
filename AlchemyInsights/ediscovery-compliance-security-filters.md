---
title: Nema povratnih rezultata tijekom pretraživanja sadržaja/izvoza
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
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727215"
---
# <a name="no-results-returned-during-content-searchexport"></a>Nema povratnih rezultata tijekom pretraživanja sadržaja/izvoza

Ako nailazite na probleme s sljedećim scenarijima za otkrivanje:

- Pretraživanje sadržaja/izvoz ne vraća nikakve podatke ni neočekivane podatke
- Pretraživanje ili izvoz razotkrivanja nije uspjelo

Možda se radi o određenim sigurnosnim filtrima za usklađenost koje je postavljen određeni administrator, a nisu priopćeni svim administratorima.

Da biste riješili taj problem, provjerite postoje li sigurnosni filtri za usklađenost koji mogu uzrokovati te probleme:

1. Spojite se na PowerShell centra za sigurnost i usklađenost
2. Pokrenite sljedeće cmdlets:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Dodatne informacije o sigurnosnim filtrima usklađenosti potražite u članku [Filtriranje dozvola za pretraživanje sadržaja](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
