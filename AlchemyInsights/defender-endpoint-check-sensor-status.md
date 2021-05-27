---
title: Status senzora provjere krajnje točke programa Defender
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676056"
---
# <a name="defender-endpoint-check-sensor-status"></a>Status senzora provjere krajnje točke programa Defender

Pločica **Uređaji s problemima sa senzorom** nalazi se na nadzornoj ploči sigurnosnih operacija. Ova pločica sadrži informacije o mogućnosti pojedinačnog uređaja za pružanje podataka senzora i komunikaciju sa servisom Defender for Endpoint. U njemu se izvješćuje koliko je uređaja potrebno obratiti pozornost i pomaže vam prepoznati problematične uređaje i poduzeti radnje za ispravljanje poznatih problema.

Dva pokazatelja statusa na pločici pružaju informacije o broju uređaja koji se ne prijave pravilno servisu:

- **Pogrešno konfigurirano** Uređaji koji djelomično izvješćuju o podacima senzora servisu Defender for Endpoint i mogu imati konfiguracijske pogreške koje je potrebno ispraviti.
- **Neaktivno** Uređaji koji su u proteklom mjesecu prestali izvješćivanju o servisu Defender za krajnju točku više od sedam dana.

Klikom na neku od grupa usmjeravate se na popis Uređaji filtrirani prema vašim izborima. Na popisu Uređaji popis stanja stanja možete filtrirati prema sljedećem statusu:

- **Aktivno** Uređaji koji aktivno izvješćuju servisu Defender for Endpoint.
- **Pogrešno konfigurirano** Uređaji koji djelomično izvješćuju o podacima senzora servisu Defender for Endpoint, ali imaju konfiguracijske pogreške koje je potrebno ispraviti. Pogrešno konfigurirani uređaji mogu imati jedan ili kombinaciju sljedećih problema:

    - Nema podataka o senzoru – uređaji su prestali slati podatke senzora. S uređaja se mogu pokrenuti ograničena upozorenja.
    - Oštećena komunikacija – smanjena je mogućnost komunikacije s uređajem. Slanje datoteka radi dubinske analize, blokiranje datoteka, izolacija uređaja od mreže i drugih akcija koje zahtijevaju komunikaciju s uređajem možda neće funkcionirati.
- **Neaktivno** Uređaji koji su prestali s izvješćivanjem o servisu Defender for Endpoint.

Cijeli popis možete preuzeti u CSV obliku pomoću značajke Izvoz.

Dodatne informacije potražite u članku Provjera [stanja senzora u programu Microsoft Defender za krajnju točku](/microsoft-365/security/defender-endpoint/check-sensor-status).

Dodatne informacije o tome što je uzrokovalo neaktivnost ili pogrešno konfiguriranje uređaja potražite u članku Rješavanje nezdravih [senzora u programu Microsoft Defender za krajnju točku](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).
