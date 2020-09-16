---
title: Više objekata ima istu adresu e-pošte kao identitet
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
ms.openlocfilehash: 05fb43133bc68b71ccdbab44d28679a1f659e762
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724607"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Više objekata ima istu adresu e-pošte kao identitet

**Više objekata**

Jedan od običnih razloga te pogreške ne može pravilno usmjeravati zahtjev za Outlook Web Access u prisustvu više objekata koji imaju istu adresu e-pošte kao identitet. Da biste pronašli ove objekte, pokrenite sljedeće naredbe:

· Dohvaćanje primatelja <email address>

· Dohvaćanje korisnika <email address>

· Nabavite-user <email address> -softdeleteduser

· Dohvaćanje kontakta <email address>

· Nabavite-Mailbox <email address> -publifolder

· Nabavite-Mailbox <email address> – includesoftdeletedmailbox

· Dohvaćanje poštanskog sandučića <email address> -inactivemailboxonly

Da biste riješili problem, uklonite više objekata s istim identitetom e-pošte i provjerite postoji li jedan objekt s određenim identitetom e-pošte te je li njegova vrsta primatelja UserMailbox.

**Ista adresa koristi se za poštanske sandučiće tvrtke i potrošača**

Drugi je uzrok kada se ista adresa koristi za poslovne i potrošačke poštanske sandučiće. U ovom slučaju korisnik mora promijeniti pseudonim primarnog potrošača dok Cafe ne podržava ovaj scenarij. To je trajna pogreška koja ne nestaje bez intervencije.

Pojedinosti potražite u članku [Promjena adrese e-pošte ili telefonskog broja za Microsoftov račun](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).