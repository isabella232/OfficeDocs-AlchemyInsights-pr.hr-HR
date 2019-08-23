---
title: Identificiranje prosljeđivanje vanjski e-pošte na poštanskim sandučićima u zapisnika nadzora
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7defd0902e8c8bebae9c7bfee72c3199cbc1909f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539093"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Prepoznati prilikom prosljeđivanja e-pošte vanjskog konfiguriran na poštanski sandučići

Kada korisnik Office 365 konfigurira prosljeđivanje vanjski e-pošte na poštanski sandučić, aktivnost se nadzirati kao dio cmdlet **Set poštanskog sandučića** . Možete vidjeti aktivnosti pomoću pretraživanje zapisnika nadzora u & usklađenosti centar sigurnosti.

1. Prijavite se u sustav [Office 365 sigurnosne & usklađenosti centar](https://protection.office.com/).

2. Idi na **pretraživanje** > stranicu za**pretraživanje zapisnika nadzora** .

3. Odaberite raspon datum u polja **Datum početka** i **Datum završetka** . Ne morate navesti korisničko ime. Provjerite je li polje **aktivnosti** postavljeno na **Pokaži rezultate za sve aktivnosti**.

4. Kliknite **Pretraži**.

U rezultatima pritisnite **Rezultate filtra** i upišite **Skup poštanskog sandučića** u okvir filtar aktivnost. Odaberite zapis nadzora u rezultatima. Potpaleta **pojedinosti** pritisnite **Dodatne informacije**. Imate pogledajte detalje svakog nadzora zapisa da biste ustanovili Ako aktivnost odnosi prosljeđivanja e-pošte.

- **ID objekta**: vrijednost pseudonim poštanskog sandučića koja je izmijenjena.

- **Parametri**: _ForwardingSmtpAddress_ označava adresu e-pošte za cilj.

- **Korisnički ID**: korisnika koji je konfiguriran prosljeđivanja e-pošte na poštanskog sandučića u polju **ID objekta** .

Za dodatne informacije pogledajte [Determining tko postaviti poštanski sandučić za prosljeđivanje e-pošte](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
