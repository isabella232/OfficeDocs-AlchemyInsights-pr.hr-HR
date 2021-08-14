---
title: Automatsko čišćenje stalenih uređaja u programu Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 905881f08ace7afae871ac48fa30ed1a0f15d13972cdff299a6694ca2eafc9cc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53997055"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Automatsko čišćenje stalenih uređaja u programu Intune

Intune administratoru omogućuje konfiguriranje vremenskog intervala između 90 i 270 dana, nakon čega se iz servisa uklanjaju stale uređaji. Ta je postavka široka i kada se aktivira, odmah će aktivirate. Svi uređaji koji nisu provjereni na intune poslužitelju tijekom razdoblja koje premašuju postavku trajno se brišu.

**Napomena** Za tu akciju čišćenja ispunjavaju samo objekti MDM uređaja. Izuzimaju se samo objekti uređaja EAS.

Dodatne informacije o tome kada uređaj ispunjava uvjete za brisanje na temelju postavke čišćenja uređaja i njegova "stanja":

Postavka: **brisanje uređaja nakon zadnjeg datuma prijave: Da (neka vrijednost (N) u navedenim danima)**

- Na temelju vrijednosti (N) konfigurirane u postavki, servis Intune briše uređaj u navedenim danima nakon uspješne provjere.

Postavka:  **Brisanje uređaja nakon zadnjeg datuma prijave: Ne**

- 180 dana nakon isteka certifikata uređaja i ne obnovi se, uređaj se briše.

**Napomena** U oba slučaja uređaj mora biti uspješno registriran u programu Intune. Registracija se odvija tijekom prve provjere uređaja pomoću servisa Intune.

Ako se uređaj uspješno prijavi u Intune, ali ne postane registriran kao Intune, uređaj se briše 270 dana nakon registracije. (90 dana da biste uređaj označili kao opozvan, a zatim još 180 dana da biste izbrisali zapis.)

Trenutno na konzoli Intune trenutno ne postoji mehanizam za utvrđivanje datuma isteka certifikata uređaja za bilo koji uređaj.