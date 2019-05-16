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
ms.custom: 1860
ms.assetid: ''
ms.openlocfilehash: 6e66b5d60fe9ac66c2f2f8f7e99e753652c3a59e
ms.sourcegitcommit: bcb2612ab8ba2aee5165e3912dca95cc1bdd09f4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/16/2019
ms.locfileid: "34096446"
---
# <a name="recall-or-replace-an-email-message"></a>Opozvati ili zamijeniti poruku e-pošte

- Možete **samo opoziv poruke koje se šalju osobe u vašoj organizaciji**. Ako je poruka poslana na adresu Gmail, na primjer, ne možete opozvati ga.
- Možete **samo opoziv poruke poslane iz Outlook 2016 za osobnog računala**. Ako korisnik pošalje poruku koristeći Outlook za Mac ili Outlook na webu, ne može se opozvati.
- Ako ste na administraciju, možete **opoziv poruke u ime korisnika pomoću PowerShell**. Nije moguće opozvati poruke iz centra za administraciju. Pomaknite se do "Traženje i brisanje poruka e-pošte u vašoj organizaciji" Dodatne informacije.

***Opozvati ili zamijeniti poruku e-pošte koje ste poslali***
1. U oknu mape na lijevoj strani prozora programa Outlook, odaberite mapu poslane stavke.
2. Otvorite poruku koju želite opozvati. Dvokliknite morate otvoriti poruku. Ako odaberete poruku tako da se pojavljuje u oknu za čitanje neće dopustiti opozvati poruku.
3. Na kartici poruka, odaberite **Akcije** > **Opoziv ove poruke**.
4. Odaberite **izbrisati nepročitane kopije ove poruke** ili **izbrisati nepročitane kopije i zamijeniti novu poruku**, a zatim **u redu**.
5. Ako šaljete poruku zamjenski sastavite poruku, a zatim odaberite **Pošalji**.
6. Uspjeh ili Neuspjeh opoziva poruke ovisi o postavkama primatelja u programu Outlook. 

Za više informacija, uključujući kako provjeriti opoziv, pogledajte [Opoziv ili zamjena poruke e-pošte koju ste poslali](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Traženje i brisanje poruka e-pošte u vašoj organizaciji*** Za traženje i brisanje poruka e-pošte u vašoj organizaciji, najlakše ga je ako ste globalne administratora. Ako niste globalni administrator, vaš račun mora dodati grupe uloga Upravitelj predočavanja elektroničkih dokumenata ili uloge Upravljanje usklađenosti pretraživanja. Za brisanje poruka, trebat ćete pridružiti grupe uloga upravljanja organizacije ili upravljanje uloga pretraživanja i Pročisti. U [centru za sigurnost & usklađenosti](https://protection.office.com/)dodjeljuju se dozvole te uloge.

1. [Stvaranje sadržaja pretraživanja](https://docs.microsoft.com/en-us/office365/securitycompliance/content-search) da biste pronašli poruku za brisanje.
2. [Povezivanje s PowerShell usklađenosti centar sigurnosti &](https://docs.microsoft.com/en-us/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Ako koristite MFA, pogledajte [Povezivanje Office 365 sigurnosne & PowerShell centar usklađenosti korištenjem višestruku provjeru autentičnosti](https://docs.microsoft.com/en-us/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 