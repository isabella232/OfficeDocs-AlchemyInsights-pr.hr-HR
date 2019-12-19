---
title: Došlo je do pogreške pri validaciji pogreške tokena pristupa tijekom analitike radne površine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741136"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>"Došlo je do pogreške pri validaciji pristupne tokena" tijekom analitike radne površine

Ova pogreška se obično promatra kada token za provjeru autentičnosti istekne. Obično osvježavanje stranice osvježava token. Međutim, taj se problem može nastaviti ako postoje pravila uvjetnog pristupa koja se primjenjuju na račun koji se koristi za analitiku radne površine na ploči. Možete pregledati zapise za prijavu u Azure AD u web-portalu Azure da biste vidjeli postoje li neuspjesi za prijavu za račun koji se koristi za analitiku radne površine.

Dodatne informacije o uvjetnom pristupu potražite u [planu uvođenja uvjetnog pristupa](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).