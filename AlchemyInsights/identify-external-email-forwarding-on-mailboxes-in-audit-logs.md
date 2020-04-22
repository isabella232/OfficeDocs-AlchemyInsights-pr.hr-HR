---
title: Prepoznavanje vanjskog prosljeđivanja e-pošte na poštanskim sandučićima u nadzornim zapisnicima
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
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716452"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Prepoznavanje kada je vanjsko prosljeđivanje e-pošte konfigurirano na poštanskim sandučićima

Kada korisnik sustava Microsoft 365 konfigurira prosljeđivanje vanjske e-pošte na poštanskom sandučiću, aktivnost se nadzire kao dio cmdleta **Set-Mailbox.** Aktivnost možete vidjeti pomoću pretraživanja zapisnika nadzora u centru za & sigurnosti.

1. Prijavite se u Centar za [sigurnost sustava Microsoft 365 & .](https://protection.office.com/)

2. Idite na stranicu **za** > **pretraživanje zapisnika nadzora** pretraživanja.

3. Odaberite datumski raspon u poljima **Datum početka** i **Datum završetka.** Ne morate navesti korisničko ime. Provjerite je li polje **Aktivnosti** postavljeno na **Prikaži rezultate za sve aktivnosti**.

4. Kliknite **Pretraživanje**.

U rezultatima kliknite **Filtriraj rezultate** i u okvir filtra aktivnosti upišite Postavi **poštanski sandučić.** Odaberite zapis nadzora u rezultatima. U potpaleti **Detalji** kliknite **Dodatne informacije**. Morate pogledati pojedinosti svakog zapisa nadzora da biste utvrdili je li aktivnost povezana s prosljeđivanjem e-pošte.

- **ObjectId**: Vrijednost pseudonima izmijenjenog poštanskog sandučića.

- **Parametri**: _ForwardingSmtpAddress_ označava ciljnu adresu e-pošte.

- **UserId**: Korisnik koji je konfigurirao prosljeđivanje e-pošte na poštanskom sandučiću u polju **ObjectId.**

Dodatne informacije potražite u [odjeljku Određivanje tko je postavio prosljeđivanje e-pošte za poštanski sandučić](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
