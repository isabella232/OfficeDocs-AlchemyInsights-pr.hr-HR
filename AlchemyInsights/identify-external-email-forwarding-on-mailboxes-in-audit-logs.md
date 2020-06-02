---
title: Prepoznavanje vanjskog prosljeđivanja e-pošte na poštanskim sandučićima u zapisnikima nadzora
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 592eb92e4b0fe0f9da2fa20bb93ffa4fbbb76662
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508944"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Prepoznavanje konfiguriranja vanjskog prosljeđivanja e-pošte na poštanskim sandučićima

Kada korisnik microsoft 365 konfigurira vanjsko prosljeđivanje e-pošte na poštanskom sandučiću, aktivnost se nadzire kao dio cmdleta **Set-Mailbox.** Aktivnost možete vidjeti pomoću pretraživanja zapisnika nadzora u centru za usklađenost sigurnosnih &.

1. Prijavite se u Centar za [usklađenost sa sigurnosnim & sustava Microsoft 365](https://protection.office.com/).

2. Idite **Search**na  >  stranicu za pretraživanje**zapisnika nadzora** pretraživanja.

3. Odaberite datumski raspon u poljima **Datum početka** i **Datum završetka.** Ne morate navesti korisničko ime. Provjerite je li polje **Aktivnosti** postavljeno na **Prikaži rezultate za sve aktivnosti**.

4. Kliknite **Pretraži**.

U rezultatima kliknite **Filtriraj rezultate** i u okvir filtar aktivnosti upišite **Set-Mailbox.** Odaberite zapis nadzora u rezultatima. U potpaleti **Detalji** kliknite **Dodatne informacije**. Morate pogledati detalje svakog zapisa nadzora da biste utvrdili je li aktivnost povezana s prosljeđivanjem e-pošte.

- **ObjectId**: Vrijednost pseudonima koji je izmijenjen.

- **Parametri**: _ForwardingSmtpAddress_ označava ciljnu adresu e-pošte.

- **UserId**: Korisnik koji je konfigurirao prosljeđivanje e-pošte na poštanskom sandučiću u polju **ObjectId.**

Dodatne informacije potražite [u odjeljku Određivanje tko je postavio prosljeđivanje e-pošte za poštanski sandučić](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
