---
title: Opoziv ili zamjena poruke e-pošte radne površine programa Outlook Desktop
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: d64332778f9132aff6a9660bb0d522f4e16b753c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687502"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Opoziv ili zamjena poruke e-pošte programa Outlook

- Kao admin, možete **opozvati poruke u ime korisnika pomoću PowerShell**. Ne možete opozvati poruke iz centra za administratore.
- Možete **se prisjetiti samo poruka koje se šalju osobama u vašoj organizaciji**. Ako je poruka poslana na Gmail adresu, na primjer, ne možete je se sjetiti.
- Možete **samo opozvati poruke poslane iz programa Outlook 2016 na PC-ju**. Ako korisnik pošalje poruku pomoću programa Outlook za Mac ili Outlook na webu, ne možete je se sjetiti.

Da biste opozvali ili zamijenili poruku e-pošte:

1. U oknu mape s lijeve strane prozora programa Outlook odaberite mapu Poslane stavke.
1. Dvokliknite poruku koju želite opozvati da biste je otvorili.
1. Odaberite karticu **Poruka,** a zatim **Akcije Opoziv** > **ova poruka**.
1. Odaberite **Izbriši nepročitane kopije ove poruke** ili Izbriši **nepročitane kopije i zamijeni je novom porukom**, a zatim odaberite U **redu**.
1. Ako šaljete zamjensku poruku, sastavite poruku, a zatim odaberite **Pošalji**.
1. Uspjeh ili neuspjeh opoziva poruke ovisi o postavkama primatelja u programu Outlook. Korake za provjeru opoziva potražite u [ovom članku](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Traženje i brisanje poruka e-pošte u tvrtki ili ustanovi

- Ako niste globalni administrator, vaš se račun mora dodati ulozi upravitelja predočavanja elektroničkih dokumenata ili ulozi upravljanja pretraživanjem usklađenosti da biste potražili poruke. Da biste izbrisali poruke, morat ćete se pridružiti grupi uloga Upravljanje organizacijom ili ulozi upravljanja pretraživanjem i čišćenjem. Dozvole za te uloge dodjeljuju se u centru za [sigurnost i usklađenost](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Stvorite pretraživanje sadržaja](https://docs.microsoft.com/office365/securitycompliance/content-search) da biste pronašli poruku koju želite izbrisati.
- [Povežite se s powershellcentra za sigurnost i usklađenost](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Ako koristite višestruku provjeru autentičnosti, [pročitajte u članku Povezivanje sa ljuskom Microsoft 365 za sigurnost i centar za usklađenost PowerShell pomoću višestruke provjere autentičnosti](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).