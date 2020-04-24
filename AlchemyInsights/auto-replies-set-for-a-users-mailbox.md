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
ms.openlocfilehash: 4ffe8d77dad7db5fd5806fe879cf4934e5ca7c4a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/23/2020
ms.locfileid: "43788874"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Postavljanje automatskih odgovora za poštanski sandučić korisnika

**Metoda 1**

1. Prijavite se na portal sustava Microsoft 365.

2. Idite na **Korisnici > Aktivni korisnici** (ili **Grupe > Zajednički poštanski sandučići** ako ga postavite na zajednički poštanski sandučić).

3. Odaberite korisnika s poštanskim sandučićem sustava Microsoft Exchange.

4. Na izborniku s potpaletom na desnoj strani idite na **Postavke pošte > Automatski odgovori** (ako se radi o zajedničkom poštanskom sandučiću, samo kliknite **Automatski odgovori** na potpaleti).

**Metoda 2**

1. Prijavite se na portal za administratore sustava Microsoft 365 pomoću administratorskih vjerodajnica.

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
