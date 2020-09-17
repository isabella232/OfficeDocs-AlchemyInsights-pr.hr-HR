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
ms.openlocfilehash: 2e711679e7db7293d9e7e6f68d0662f03047c23d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799196"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Opoziv ili zamjena poruke e-pošte u programu Microsoft 365

- Možete se **prisjetiti samo poruka koje se šalju osobama u vašoj tvrtki ili ustanovi**. Ako je poruka poslana na adresu servisa Gmail, na primjer, ne možete je opozvati.
- Možete se **prisjetiti samo poruka poslane iz programa Outlook 2016 za PC**. Ako korisnik pošalje poruku pomoću programa Outlook za Mac ili Outlook na webu, ne možete je opozvati.
- Ako ste administrator, možete **opozvati poruke u ime korisnika pomoću komponente PowerShell**. Ne možete se prisjetiti poruka iz centra za administratore. Pomaknite se prema dolje do "traženje i brisanje poruka e-pošte u tvrtki ili ustanovi" da biste saznali više.

**Opoziv ili zamjena poruke e-pošte koju ste poslali**

1. U oknu s mapama na lijevoj strani prozora programa Outlook odaberite mapu poslane stavke.
2. Otvorite poruku koju želite opozvati. Da biste otvorili poruku, morate je dvaput kliknuti. Odabir poruke tako da se prikazuje u oknu za čitanje neće vam dopustiti opoziv poruke.
3. Na kartici poruka odaberite **Akcije**  >  **Opoziv ove poruke**.
4. Odaberite **Izbriši nepročitane kopije ove poruke** ili **Izbriši nepročitane kopije i zamijeni novom porukom**, a zatim odaberite **u redu**.
5. Ako šaljete zamjensku poruku, sastavite poruku, a zatim odaberite **Send (Šalji**).
6. Uspjeh ili neuspjeh opoziv poruke ovisi o postavkama primatelja u programu Outlook.

Dodatne informacije, uključujući kako provjeriti opoziv, potražite u članku [opoziv ili zamjena poruke e-pošte koju ste poslali](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Traženje i brisanje poruka e-pošte u tvrtki ili ustanovi*** Da biste potražili i izbrisali poruke e-pošte u tvrtki ili ustanovi, najlakše je ako ste globalni administrator. Ako niste globalni administrator, vaš račun mora biti dodan u grupu uloga upravitelja programa eDiscovery ili na ulogu upravljanja usklađivanjem pretraživanja. Da biste izbrisali poruke, morat ćete se pridružiti grupi uloga za upravljanje organizacijom ili ulogu pretraživanja i brisanja. Dozvole za te uloge dodijeljene su u [centru za sigurnost & usklađenosti](https://protection.office.com/).

1. [Stvorite pretraživanje sadržaja](https://docs.microsoft.com/microsoft-365/compliance/content-search) da biste pronašli poruku koja će se izbrisati.
2. [Spojite se na sigurnosnu & PowerShell centra za usklađenost](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Ako koristite MFA, pročitajte članak [Povezivanje sa sigurnošću & u programu Microsoft 365 za usklađenost s pomoću multi-Factor provjere autentičnosti](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
