---
title: Outlook radne površine opoziv ili zamjena poruke e-pošte
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: aced684777ef82860b969aea8825699b78b04c5a
ms.sourcegitcommit: aad9f863bc9fd7d5522c480bd1a7d15f3a80ff4f
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/15/2019
ms.locfileid: "30657036"
---
# <a name="recall-or-replace-an-email-message"></a>Opozvati ili zamijeniti poruku e-pošte

- Kao administrator, možete **opoziv poruke u ime korisnika pomoću PowerShell**. Nije moguće opozvati poruke iz centra za administraciju.
- Možete **samo opoziv poruke koje se šalju osobe u vašoj organizaciji**. Ako je poruka poslana na adresu Gmail, na primjer, ne možete opozvati ga.
- Možete **samo opoziv poruke poslane iz Outlook 2016 na Računalu**. Ako korisnik pošalje poruku koristeći Outlook za Mac ili Outlook na webu, ne može se opozvati.

Kako opozvati ili zamijeniti poruku e-pošte:

1. U oknu mape na lijevoj strani prozora programa Outlook, odaberite mapu poslane stavke.
1. Dvokliknite poruku koju želite opozvati da biste ga otvorili.
1. Odaberite karticu **poruku** , a zatim odaberite **Akcije** > **Opoziv ove poruke**.
1. Odaberite **izbrisati nepročitane kopije ove poruke** ili **izbrisati nepročitane kopije i zamijeniti novu poruku**, a zatim odaberite **u redu**.
1. Ako šaljete poruku zamjenski sastavite poruku, a zatim odaberite **Pošalji**.
1. Uspjeh ili Neuspjeh opoziva poruke ovisi o postavkama primatelja u programu Outlook. Korake provjeriti opoziv potražite u [ovom članku](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Traženje i brisanje poruka e-pošte u vašoj organizaciji

- Ako niste globalni administrator, vaš račun mora dodati predočavanja elektroničkih dokumenata Upravitelj ulogu ili uloge Upravljanje usklađenosti pretraživanja za traženje poruke. Za brisanje poruka, trebat ćete pridružiti grupe uloga upravljanja organizacije ili upravljanje uloga pretraživanja i Pročisti. Dozvole za ove uloge dodjeljuju se u [centru sigurnosti i usklađenosti](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Stvaranje sadržaja pretraživanja](https://docs.microsoft.com/office365/securitycompliance/content-search) da biste pronašli poruku za brisanje.
- [Povezivanje s sigurnost i usklađenosti centar PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Ako koristite višestruku provjeru autentičnosti, pogledajte [povezivanje za Office 365 sigurnost i usklađenosti centar PowerShell korištenjem višestruku provjeru autentičnosti](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).