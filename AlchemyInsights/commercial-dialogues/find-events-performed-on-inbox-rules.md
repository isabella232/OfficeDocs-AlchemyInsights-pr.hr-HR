---
title: Pronalaženje događaja izvedenih na pravilima ulazne pošte
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
ms.openlocfilehash: 626bd7515270f03e1560a3ed637e7bc60b374c5525527205d5f6775e4758f07a
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57882627"
---
# <a name="find-events-performed-on-inbox-rules"></a>Pronalaženje događaja izvedenih na pravilima ulazne pošte

Kada se pravila ulazne pošte stvaraju, mijenjaju ili brišu, događaji se bilježe u zapisnik nadzora. Evo kako ih pregledati:

1. Učinite jednu od sljedećih akcija:
   - U Centar za usklađenost okruženja Microsoft 365 na <https://compliance.microsoft.com> idite na **Nadzor** \> **rješenja**. Možete i izravno pristupiti stranici **Nadzor** pomoću sustava <https://compliance.microsoft.com/auditlogsearch> .
   - Na portalu Microsoft 365 Defender , <https://security.microsoft.com> idite na **Nadzor**. Možete i izravno pristupiti stranici **Nadzor** pomoću sustava <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Ako vidite obavijest da morate uključiti nadzor, odmah je uključite. Ako ta značajka nije uključena, rezultati pretraživanja neće moći povući podatke iz prethodnih datuma.

2. Na kartici **Pretraživanje** na **stranici Nadzor** konfigurirajte sljedeće postavke:
   - **Raspon datuma i vremena:** odaberite raspon datuma/vremena u **okvirima Početak** **i** Kraj.
   - **Aktivnosti**: Odaberite **Novo-ulazna poštaRule Stvori pravilo ulazne pošte iz Outlook Web App**

3. Kada završite, kliknite **Pretraživanje**. Aktivnosti se prikazuju na novoj stranici **pretraživanja nadzora.**

4. Odaberite aktivnost u rezultatima da biste otvorili letak s detaljima. U **odjeljku** Parametri možete vidjeti naziv pravila, postavljene uvjete i akcije koje će pravilo poduzeti.

Dodatne informacije potražite u članku Pretraživanje [zapisnika nadzora da biste istražili uobičajene probleme s podrškom](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
