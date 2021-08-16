---
title: Prepoznavanje vanjskog prosljeđivanja e-pošte u poštanskim sandučićima u zapisnicima nadzora
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
ms.openlocfilehash: 1e80917a323128ba23175651cdf4d892d7815a89c1223b654812c1b456c787da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028722"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Prepoznavanje kada je vanjsko prosljeđivanje e-pošte konfigurirano na poštanskim sandučićima

Kada korisnik Microsoft 365 vanjsko prosljeđivanje e-pošte na poštanskom sandučiću, aktivnost se nadjača kao dio cmdleta **Set-Mailbox.** Aktivnost možete vidjeti pomoću pretraživanja zapisnika nadzora u centru za & usklađenosti.

1. Prijavite se u [centar za Microsoft 365 usklađenost](https://protection.office.com/).

2. Idite na stranicu **pretraživanje**  >  **zapisnika nadzora pretraživanja.**

3. Odaberite raspon datuma u poljima **Datum početka** **i Datum** završetka. Ne morate navesti korisničko ime. Provjerite je **li polje** Aktivnosti postavljeno na Prikaz rezultata za **sve aktivnosti**.

4. Kliknite **Pretraživanje**.

U rezultatima kliknite Filtriraj rezultate **i** u okvir filtar aktivnosti **upišite Set-Mailbox.** Odaberite zapis nadzora u rezultatima. U **letci** Detalji kliknite **Dodatne informacije**. Da biste utvrdili je li aktivnost povezana s prosljeđivanjem e-pošte, morate pogledati pojedinosti o svakom zapisu nadzora.

- **ObjectId**: vrijednost pseudonima izmijenjenog poštanskog sandučića.

- **Parametri:** _ForwardingSmtpAddress označava_ odredišnu adresu e-pošte.

- **UserId**: korisnik koji je konfigurirao prosljeđivanje e-pošte u poštanskom sandučiću u **polju ObjectId.**

Dodatne informacije potražite u članku [Određivanje tko je postavio prosljeđivanje e-pošte za poštanski sandučić.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
