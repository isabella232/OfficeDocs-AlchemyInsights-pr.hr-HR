---
title: 451 4.7.0 Pogreška na privremenom poslužitelju. Pokušajte ponovno kasnije. PRX4
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: ce898981d053c8b5dc080ee83434bdacd7f02a636f0183293915bacdb48ba4ef
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812574"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 Pogreška na privremenom poslužitelju. Pokušajte ponovno kasnije. PRX4

Prilikom slanja e-pošte putem servisa Smarthost "smtp.office365.com" možete se sučeliti s problemom pomoću metode slanja SMTP klijenta i primiti pogrešku: "451 4.7.0 Pogreška Temporary server. Pokušajte ponovno kasnije. PRX4 je uglavnom privremen." 

Provjerite ne koristite li zajednički poštanski sandučić za slanje SMTP klijenta jer za slanje pošte putem metode slanja SMTP klijenta potreban je licencirani poštanski sandučić. No ako ne koristite zajednički poštanski sandučić i problem se i dalje pojavljuje, provjerite sljedeće:

1. Omogućivanje slanja klijentskog SMTP-a na licencirani poštanski sandučić koji se koristi pokretanjem ove naredbe komponente PowerShell:

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    OR

    1. Idite na Centar za administratore okruženja Microsoft 365 > **Aktivni korisnici** pa odaberite korisnika.
    1. Idite na karticu Pošta > **aplikacije e->** odaberite Upravljanje **aplikacijama za e-poštu**. 
    1. Provjerite je li **potvrđena postavka provjerenog SMTP-a** (omogućena).
    1. Odaberite **Spremi promjene**.
    
    Da biste omogućili SMTP provjeru autentičnosti za cijelu organizaciju, pokrenite ovu naredbu:

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **Napomena:** iz sigurnosnih razloga preporučuje se da smtp provjeru autentičnosti omogućite samo za poštanski sandučić koji se koristi. Postavka na razini korisnika nadjačava postavku razine tvrtke ili ustanove.

2. Onemogućivanje zadanih sigurnosnih postavki za Azure tako da se **sigurnosne zadane postavke aktiviraju** na **Ne:**

    1. Prijavite se na portal Azure kao administrator sigurnosti, administrator uvjetnog pristupa ili globalni administrator.
    1. Idite na Azure Active Directory >**  Svojstva pa** odaberite **Upravljanje sigurnosnim zadanim postavkama**.
    1. Postavite **prekidač Omogući zadane sigurnosne postavke** na **Ne**.
    1. Odaberite **Spremi**.

3. Onemogućivanje višestruke provjere autentičnosti (MFA) na licenciranom poštanskom sandučiću koji se koristi.

    1. Idite na Centar za administratore okruženja Microsoft 365, a zatim na lijevom navigacijskom izborniku **odaberite Korisnici**  >  **Aktivni korisnici**.
    1. Na **stranici Aktivni korisnici** odaberite **Višestruka provjera autentičnosti**.
    1. Odaberite korisnika i onemogućite **višestruku provjeru autentičnosti**.

