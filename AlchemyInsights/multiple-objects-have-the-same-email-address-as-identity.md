---
title: Više objekata ima istu adresu e-pošte kao i identitet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438801"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Više objekata ima istu adresu e-pošte kao i identitet

**Više objekata**

Jedan od uobičajenih razloga ove pogreške nije u mogućnosti ispravno usmjeriti zahtjev za Outlook Web Access u prisutnosti više objekata koji imaju istu adresu e-pošte kao i identitet. Da biste pronašli te objekte, pokrenite sljedeće naredbe:

· Primatelja<email address>

· Get-User<email address>

· Get-User <email address> -SoftDeletedUser

· Get-Kontakt<email address>

· Get-Mailbox <email address> -PublicFolder

· Get-Mailbox <email address> -IncludeSoftDeletedMailbox

· Get-Mailbox <email address> -InactiveMailboxSamo

Da biste riješili problem, uklonite više objekata s istim identitetom e-pošte i provjerite postoji li jedan objekt s određenim identitetom e-pošte i da je vrsta primatelja UserMailbox.

**Ista adresa koristi se za poslovne i potrošačke poštanske sandučiće**

Drugi uzrok je kada se ista adresa koristi za poslovne i potrošačke poštanske sandučiće. U tom slučaju korisnik mora promijeniti svoj primarni pseudonim za korisnike dok Cafe ne podržava ovaj scenarij. To je trajna pogreška koja ne prolazi bez intervencije.

Pojedinosti potražite [u odjeljku Promjena adrese e-pošte ili telefonskog broja microsoftova računa](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).