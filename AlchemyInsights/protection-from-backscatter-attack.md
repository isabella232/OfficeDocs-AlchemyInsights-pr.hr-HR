---
title: Zaštita od napada na Backscatter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035077"
---
# <a name="protection-from-backscatter-attack"></a>Zaštita od napada na Backscatter

Backscatter je izvješće o neisporuci (koje se nazivaju i poruke NDRs ili Bounce) koje primate za poruke koje niste slali. Spameri Forge (podvala) **iz:** adresa svojih poruka, a često koriste i stvarne adrese e-pošte da bi mogli prenijeti vjerodostojnost porukama. Dakle, kada spameri neminovno pošalju poruke nepostojećim primateljima, odredišni poslužitelj e-pošte u suštini je prevaren da vrati neisporučenu poruku u NDR u falsificirani pošiljatelj iz **:** adresa.

Dodatne informacije možete pronaći u odjeljku [Backscatter u programu eeiop](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).

**Omogućavanje zaštite Pozadinnog raspršivanja**

Da biste omogućili zaštitu od povratnog raspršivanja, slijedite put u nastavku.

**Protection.Office.com > upravljanje prijetnjama > Policy > antispam > odaberite pravilnik o filtriranju neželjene pošte i uređivanje pravilnika > svojstva neželjene pošte > označiti kao neželjena pošta > NDR odzivu > postavite ga na "uključeno"**

Ako smatrate da je račun ugrožen, pročitajte sljedeće:

- [Odgovaranje na kompromitirani račun e-pošte](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [Uklanjanje blokiranih korisnika s portala ograničenog korisnika u sustavu Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



