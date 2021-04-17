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
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821403"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Rješavanje problema s isporukom e-pošte za kod pogreške 5.7.23

Provjerite SPF DNS zapis za svoju domenu na javno dostupnoj provjeri SPF ili DNS zapisa na webu.

Provjerite nije li Microsoft prepoznao izlaznu poruku kao neželjenu poštu i usmjeravao je putem centra za isporuku [visokog rizika](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Poruke u visokorizičnoj isporuci neće proći provjere SPF-a, pa je stoga odredišna tvrtka ili ustanova za e-poštu neće prihvatiti.

Ako se problem nastavi pojavljivati, možda ćete se morati obratiti administratoru glavnog računala e-pošte kojemu pokušavate poslati poruku e-pošte. Zabilježite detaljnu vanjsku pogrešku koja je dostupna u poruci o odskoci. Microsoftova podrška možda neće moći dodatno pomoći.
