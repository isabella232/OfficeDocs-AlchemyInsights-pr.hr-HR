---
title: Više objekata ima istu adresu e-pošte kao i identitet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: 5866d182cb2e97e37bc6df87e05fb6ef55bfed1d36f9daa95b7b8993a509e2dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011904"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Više objekata ima istu adresu e-pošte kao i identitet

**Više objekata**

Jedan od najčešćih razloga te pogreške nije moguće pravilno usmjeravati zahtjev za Outlook Web Access u prisutnosti više objekata koji imaju istu adresu e-pošte kao i identitet. Da biste pronašli te objekte, pokrenite sljedeće naredbe:

· Get-Recipient <email address>

· Get-User <email address>

· Get-User <email address> -SoftDeletedUser

· Get-Contact <email address>

· Get-Mailbox <email address> -PublicFolder

· Get-Mailbox <email address> -IncludeSoftDeletedMailbox

· Get-Mailbox <email address> -InactiveMailboxOnly

Da biste riješili problem, uklonite više objekata s istim identitetom e-pošte i provjerite postoji li jedan objekt s određenim identitetom e-pošte i je li njegova vrsta primatelja UserMailbox.

**Ista se adresa koristi za poslovne i korisničke poštanske sandučiće**

Drugi je uzrok kada se ista adresa koristi za poslovne i korisničke poštanske sandučiće. U tom slučaju korisnik mora promijeniti primarni korisnički pseudonim dok Cafe ne podržava taj scenarij. To je trajna pogreška koja ne nestane bez intervencije.

Detalje potražite u članku [Promjena adrese e-pošte ili telefonskog broja za Microsoftov račun.](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account)