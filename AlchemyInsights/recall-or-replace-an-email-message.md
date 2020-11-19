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
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353498"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Opoziv ili zamjena poruke e-pošte u programu Microsoft 365

- Možete se **prisjetiti samo poruka koje se šalju osobama u vašoj tvrtki ili ustanovi**. Ako je, primjerice, poruka poslana na adresu servisa Gmail, ne možete je opozvati.
- Možete se **prisjetiti samo poruka poslane iz programa Outlook za PC**. Ako korisnik pošalje poruku pomoću programa Outlook za Mac ili Outlook na webu, ne možete je opozvati.
- Kao administrator administratora možete **opozvati poruke u ime korisnika pomoću komponente PowerShell** (Dodatne informacije potražite u člancima: [Traženje i brisanje poruka e-pošte](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).
- Ne možete se prisjetiti poruka iz centra za administratore. Pomaknite se prema dolje do "traženje i brisanje poruka e-pošte u tvrtki ili ustanovi" da biste saznali više.

**Opoziv ili zamjena poruke e-pošte koju ste poslali**

1. U oknu s mapama na lijevoj strani prozora programa Outlook odaberite mapu poslane stavke.
2. Otvorite poruku koju želite opozvati. Da biste otvorili poruku, morate je dvaput kliknuti. Odabir poruke tako da se prikazuje u oknu za čitanje neće vam dopustiti opoziv poruke.
3. Na kartici poruka odaberite **Akcije**  >  **Opoziv ove poruke**.
4. Odaberite **Izbriši nepročitane kopije ove poruke** ili **Izbriši nepročitane kopije i zamijeni novom porukom**, a zatim odaberite **u redu**.
5. Ako šaljete zamjensku poruku, sastavite poruku, a zatim odaberite **Send (Šalji**).
6. Uspjeh ili neuspjeh opoziv poruke ovisi o postavkama primatelja u programu Outlook.

Dodatne informacije, uključujući kako provjeriti opoziv, potražite u članku [opoziv ili zamjena poruke e-pošte koju ste poslali](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

**_Da biste potražili i izbrisali poruke e-pošte u tvrtki ili ustanovi_**, najlakše je ako ste globalni administrator. Ako niste globalni administrator, vaš račun mora biti dodan u grupu uloga upravitelja programa eDiscovery ili na ulogu upravljanja usklađivanjem pretraživanja. Da biste izbrisali poruke, morat ćete se pridružiti grupi uloga za upravljanje organizacijom ili ulogu pretraživanja i brisanja. Dozvole za te uloge dodijeljene su u [centru za sigurnost & usklađenosti](https://protection.office.com/).

1. [Stvorite pretraživanje sadržaja](https://docs.microsoft.com/microsoft-365/compliance/content-search) da biste pronašli poruku koja će se izbrisati.
2. [Spojite se na sigurnosnu & PowerShell centra za usklađenost](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Ako koristite MFA (višestruka provjera autentičnosti), pročitajte članak [Povezivanje sa zaštitom programa Microsoft 365 za sigurnost & PowerShell centra za usklađenost pomoću višečimbenika provjere autentičnosti](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).
