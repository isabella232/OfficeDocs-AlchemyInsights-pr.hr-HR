---
title: Outlook Desktop opoziv ili zamijeniti poruku e-pošte
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/15/2019
ms.locfileid: "36496103"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Opoziv ili zamjena poruke e-pošte programa Outlook

- Kao administrator, možete **opozvati poruke u ime korisnika pomoću PowerShell**. Ne možete se sjetiti poruka iz centra za administraciju.
- Možete se **prisjetiti samo poruka koje se šalju osobama u vašoj organizaciji**. Ako je poruka poslana na Gmail adresu, na primjer, ne možete ga opozvati.
- Možete se **prisjetiti samo poruka poslane iz outlooka 2016 na PC-ju**. Ako korisnik pošalje poruku pomoću programa Outlook za Mac ili Outlook na webu, ne možete ga opozvati.

Da biste opozvali ili zamijenili poruku e-pošte:

1. U oknu mape s lijeve strane prozora programa Outlook odaberite mapu poslane stavke.
1. Dvaput pritisnite poruku koju želite podsjetiti da biste je otvorili.
1. Odaberite karticu **poruka** , a zatim odaberite **Akcije** > **Opozovi ovu poruku**.
1. Odaberite **Izbriši nepročitanih kopija ove poruke** ili **izbrišite nepročitanih kopija i zamijenite novom porukom**, a zatim odaberite **u redu**.
1. Ako šaljete zamjensku poruku, sastavite poruku, a zatim odaberite **Pošalji**.
1. Uspjeh ili neuspjeh opoziv poruke ovisi o postavkama primatelja u programu Outlook. Za korake za provjeru opoziva pogledajte [ovaj članak](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Traženje i brisanje poruka e-pošte u organizaciji

- Ako niste globalni administrator, vaš račun mora biti dodan ulozi eDiscovery managera ili u ulozi za upravljanje pretraživanjem usklađenosti da biste potražili poruke. Da biste izbrisali poruke, morate se pridružiti grupi uloga za upravljanje organizacijom ili u ulozi upravljanja pretraživanjem i pročišćavanja. Dozvole za te uloge dodijeljene su u [centru za sigurnost i usklađenost](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Stvorite pretraživanje sadržaja](https://docs.microsoft.com/office365/securitycompliance/content-search) da biste pronašli poruku koju želite izbrisati.
- [Povežite se s PowerShell centrom za sigurnost i usklađenost](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Ako koristite multi-faktor provjeru autentičnosti, pogledajte [Povezivanje na Office 365 sigurnost i usklađenost centar PowerShell pomoću multi-faktor provjere autentičnosti](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).