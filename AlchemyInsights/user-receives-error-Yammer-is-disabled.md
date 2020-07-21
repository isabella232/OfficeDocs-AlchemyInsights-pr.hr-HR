---
title: Korisnik prima pogrešku AADSTS7000112 Yammer je onemogućen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197794"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>Korisnik prima pogrešku AADSTS7000112 Yammer je onemogućen

Ako primite poruku o pogrešci "AADSTS7000112: aplikacija '00000005-0000-0ff1-ce00-00000000000000000000000000000000000000000000000000000"(Yammer) je onemogućena", postoji problem s glavnim servisom unutar Azure AD. Administrator je možda onemogućio glavnu servisnu karticu da bi blokirao pristup servisu Yammer.

Onemogućivanje principala servisa se ne preporučuje i može uzrokovati dodatne probleme. Dodatne informacije o podržanom pristupu za blokiranje korisničkog pristupa servisu Yammer potražite u odjeljku [Isključivanje pristupa servisu Yammer za korisnike sustava Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).  

Da biste ispravili taj problem na portalu Azure i vratili korisnički pristup servisu Yammer:

1.  Otvorite stranicu Azure Active Directory i odaberite **Enterprise aplikacije** u odjeljku **Upravljanje** u lijevom navigacijskom oknu.
3.  U okvir za pretraživanje upišite **Office 365 Yammer** i odaberite naziv aplikacije da biste otvorili postavke.
4.  U lijevom navigacijskom oknu odaberite **Svojstva** u odjeljku **Upravljanje.**
5.  Postavite vrijednost **omogućeno za korisnike za prijavu ?** **Yes** **Save**
6.  Ponovno se prijavite na Yammer. Možda ćete morati očistiti kolačiće.

Umjesto toga pokrenite PowerShell naredbe da biste postavili vrijednost. Dodatne informacije potražite [u odjeljku Pogreška "Nažalost, ali imamo poteškoća s prijavom" kada kliknete pločicu Yammer u sustavu Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365). 