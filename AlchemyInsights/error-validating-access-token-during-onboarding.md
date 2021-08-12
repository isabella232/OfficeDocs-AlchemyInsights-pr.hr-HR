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
ms.openlocfilehash: 1d6b840e731eaff537d8f74f9ce0af29af13bd390e701fb2835e8718b4521158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946607"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Pogreška "Došlo je do pogreške prilikom validacije pristupnog tokena" tijekom rada analitike radne površine

Ta se pogreška obično opaža kada token za provjeru autentičnosti istekne. Osvježavanje stranice obično osvježava token. No taj se problem može zadržati ako postoje neki pravilniki uvjetnog pristupa koji se primjenjuju na račun koji se koristi za analitiku radne površine na ploči. Možete pregledati zapisnike prijave za Azure AD na portalu Azure da biste vidjeli postoje li pogreške pri prijavi za račun koji se koristi za analitiku radne površine u sustavu.

Dodatne informacije o uvjetnom pristupu potražite u web-aplikaciji [Planiranje implementacije uvjetnog pristupa](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).