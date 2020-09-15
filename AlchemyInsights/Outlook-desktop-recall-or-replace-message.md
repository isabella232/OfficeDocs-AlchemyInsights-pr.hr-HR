---
title: Outlook desktopa opoziv ili zamjena poruke e-pošte
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663982"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Opoziv ili zamjena poruke e-pošte programa Outlook

- Kao administrator možete **opozvati poruke u ime korisnika pomoću komponente PowerShell**. Ne možete se prisjetiti poruka iz centra za administratore.
- Možete se **prisjetiti samo poruka koje se šalju osobama u vašoj tvrtki ili ustanovi**. Ako je poruka poslana na adresu servisa Gmail, na primjer, ne možete je opozvati.
- Možete se **prisjetiti samo poruka poslane iz programa Outlook 2016 na PC-ju**. Ako korisnik pošalje poruku pomoću programa Outlook za Mac ili Outlook na webu, ne možete je opozvati.

Opoziv ili zamjena poruke e-pošte:

1. U oknu s mapama na lijevoj strani prozora programa Outlook odaberite mapu poslane stavke.
1. Dvokliknite poruku koju želite opozvati da biste je otvorili.
1. Odaberite karticu **poruka** , a zatim odaberite **Akcije**  >  **Opoziv ove poruke**.
1. Odaberite **Izbriši nepročitane kopije ove poruke** ili **izbrišite nepročitane kopije i zamijenite je novom porukom**, a zatim odaberite **u redu**.
1. Ako šaljete zamjensku poruku, sastavite poruku, a zatim odaberite Send ( **Šalji**).
1. Uspjeh ili neuspjeh opoziv poruke ovisi o postavkama primatelja u programu Outlook. Upute za provjeru opoziv potražite u [ovom članku](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Traženje i brisanje poruka e-pošte u tvrtki ili ustanovi

- Ako niste globalni administrator, vaš račun mora biti dodan u ulogu upravitelja programa za otkrivanje ili usklađenost pretraživanja da biste potražili poruke. Da biste izbrisali poruke, morat ćete se pridružiti grupi uloga za upravljanje organizacijom ili ulogu pretraživanja i brisanja. Dozvole za ove uloge dodijeljene su u [centru za sigurnost i usklađenost](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Stvorite pretraživanje sadržaja](https://docs.microsoft.com/microsoft-365/compliance/content-search) da biste pronašli poruku koja će se izbrisati.
- [Spojite se na PowerShell centra za sigurnost i usklađenost](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Ako koristite višestruka provjera autentičnosti, pročitajte članak [Povezivanje s pomoću komponente Security i centar za usklađenost s microsoftovim 365 uz multi-Factor](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).