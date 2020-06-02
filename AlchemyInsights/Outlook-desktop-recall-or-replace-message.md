---
title: Opoziv ili zamjena poruke e-pošte za Outlook za stolna računala
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: bb84363ae7d3c91750d5de789c091c7cebbbedc2
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502311"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Opoziv ili zamjena poruke e-pošte programa Outlook

- Kao administrator možete **opozvati poruke u ime korisnika pomoću powershell**. Ne možete se sjetiti poruka iz centra za administratore.
- Možete **se sjetiti samo poruka koje se šalju osobama u vašoj organizaciji**. Ako je poruka poslana na Gmail adresu, na primjer, ne možete je se sjetiti.
- Možete **se sjetiti samo poruka poslanih iz programa Outlook 2016 na PC- u**. Ako korisnik pošalje poruku pomoću programa Outlook za Mac ili Outlook na webu, ne možete je se sjetiti.

Da biste opozvali ili zamijenili poruku e-pošte:

1. U oknu mape s lijeve strane prozora programa Outlook odaberite mapu Poslane stavke.
1. Dvokliknite poruku koju želite opozvati da biste je otvorili.
1. Odaberite karticu **Poruka** , a zatim **Akcije**  >  **Opoziv ove poruke**.
1. Odaberite **Izbriši nepročitane kopije ove poruke** ili Izbriši **nepročitane kopije i zamijenite ga novom porukom**, a zatim odaberite U **redu**.
1. Ako šaljete zamjensku poruku, sastavite poruku, a zatim odaberite **Pošalji**.
1. Uspjeh ili neuspjeh opoziva poruke ovisi o postavkama primatelja u programu Outlook. Upute za provjeru opoziva potražite u [ovom članku](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Traženje i brisanje poruka e-pošte u tvrtki ili ustanovi

- Ako niste globalni administrator, vaš račun mora biti dodan ulozi upravitelja predočavanja elektroničkih dokumenata ili ulozi upravljanja pretraživanjem usklađenosti da biste potražili poruke. Da biste izbrisali poruke, morat ćete se pridružiti grupi uloga upravljanje organizacijom ili ulozi upravljanja pretraživanjem i čišćenjem. Dozvole za te uloge dodijeljene su u [centru za sigurnost i usklađenost](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Stvorite pretraživanje sadržaja](https://docs.microsoft.com/microsoft-365/compliance/content-search) da biste pronašli poruku koju želite izbrisati.
- [Povezivanje sa sigurnosnom jezgrom i powershell centrom za usklađenost](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Ako koristite višestruku provjeru autentičnosti, pročitajte mogućnost [Povezivanje sa sigurnošću sustava Microsoft 365 i PowerShell centar za usklađenost pomoću višestruke provjere autentičnosti](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).