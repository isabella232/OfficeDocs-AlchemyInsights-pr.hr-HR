---
title: Došlo je do pogreške prilikom validacije pogreške u pristupnom tokenu tijekom sesije analitike radne površine
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
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813680"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Pogreška "Došlo je do pogreške prilikom validacije pristupnog tokena" tijekom rada analitike radne površine

Ta se pogreška obično opaža kada token za provjeru autentičnosti istekne. Osvježavanje stranice obično osvježava token. No taj se problem može zadržati ako postoje neki pravilniki uvjetnog pristupa koji se primjenjuju na račun koji se koristi za analitiku radne površine na ploči. Možete pregledati zapisnike prijave za Azure AD na portalu Azure da biste vidjeli postoje li pogreške pri prijavi za račun koji se koristi za analitiku radne površine u sustavu.

Dodatne informacije o uvjetnom pristupu potražite u web-aplikaciji [Planiranje implementacije uvjetnog pristupa](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).