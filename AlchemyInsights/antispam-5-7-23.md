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
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506435"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Rješavanje problema s isporukom e-pošte za kod pogreške 5.7.23

Provjerite SPF DNS zapis za svoju domenu na javno dostupnom SPF ili DNS zapisu na webu.

Provjerite nije li Microsoft identificirao odlaznu poruku kao neželjenu poštu i da je preusmjeren kroz bazen za [isporuku visokog rizika](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Poruke u skupu za isporuku visokog rizika neće proći SPF provjere i stoga neće biti prihvaćene od strane odredišne organizacije e-pošte.

Ako se problem nastavi pojavljivati, možda ćete se morati obratiti administratoru glavnog računala e-pošte kojem pokušavate poslati e-poštu. Zabilježite detaljnu vanjsku pogrešku dostupnu u poruci napuštanja početne stranice. Microsoftova podrška možda neće moći dalje pomagati.
