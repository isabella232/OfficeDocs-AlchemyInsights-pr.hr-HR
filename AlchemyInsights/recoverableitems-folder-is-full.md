---
title: 1336 Mapa RecoverableItems je puna
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720244"
---
# <a name="the-recoverable-items-folder-is-full"></a>Mapa Oporavljene stavke puna je

Za poštanske sandučiće sustava Exchange Online zadano ograničenje pohrane za mapu Oporavljene stavke je 30 GB. Ograničenje prostora za pohranu za mapu Oporavljene stavke automatski se povećava na 100 GB ako je poštanski sandučić smješten na čuvanje parnice, čuvanje elektroničkih dokumenata ili je dodijeljeno pravilima zadržavanja.

Kada mapa Oporavljene stavke dosegne ograničenje pohrane, funkcija poštanskog sandučića utječe na sljedeće načine:

- Korisnik ne može izbrisati stavke iz poštanskog sandučića.

- Pomoćnik za upravljane mape ne može izbrisati stavke na temelju oznake zadržavanja ili postavki upravljanih mapa.

- Za poštanske sandučiće kojima je omogućen oporavak jedne stavke ili su stavljeni na čekanje, postupak zaštite stranice za kopiranje na pisati ne može održavati verzije stavki koje je korisnik uredio.

- Za poštanske sandučiće kojima je omogućeno zapisivanje nadzora poštanskog sandučića, stavke zapisnika nadzora poštanskog sandučića ne mogu se spremiti u podmapu Nadzori u mapi Stavke koje se mogu oporaviti.

Za poštanske sandučiće koji nisu na čekanju `Search-Mailbox -SearchDumpsterOnly -DeleteContent` administratori mogu koristiti naredbu u komponente Exchange Online PowerShell za brisanje stavki u mapi Stavke koje se mogu oporaviti. Dodatne informacije potražite u sljedećim temama:

- [Traženje i brisanje poruka](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [Pretraživanje poštanskog sandučića](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Za poštanske sandučiće koji su na čekanju administratori moraju ukloniti čekanje da bi mogli izbrisati stavke iz mape Stavke koje se mogu oporaviti. Dodatne informacije [potražite u odjeljku Brisanje stavki u mapi Stavke koje se mogu oporaviti u oblaku na čekanju](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Da bi spriječili da mapa Oporavive stavke postane puna, administratori mogu povećati ograničenje pohrane mape Oporavljene stavke za poštanske sandučiće na čekanju i postaviti pravila zadržavanja poštanskog sandučića koja premješta stavke iz mape Stavke koje se mogu oporaviti u poštanski sandučić arhive korisnika. Pogledajte [Povećanje kvote Oporavljenih stavki za poštanske sandučiće na čekanju](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
