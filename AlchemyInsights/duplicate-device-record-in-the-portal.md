---
title: Dupliciranje zapisa o uređaju na portalu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814508"
---
# <a name="duplicate-device-record-in-the-portal"></a>Dupliciranje zapisa o uređaju na portalu

Možda će vam se na portalu prikazati dva zapisa o uređaju ako uređaj točno ne izvještava web-mjesto upravitelja konfiguracije o statusu zajedničkog upravljanja. Da biste provjerili status zajedničkog upravljanja za uređaj, pregledajte stupac **Zajedničko upravljanje** za pripadni uređaj na konzoli programa Configuration Manager. Ako stupac nije vidljiv, možete ga dodati tako da desnom tipkom miša kliknete bilo koje zaglavlje stupca i odaberete ga s popisa.

Vrijednost u stupcu Zajedničko upravljanje mora biti **Da**. Ako je vrijednost **Ne**, otvorite klijentski aplet programa Configuration Manager i na kartici Općenito provjerite svojstvo **Zajedničko upravljanje**.

- Ako ono ima vrijednost **Omogućeno**, to označava poteškoće s komunikacijom između klijenta i točke upravljanja. Pregledajte **CcmMessaging.log** na uređaju da biste istražili moguće probleme s povezivanjem.

- Ako svojstvo ima vrijednost **Onemogućeno**, a uređaj je prijavljen u Intune, provjerite je li uređaj primio pravilnik o zajedničkom upravljanju tako da pregledate **CoManagementHandler.log** na uređaju.
