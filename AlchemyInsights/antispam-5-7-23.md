---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676489"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Rješavanje problema s isporukom e-pošte za kod pogreške 5.7.23

Provjerite SPF DNS zapis za svoju domenu na javno dostupnom SPF ili DNS provjeru zapisa na webu.

Provjerite nije li Microsoft identificirao odlaznu poruku kao neželjenu poštu i usmjerio se putem grupe za [isporuku visokog rizika](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). Poruke u skupu za isporuku visokog rizika neće proći SPF čekove i stoga ih odredišna organizacija e-pošte neće prihvatiti.

Ako se problem nastavi pojavljivati, možda ćete se morati obratiti administratoru glavnog računala pošte kojem pokušavate poslati e-poštu. Zabilježite detaljnu vanjsku pogrešku dostupnu u poruci napuštanja početne stranice. Microsoftova podrška možda neće moći dodatno pomoći.
