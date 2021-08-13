---
title: Outlook Opoziv radne površine ili zamjena poruke e-pošte
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
ms.openlocfilehash: 33fe7ebd53d7ff11dbab54ce589aaf58e68c633be4d83a3cdfb00edc7752430e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918387"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Opoziv ili zamjena poruke Outlook e-pošte

- Kao administrator možete **opozvati poruke u ime korisnika pomoću komponente PowerShell.** Ne možete opozvati poruke iz centra za administratore.
- Možete **opozvati samo poruke koje se šalju osobama u tvrtki ili ustanovi**. Ako je, primjerice, poruka poslana na Gmail adresu, ne možete je se sjetiti.
- Možete **opozvati samo poruke poslane s Outlook 2016 na PC-ju**. Ako korisnik pošalje poruku pomoću Outlook za Mac ili Outlook na webu, ne možete je se sjetiti.

Da biste opozvati ili zamijeniti poruku e-pošte:

1. U oknu s mapama s lijeve strane Outlook odaberite mapu Poslane stavke.
1. Dvokliknite poruku koju želite opozvati da biste je otvorili.
1. Odaberite **karticu Poruka,** a zatim Odaberite **Akcije**  >  **Opozovi ovu poruku**.
1. Odaberite **Izbriši nepročitane kopije ove poruke** ili Izbriši **nepročitane** kopije i zamijenite je novom porukom , a zatim odaberite U **redu**.
1. Ako šaljete zamjensku poruku, sastavite poruku, a zatim odaberite **Pošalji**.
1. Uspjeh ili neuspjeh opoziva poruke ovisi o postavkama primatelja u programu Outlook. Upute za provjeru opoziva potražite u [ovom članku.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

Traženje i brisanje poruka e-pošte u tvrtki ili ustanovi

- Ako niste globalni administrator, račun morate dodati u ulogu upravitelja predočavanja elektroničkih elektroničkih obveza ili ulogu upravljanja pretraživanjem usklađenosti da biste potražili poruke. Da biste izbrisali poruke, morate se pridružiti grupi uloga za upravljanje organizacijom ili ulozi upravljanja pretraživanjem i čišćenjem. Dozvole za te uloge dodjeljuju se u centru [za sigurnost i usklađenost](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Stvorite pretraživanje sadržaja da](https://docs.microsoft.com/microsoft-365/compliance/content-search) biste pronašli poruku koju želite izbrisati.
- [Povezivanje centru za sigurnost i usklađenost PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Ako koristite višestruku provjeru autentičnosti, pogledajte Povezivanje biste Microsoft 365 sigurnosti i usklađenosti [PowerShell pomoću višestruke provjere autentičnosti](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).