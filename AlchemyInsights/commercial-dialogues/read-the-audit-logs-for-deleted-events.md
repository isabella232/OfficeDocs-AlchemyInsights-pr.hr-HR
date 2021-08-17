---
title: Čitanje zapisnika nadzora za izbrisane događaje
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: ef4cbb0b778b22fba83d22d5056449c2281c5a2947ecb41ce8f808a4d1132426
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896007"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Čitanje zapisnika nadzora za izbrisane događaje

Evo kako to učiniti:

1. Učinite jednu od sljedećih akcija:
   - U Centar za usklađenost okruženja Microsoft 365 na <https://compliance.microsoft.com> idite na **Nadzor** \> **rješenja**. Možete i izravno pristupiti stranici **Nadzor** pomoću sustava <https://compliance.microsoft.com/auditlogsearch> .
   - Na portalu Microsoft 365 Defender , <https://security.microsoft.com> idite na **Nadzor**. Možete i izravno pristupiti stranici **Nadzor** pomoću sustava <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Ako vidite obavijest da morate uključiti značajku, odmah je uključite. Ako značajka nije uključena, rezultati pretraživanja neće moći povući podatke iz prethodnih datuma.

2. Na kartici **Pretraživanje** na **stranici Nadzor** konfigurirajte sljedeće postavke:
   - **Raspon datuma i vremena:** odaberite raspon datuma/vremena u **okvirima Početak** **i** Kraj.
   - **Aktivnosti**: **unesite Exchange poštanskog sandučića,** a zatim odaberite sljedeće vrijednosti:
     - **Izbrisane poruke iz mape Izbrisane stavke**
     - **Premještene poruke u mapu Izbrisane stavke**

       Kada završite, kliknite izvan okna da biste minimizirali **okno** Aktivnosti.

   - **Korisnici:** prihvatite praznu zadanu vrijednost da biste vratili rezultate za sve korisnike ili unesite jednog ili više korisnika.

3. Kada završite, kliknite **Pretraživanje**. Aktivnosti se prikazuju na novoj stranici **pretraživanja nadzora.**

4. Odaberite aktivnost u rezultatima da biste otvorili letak s detaljima. Dodatne informacije o izbrisanoj stavci, kao što su redak predmeta i mjesto stavke kada je izbrisana, prikazuju se u polju **Zahvaćeniitami.**

   > [!NOTE]
   > Izbrisane stavke ne možete vratiti pomoću značajke zapisnika nadzora. Da biste vratili izbrisane stavke, pogledajte [oporavak izbrisanih poruka e-pošte Outlook na webu](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11).

Dodatne informacije potražite u članku Pretraživanje [zapisnika nadzora da biste istražili uobičajene probleme s podrškom](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
