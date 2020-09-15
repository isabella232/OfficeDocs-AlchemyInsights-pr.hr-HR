---
title: Prepoznavanje vanjskih prosljeđivanja e-pošte u poštanskom sandučiću u evidenciji nadzora
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696289"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Određivanje kada je vanjsko prosljeđivanje e-pošte konfigurirano na poštanskim sandučićima

Kada korisnik Microsoft 365 u poštanskom sandučiću konfigurira vanjsku prosljeđivanje e-pošte, aktivnost se nadzire kao dio cmdleta **Set-Mailbox** . Aktivnost možete vidjeti pomoću pretraživanja zapisnika nadzora u centru za sigurnost & usklađenosti.

1. Prijavite se u [centar za sigurnost & sustava Microsoft 365](https://protection.office.com/).

2. Idite na stranicu **Search**  >  **pretraživanja zapisnika nadzora** pretraživanja.

3. Odaberite raspon datuma u poljima **Datum početka** i **Datum završetka** . Ne morate navesti korisničko ime. Provjerite je li polje **aktivnosti** postavljeno **tako da pokazuje rezultate za sve aktivnosti**.

4. Kliknite **Pretraživanje**.

U rezultatima kliknite **Filtriraj rezultate** , a zatim u okvir Filtar aktivnosti upišite **skup poštanskih sandučića** . Odaberite zapis nadzora u rezultatima. U nastavku **Pojedinosti** kliknite **više informacija**. Da biste utvrdili je li aktivnost povezana s prosljeđivanjem e-pošte, morate pogledati pojedinosti o svakom zapisu nadzora.

- **Objektand**: vrijednost pseudonima poštanskog sandučića koji je promijenjen.

- **Parametri**: _forwardingsmtpaddress_ označava ciljnu adresu e-pošte.

- **Userid**: korisnik koji je konfigurirao prosljeđivanje e-pošte na poštanskom sandučiću u polju **Objekt** .

Dodatne informacije potražite u članku [određivanje tko je postavio prosljeđivanje e-pošte za poštanski sandučić](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
