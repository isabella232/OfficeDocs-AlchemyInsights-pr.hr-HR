---
title: Opozvati ili zamijeniti poruku e-pošte
ms.author: daeite
author: daeite
manager: joallard
ms.date: 05/15/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: d5952041f6f2fd736e975abf06cc22880d21a089
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36553424"
---
# <a name="recall-or-replace-an-email-message-in-office-365"></a>Opozvati ili zamijeniti poruku e-pošte u sustavu Office 365

- Možete **samo opoziv poruke koje se šalju osobe u vašoj organizaciji**. Ako je poruka poslana na adresu Gmail, na primjer, ne možete opozvati ga.
- Možete **samo opoziv poruke poslane iz Outlook 2016 za osobnog računala**. Ako korisnik pošalje poruku koristeći Outlook za Mac ili Outlook na webu, ne može se opozvati.
- Ako ste na administraciju, možete **opoziv poruke u ime korisnika pomoću PowerShell**. Nije moguće opozvati poruke iz centra za administraciju. Pomaknite se do "Traženje i brisanje poruka e-pošte u vašoj organizaciji" Dodatne informacije.

**Opozvati ili zamijeniti poruku e-pošte koje ste poslali**

1. U oknu mape na lijevoj strani prozora programa Outlook, odaberite mapu poslane stavke.
2. Otvorite poruku koju želite opozvati. Dvokliknite morate otvoriti poruku. Ako odaberete poruku tako da se pojavljuje u oknu za čitanje neće dopustiti opozvati poruku.
3. Na kartici poruka, odaberite **Akcije** > **Opoziv ove poruke**.
4. Odaberite **izbrisati nepročitane kopije ove poruke** ili **izbrisati nepročitane kopije i zamijeniti novu poruku**, a zatim **u redu**.
5. Ako šaljete poruku zamjenski sastavite poruku, a zatim odaberite **Pošalji**.
6. Uspjeh ili Neuspjeh opoziva poruke ovisi o postavkama primatelja u programu Outlook.

Za više informacija, uključujući kako provjeriti opoziv, pogledajte [Opoziv ili zamjena poruke e-pošte koju ste poslali](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Traženje i brisanje poruka e-pošte u vašoj organizaciji*** Za traženje i brisanje poruka e-pošte u vašoj organizaciji, najlakše ga je ako ste globalne administratora. Ako niste globalni administrator, vaš račun mora dodati grupe uloga Upravitelj predočavanja elektroničkih dokumenata ili uloge Upravljanje usklađenosti pretraživanja. Za brisanje poruka, trebat ćete pridružiti grupe uloga upravljanja organizacije ili upravljanje uloga pretraživanja i Pročisti. U [centru za sigurnost & usklađenosti](https://protection.office.com/)dodjeljuju se dozvole te uloge.

1. [Stvaranje sadržaja pretraživanja](https://docs.microsoft.com/office365/securitycompliance/content-search) da biste pronašli poruku za brisanje.
2. [Povezivanje s PowerShell usklađenosti centar sigurnosti &](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Ako koristite MFA, pogledajte [Povezivanje Office 365 sigurnosne & PowerShell centar usklađenosti korištenjem višestruku provjeru autentičnosti](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
