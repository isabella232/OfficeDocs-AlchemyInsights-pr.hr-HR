---
title: Automatsko čišćenje ustajalih uređaja u intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554772"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Automatsko čišćenje ustajalih uređaja u intune

Intune omogućuje admin konfigurirati vremenski interval između 90 i 270 dana, nakon čega ustajali uređaji su uklonjeni iz usluge. Ova postavka je organizacija široka i nakon što se aktivira stupa na snagu odmah. Svi uređaji koji nisu prijavljeni na Intune poslužitelj u razdoblju koje premašuje postavku trajno se brišu.

**Napomena:** Samo objekti MDM uređaja ispunjavaju uvjete za ovu akciju čišćenja. Isključeni su samo objekti uređaja EAS- a.

Za dodatne informacije o tome kada uređaj ispunjava uvjete za brisanje na temelju postavke čišćenja uređaja i njezina "stanja":

Postavka: **brisanje uređaja nakon zadnjeg datuma prijave: Da (neka vrijednost (N) u navedenim danima)**

- Na temelju vrijednosti (N) konfigurirane u postavci, servis Intune briše uređaj u navedenim danima nakon zadnje uspješne prijave.

Postavka: **brisanje uređaja nakon zadnjeg datuma prijave: Ne**

- 180 dana nakon isteka certifikata uređaja i ne obnavlja se, uređaj se briše.

**Napomena:** U oba slučaja uređaj mora biti uspješno registriran u Intuneu. Registracija se događa tijekom prve provjere uređaja s uslugom Intune.

Ako se uređaj uspješno upiše u Intune, ali ne postane registriran u Intuneu, uređaj se briše 270 dana nakon prijave. (90 dana za označavanje uređaja kao opozvanog, a zatim još 180 dana za brisanje zapisa.)

Trenutno ne postoji mehanizam u intune konzoli kako bi se utvrdio datum isteka certifikata uređaja za bilo koji uređaj.