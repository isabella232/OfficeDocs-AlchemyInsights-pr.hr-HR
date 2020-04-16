---
title: Postavljanje automatskih odgovora za poštanski sandučić
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: aeeb2e1e76fe602d2767b422797452fd1155fdd5
ms.sourcegitcommit: fdfd41c2bfb2d45003b3906e6469377384a91cb5
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2020
ms.locfileid: "43509482"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Postavljanje automatskih odgovora za poštanski sandučić korisnika

**Metoda 1**

1. Prijavite se na portal sustava Office 365.

2. Idite na **Korisnici > Aktivni korisnici** (ili **Grupe > Zajednički poštanski sandučići** ako ga postavite na zajednički poštanski sandučić).

3. Odaberite korisnika s poštanskim sandučićem sustava Microsoft Exchange.

4. Na izborniku s potpaletom na desnoj strani idite na **Postavke pošte > Automatski odgovori** (ako se radi o zajedničkom poštanskom sandučiću, samo kliknite **Automatski odgovori** na potpaleti).

**Metoda 2**

1. Prijavite se na portal za administratore sustava Office 365 s pomoću administratorskih vjerodajnica.

2. Proširite mogućnost **Administratorski centri**, pa kliknite **Exchange**.

3. Kliknite sliku u gornjem desnom kutu, kliknite **Drugi korisnik**, pa odaberite poštanski sandučić korisnika koji želite promijeniti.

4. Na lijevoj strani odaberite **Mogućnosti**, kliknite **Organiziranje e-pošte**, pa kliknite **Automatski odgovori.**

**Metoda 3**

Pokrenite sljedeći cmdlet u servisu PowerShell za Exchange Online:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

Dodatne informacije o tom cmdletu potražite u članku [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
