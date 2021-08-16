---
title: Saznajte tko je postavio prosljeđivanje na poštanskom sandučiću i kako
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
ms.openlocfilehash: 6243e787bb6b51f26cf22782d9ec80f946430b864f53de7ea626b7166a674d2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988171"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Saznajte tko je postavio prosljeđivanje na poštanskom sandučiću i kako

Ako je vanjsko prosljeđivanje postavljeno na poštanski sandučić, aktivnost se nadjača kao dio cmdleta Set-Mailbox. Evo kako pronaći aktivnost u zapisniku nadzora:

1. Idite na [centar Office 365 sigurnosti & usklađenosti](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Odaberite **Pretraživanje** >  **pretraživanja zapisnika nadzora**.
    > [!NOTE]
    > Ako vidite obavijest da morate uključiti nadzor, odmah je uključite. Ako ta značajka nije uključena, rezultati pretraživanja neće moći povući podatke iz prethodnih datuma.
1. Provjerite je li **polje Aktivnosti** postavljeno na Prikaz rezultata za **sve aktivnosti** (zadano). Navedite raspon datuma. Ne morate navesti korisničko ime.
1. Odaberite **Pretraživanje**. Aktivnosti se prikazuju u odjeljku **Rezultati**.
1. Odaberite **Filtriraj rezultate**, a zatim u **polje Filtar** aktivnosti unesite **Postavi** poštanski sandučić. Time se vraćaju sve **aktivnosti postavljenog poštanskog** sandučića.
1. Da biste pogledali pojedinosti, odaberite aktivnost, a zatim dodatne **informacije**. U **odjeljku** Parametri možete vidjeti adresu e-pošte za prosljeđivanje koja je postavljena na poštanskom sandučiću. **UserID predstavlja** korisnika koji je postavio vanjsko prosljeđivanje u poštanskom sandučiću.
Dodatne informacije potražite u članku Pretraživanje [zapisnika Office 365 da biste otklonili uobičajene scenarije](https://go.microsoft.com/fwlink/?linkid=2103944).