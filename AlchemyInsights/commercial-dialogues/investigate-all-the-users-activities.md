---
title: Istraživanje svih aktivnosti korisnika
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 016f4b1caa05cb26d1e6795551b64737d4cb64a5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332335"
---
# <a name="investigate-all-the-users-activities"></a>Istraživanje svih aktivnosti korisnika

Evo kako to učiniti:

1. Učinite jednu od sljedećih akcija:
   - U Centar za usklađenost okruženja Microsoft 365 na <https://compliance.microsoft.com> idite na **Nadzor** \> **rješenja**. Možete i izravno pristupiti stranici **Nadzor** pomoću sustava <https://compliance.microsoft.com/auditlogsearch> .
   - Na portalu Microsoft 365 Defender idite <https://security.microsoft.com> na **Nadzor**. Možete i izravno pristupiti stranici **Nadzor** pomoću sustava <https://security.microsoft.com/auditlogsearch> .

    **Napomena:** ako vidite obavijest da morate uključiti značajku, odmah je uključite. Ako značajka nije uključena, rezultati pretraživanja neće moći povući podatke iz prethodnih datuma.

2. Na kartici **Pretraživanje** na **stranici Nadzor** konfigurirajte sljedeće postavke:
   - **Raspon datuma i vremena:** odaberite raspon datuma/vremena u **okvirima Početak** **i** Kraj.
   - **Aktivnosti**: ako vas zanima određena aktivnost, odaberite je s popisa; u suprotnom zadana vrijednost **Prikaži rezultate za sve aktivnosti vraća** sve aktivnosti.
   - **Korisnici:** prihvatite praznu zadanu vrijednost da biste vratili rezultate za sve korisnike ili unesite jednog ili više korisnika.

3. Kada završite, kliknite **Pretraživanje**. Aktivnosti se prikazuju na novoj stranici **pretraživanja nadzora.** Vidjet ćete **IP** adresu, **korisnik i** **naziv** aktivnosti.

4. Da biste preuzeli  rezultate, odaberite \> **Izvezi preuzmi sve rezultate**.

5. Odaberite aktivnost u rezultatima da biste otvorili letak s detaljima.

Dodatne informacije potražite u članku Pretraživanje [zapisnika nadzora da biste istražili uobičajene probleme s podrškom](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
