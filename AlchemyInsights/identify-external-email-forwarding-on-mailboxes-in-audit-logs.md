---
title: Identificiranje prosljeđivanje vanjski e-pošte na poštanskim sandučićima u zapisnika nadzora
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 7fb2c161c558a7eb961f86ca2b86e33750d902fd
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32417204"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Prepoznati prilikom prosljeđivanja e-pošte vanjskog konfiguriran na poštanski sandučići

Kada korisnik konfigurira prosljeđivanje vanjski e-pošte u poštanski sandučić, aktivnost se nadzirati kao dio cmdlet **Set poštanskog sandučića** . Možete vidjeti aktivnosti pomoću pretraživanje zapisnika nadzora u & usklađenosti centar sigurnosti.

1. Prijavite se u sustav [Office 365 sigurnosne & usklađenosti centar](https://protection.office.com/)

2. Kliknite **za pretraživanje i istraživanja** i odaberite **Pretraživanje zapisnika nadzora**.

3. Odaberite raspon datum u polja **Datum početka** i **Datum završetka** . Ne morate navesti korisničko ime. Provjerite je li polje **aktivnosti** postavljeno na **Pokaži rezultate za sve aktivnosti**.

4. Kliknite **Pretraži**.

U rezultatima pritisnite **Rezultate filtra** i upišite **Skup poštanskog sandučića** u okvir filtar aktivnost. Odaberite zapis nadzora u rezultatima. Potpaleta **pojedinosti** pritisnite **Dodatne informacije**. Imate pogledajte detalje svakog nadzora zapisa da biste ustanovili Ako aktivnost odnosi prosljeđivanja e-pošte.

- **ID objekta**: vrijednost pseudonim poštanskog sandučića koja je izmijenjena.

- **Parametri**: _ForwardingSmtpAddress_ označava adresu e-pošte za cilj.

- **Korisnički ID**: korisnika koji je konfiguriran prosljeđivanja e-pošte na poštanskog sandučića u polju **ID objekta** .

Za dodatne informacije pogledajte [Determining tko postaviti poštanski sandučić za prosljeđivanje e-pošte](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
