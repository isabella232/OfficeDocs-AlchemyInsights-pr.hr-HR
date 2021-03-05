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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481204"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Saznajte tko je postavio prosljeđivanje na poštanskom sandučiću i kako

Ako je vanjsko prosljeđivanje postavljeno na poštanski sandučić, aktivnost se nadzire kao dio cmdleta Set-Mailbox. Slijede upute za pronalaženje aktivnosti u zapisniku nadzora:

1. Otvorite centar za [sigurnost & sustava Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Odaberite **Pretraži pretragu** >  **zapisnika nadzora**.
    > [!NOTE]
    > Ako vam se prikaže obavijest da morate uključiti nadzor, nastavite i uključite ga odmah. Ako ta značajka nije uključena, rezultati pretraživanja neće moći povući podatke iz prethodnih datuma.
1. Provjerite je li polje **aktivnosti** postavljeno tako da **prikazuje rezultate za sve aktivnosti** (zadano). Navedite raspon datuma. Ne morate navesti korisničko ime.
1. Odaberite **Pretraživanje**. Aktivnosti se prikazuju u odjeljku **Rezultati**.
1. Odaberite **Filtriraj rezultate**, a zatim u polje Filtar **aktivnosti** unesite **skup poštanskih sandučića** . Time se vraća sve aktivnosti **skupa poštanskih sandučića** .
1. Da biste pogledali detalje, odaberite aktivnost, a zatim odaberite **Dodatne informacije**. U odjeljku **Parametri** možete vidjeti adresu e-pošte za prosljeđivanje koja je postavljena na poštanskom sandučiću. **Userid** predstavlja korisnika koji je postavio vanjsko prosljeđivanje na poštanskom sandučiću.
Dodatne informacije potražite u članku [pretraživanje zapisnika nadzora sustava Office 365 radi otklanjanja običnih scenarija](https://go.microsoft.com/fwlink/?linkid=2103944).