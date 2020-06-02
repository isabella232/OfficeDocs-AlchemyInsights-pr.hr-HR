---
title: Opoziv ili zamjena poruke e-pošte
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: e958dab159e4dcc11f9c068bded3aa06ccd65c15
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509448"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Opoziv ili zamjena poruke e-pošte u sustavu Microsoft 365

- Možete **se sjetiti samo poruka koje se šalju osobama u vašoj organizaciji**. Ako je poruka poslana na Gmail adresu, na primjer, ne možete je se sjetiti.
- Možete **se sjetiti samo poruka poslanih iz programa Outlook 2016 za PC**. Ako korisnik pošalje poruku pomoću programa Outlook za Mac ili Outlook na webu, ne možete je se sjetiti.
- Ako ste administrator, poruke **možete opozvati u ime korisnika pomoću komponente PowerShell**. Ne možete se sjetiti poruka iz centra za administratore. Dodatne informacije pomaknite se prema dolje do odjeljka "Traženje i brisanje poruka e-pošte u tvrtki ili ustanovi".

**Opoziv ili zamjena poslane poruke e-pošte**

1. U oknu mape s lijeve strane prozora programa Outlook odaberite mapu Poslane stavke.
2. Otvorite poruku koju želite opozvati. Da biste otvorili poruku, morate dvokliknuti. Odabirom poruke tako da se pojavi u oknu za čitanje neće vam omogućiti da se prisjetite poruke.
3. Na kartici Poruka odaberite **Akcije**  >  **Opoziv ove poruke**.
4. Odaberite **Izbriši nepročitane kopije ove poruke** ili Izbriši **nepročitane kopije i zamijenite ga novom porukom**, a zatim odaberite U **redu**.
5. Ako šaljete zamjensku poruku, sastavite poruku, a zatim odaberite **Pošalji**.
6. Uspjeh ili neuspjeh opoziva poruke ovisi o postavkama primatelja u programu Outlook.

Dodatne informacije, uključujući kako provjeriti opoziv, potražite u [odjeljku Opoziv ili zamjena poruke e-pošte koju ste poslali](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Traženje i brisanje poruka e-pošte u tvrtki ili ustanovi*** Da biste potražili i izbrisali poruke e-pošte u tvrtki ili ustanovi, najjednostavnije je ako ste globalni administrator. Ako niste globalni administrator, vaš račun mora biti dodan u grupu uloga upravitelja predočavanja elektroničkih dokumenata ili u ulogu upravljanja pretraživanjem usklađenosti. Da biste izbrisali poruke, morat ćete se pridružiti grupi uloga upravljanje organizacijom ili ulozi upravljanja pretraživanjem i čišćenjem. Dozvole za te uloge dodjeljuju se u centru za [usklađenost & sigurnosti](https://protection.office.com/).

1. [Stvorite pretraživanje sadržaja](https://docs.microsoft.com/microsoft-365/compliance/content-search) da biste pronašli poruku koju želite izbrisati.
2. [Povezivanje sa sigurnosnom & PowerShell centra za usklađenost](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Ako koristite MFA, [pročitajte mogućnost Povezivanje sa sustavom Microsoft 365 security & PowerShell centar za usklađenost pomoću višestruke provjere autentičnosti](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
