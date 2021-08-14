---
title: Antispam - 5.7.23
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
- "3156"
- "9001196"
ms.openlocfilehash: cb9073306c65b09813290d6c8470d14395d2836fa3048f8ce0ecb8b06e71a010
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932161"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Rješavanje problema s isporukom e-pošte za kod pogreške 5.7.23

Provjerite SPF DNS zapis za svoju domenu na javno dostupnoj provjeri SPF ili DNS zapisa na webu.

Provjerite nije li Microsoft prepoznao izlaznu poruku kao neželjenu poštu i usmjeravao je putem centra za isporuku [visokog rizika](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Poruke u visokorizičnoj isporuci neće proći provjere SPF-a, pa je stoga odredišna tvrtka ili ustanova za e-poštu neće prihvatiti.

Ako se problem nastavi pojavljivati, možda ćete se morati obratiti administratoru glavnog računala e-pošte kojemu pokušavate poslati poruku e-pošte. Zabilježite detaljnu vanjsku pogrešku koja je dostupna u poruci o odskoci. Microsoftova podrška možda neće moći dodatno pomoći.
