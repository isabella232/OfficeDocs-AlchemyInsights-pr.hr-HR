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
ms.openlocfilehash: 48634fad8f573e3a7c38cac299bb95ec90814f5c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331151"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Prepoznavanje kada je vanjsko prosljeđivanje e-pošte konfigurirano na poštanskim sandučićima

Kada korisnik Microsoft 365 vanjsko prosljeđivanje e-pošte na poštanskom sandučiću, aktivnost se nadzirana provodi u sklopu cmdleta **Set-Mailbox.** Aktivnost možete vidjeti pomoću pretraživanja zapisnika nadzora. Evo kako to učiniti.

1. Učinite nešto od sljedećeg:
   - U Centar za usklađenost okruženja Microsoft 365 na <https://compliance.microsoft.com> idite na **Nadzor** \> **rješenja**. Možete i izravno pristupiti stranici **Nadzor** pomoću sustava <https://compliance.microsoft.com/auditlogsearch> .
   - Na portalu Microsoft 365 Defender idite <https://security.microsoft.com> na **Nadzor**. Možete i izravno pristupiti stranici **Nadzor** pomoću sustava <https://sip.security.microsoft.com/auditlogsearch> .

2. Na **stranici** Nadzor provjerite je li **odabrana** kartica Pretraživanje, a zatim konfigurirajte sljedeće postavke:
   - Odaberite raspon datuma/vremena u **okvirima Početak** **i** Kraj.
   - Provjerite sadrži **li okvir** Aktivnosti Prikaz rezultata za **sve aktivnosti**.

3. Kada završite, kliknite **Pretraživanje**. Aktivnosti se prikazuju na novoj stranici **pretraživanja nadzora.**

4. U rezultatima kliknite Filtriraj rezultate **i** u okvir filtar aktivnosti **upišite Set-Mailbox.**

5. Odaberite zapis nadzora u rezultatima. U **podotočiću** Detalji kliknite **Dodatne informacije**. Da biste utvrdili je li aktivnost povezana s prosljeđivanjem e-pošte, morate pogledati pojedinosti o svakom zapisu nadzora.

   - **ObjectId**: vrijednost pseudonima izmijenjenog poštanskog sandučića.
   - **Parametri:** _ForwardingSmtpAddress označava_ odredišnu adresu e-pošte.
   - **UserId**: korisnik koji je konfigurirao prosljeđivanje e-pošte u poštanskom sandučiću u **polju ObjectId.**

Dodatne informacije potražite u članku [Određivanje tko je postavio prosljeđivanje e-pošte za poštanski sandučić.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
