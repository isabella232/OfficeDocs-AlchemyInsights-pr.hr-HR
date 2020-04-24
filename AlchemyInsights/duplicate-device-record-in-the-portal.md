---
title: Dupliciranje zapisa o uređaju na portalu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/23/2020
ms.locfileid: "43789681"
---
# <a name="duplicate-device-record-in-the-portal"></a>Dupliciranje zapisa o uređaju na portalu

Možda će vam se na portalu prikazati dva zapisa o uređaju ako uređaj točno ne izvještava web-mjesto upravitelja konfiguracije o statusu zajedničkog upravljanja. Da biste provjerili status zajedničkog upravljanja za uređaj, pregledajte stupac **Zajedničko upravljanje** za pripadni uređaj na konzoli programa Configuration Manager. Ako stupac nije vidljiv, možete ga dodati tako da desnom tipkom miša kliknete bilo koje zaglavlje stupca i odaberete ga s popisa.

Vrijednost u stupcu Zajedničko upravljanje mora biti **Da**. Ako je vrijednost **Ne**, otvorite klijentski aplet programa Configuration Manager i na kartici Općenito provjerite svojstvo **Zajedničko upravljanje**.

- Ako ono ima vrijednost **Omogućeno**, to označava poteškoće s komunikacijom između klijenta i točke upravljanja. Pregledajte **CcmMessaging.log** na uređaju da biste istražili moguće probleme s povezivanjem.

- Ako svojstvo ima vrijednost **Onemogućeno**, a uređaj je prijavljen u Intune, provjerite je li uređaj primio pravilnik o zajedničkom upravljanju tako da pregledate **CoManagementHandler.log** na uređaju.
