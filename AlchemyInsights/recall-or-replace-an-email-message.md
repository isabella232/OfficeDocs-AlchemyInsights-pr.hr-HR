---
title: Opoziv ili zamjena poruke e-pošte
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 45882b49c5c47b3e0e4519e2339e6c68110bc75aebeaeac2d0ccd009bdfa3f7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024378"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Opoziv ili zamjena poruke e-pošte u programu Microsoft 365

- Možete **opozvati samo poruke koje se šalju osobama u tvrtki ili ustanovi**. Ako je, primjerice, poruka poslana na Gmail adresu, ne možete je se sjetiti.
- Možete **opozvati samo poruke poslane Outlook za PC**. Ako korisnik pošalje poruku pomoću Outlook za Mac ili Outlook na webu, ne možete je se sjetiti.
- Kao administrator klijenta možete opozvati poruke u ime korisnika pomoću komponente **PowerShell** (Dodatne informacije potražite u članku Traženje i brisanje poruka [e-pošte).](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)
- Ne možete opozvati poruke iz centra za administratore. Pomaknite se prema dolje do "Traženje i brisanje poruka e-pošte u tvrtki ili ustanovi" da biste saznali više.

**Opoziv ili zamjena poruke e-pošte koju ste poslali**

1. U oknu s mapama s lijeve strane Outlook odaberite mapu Poslane stavke.
2. Otvorite poruku koju želite opozvati. Da biste otvorili poruku, morate dvoklikom otvoriti poruku. Odabir poruke tako da se prikazuje u oknu za čitanje neće vam omogućiti opoziv poruke.
3. Na kartici Poruka odaberite **Akcije**  >  **Opozovi ovu poruku**.
4. Odaberite **Izbriši nepročitane kopije ove poruke** ili Izbriši **nepročitane** kopije i zamijenite je novom porukom , a zatim odaberite U **redu**.
5. Ako šaljete zamjensku poruku, sastavite poruku, a zatim odaberite **Pošalji**.
6. Uspjeh ili neuspjeh opoziva poruke ovisi o postavkama primatelja u Outlook.

Dodatne informacije, uključujući upute za provjeru opoziva potražite u članku Opoziv ili zamjena poslane poruke [e-pošte.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

***Da biste potražili i izbrisali poruke*** e-pošte u tvrtki ili ustanovi, najjednostavnije je ako ste globalni administrator. Ako niste globalni administrator, račun morate dodati u grupu uloga upravitelja elektroničkih elektroničkih obveza ili u ulogu upravljanja pretraživanjem usklađenosti. Da biste izbrisali poruke, morate se pridružiti grupi uloga za upravljanje organizacijom ili ulozi upravljanja pretraživanjem i čišćenjem. Dozvole za te uloge dodjeljuju se u centru [za & usklađenosti](https://protection.office.com/).

1. [Stvorite pretraživanje sadržaja da](https://docs.microsoft.com/microsoft-365/compliance/content-search) biste pronašli poruku koju želite izbrisati.
2. [Povezivanje na powershell centra za & sigurnosti](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Ako koristite MFA (višestruku provjeru autentičnosti), pogledajte Povezivanje za Microsoft 365 sigurnost & PowerShell pomoću [višestruke provjere autentičnosti](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).
