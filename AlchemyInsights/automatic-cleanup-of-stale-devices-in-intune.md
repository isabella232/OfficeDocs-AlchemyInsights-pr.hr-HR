---
title: Automatsko čišćenje ustajalih uređaja u programu Intune
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
ms.openlocfilehash: 49a15132253c59189e343aeaa1c11d450b344896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715013"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Automatsko čišćenje ustajalih uređaja u programu Intune

Intune administratore omogućuje konfiguriranje vremenskog intervala između 90 i 270 dana, nakon čega se ustajali uređaji uklanjaju iz servisa. Ta je postavka široko organizacijska i kada se aktivira odmah stupa na sebi. Svi uređaji koji nisu potvrđeni u sustavu Intune Server za razdoblje koje prelazi postavku trajno se brišu.

**Notes** Samo objekti MDM uređaja imaju pravo na ovu akciju čišćenja. Ako su isključeni samo objekti uređaja.

Dodatne informacije o tome kada uređaj postane podoban za brisanje na temelju postavke čišćenja uređaja i njegova "stanja":

Postavka: **Brisanje uređaja nakon posljednjeg datuma prijave: da (neka vrijednost (N) u određenim danima)**

- Na temelju vrijednosti (N) konfiguriranih u postavci, poslužitelj za Intune briše uređaj u navedenim danima kada se zadnji put uspješno prijavljuje.

Postavka:  **Brisanje uređaja nakon posljednjeg datuma prijave: ne**

- 180 dana nakon isteka certifikata uređaja i nije obnovljen, uređaj se briše.

**Notes** U oba slučaja uređaj mora biti uspješno registriran u programu Intune. Registracija se javlja prilikom prvog provjere uređaja pomoću servisa Intune.

Ako se uređaj uspješno uključi, ali ne postane registriran, uređaj se briše 270 dana nakon upisa. (90 dana da biste označili uređaj kao ukinut, a zatim još 180 dana da biste izbrisali zapis.)

U konzoli za Intune ne postoje mehanizmi za uspostavljanje datuma isteka certifikata uređaja za bilo koji uređaj.