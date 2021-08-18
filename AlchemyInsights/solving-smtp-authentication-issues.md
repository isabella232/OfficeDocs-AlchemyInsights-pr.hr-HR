---
title: Omogućivanje provjere autentičnosti i otklanjanja poteškoća s SMTP-om
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 14f1454ad687b4d76cf419583b442685fa19b5a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321745"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>Omogućivanje provjere autentičnosti i otklanjanja poteškoća s SMTP-om

Ako želite omogućiti SMTP provjeru autentičnosti za poštanski sandučić ili vam se prikazuje pogreška "Klijent nije provjeren", "Provjera autentičnosti nije uspješna" ili pogreška "SmtpClientAuthentication" s kodom 5.7.57 ili 5.7.3 ili 5.7.139 kada pokušate prenijeti poruku e-pošte provjerom autentičnosti uređaja ili aplikacije s Microsoft 365, provedite sljedeće tri radnje da biste riješili problem:

1. Onemogućivanje [sigurnosnih zadanih postavki](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) za Azure tako da sigurnosne zadane **postavke omogućite** na **Ne**.

    a. Prijavite se na portal Azure kao administrator sigurnosti, administrator uvjetnog pristupa ili globalni administrator.<BR/>
    b. Idite na Azure Active Directory > **Svojstva**.<BR/>
    c. Odaberite **Upravljanje sigurnosnim zadanim postavkama**.<BR/>
    d. Postavite **Omogući zadane sigurnosne postavke** na **Ne**.<BR/>
    e. Odaberite **Spremi**.

2. [Omogućivanje slanja klijentskog SMTP-a](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) u licenciranom poštanskom sandučiću.

    a. Na Centar za administratore okruženja Microsoft 365 odaberite Aktivni **korisnici** pa odaberite korisnika.<BR/>
    b. Idite na karticu Pošta pa u odjeljku **Aplikacije za e-poštu** odaberite **Upravljanje aplikacijama za e-poštu**.<BR/>
    d. Provjerite je **li potvrđena provjera autentičnosti SMTP-a** (omogućeno).<BR/>
    e. Odaberite **Spremi promjene**.<BR/>

3. [Onemogućivanje višestruke provjere autentičnosti (MFA) u](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) licenciranom poštanskom sandučiću.

    a. Idite na Centar za administratore okruženja Microsoft 365, a zatim na lijevom navigacijskom izborniku **odaberite Korisnici**  >  **Aktivni korisnici**.<BR/>
    b. Odaberite **Višestruka provjera autentičnosti**.<BR/>
    c. Odaberite korisnika i **onemogućite višestruku provjeru**.<BR/>
