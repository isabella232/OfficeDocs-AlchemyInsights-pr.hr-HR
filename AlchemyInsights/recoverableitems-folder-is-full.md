---
title: 1336 RecoverableItems folder is full
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061748"
---
# <a name="the-recoverable-items-folder-is-full"></a>Mapa Stavke koje se mogu oporaviti puna je

Za Exchange Online poštanskih sandučića zadano je ograničenje prostora za pohranu za mapu Stavke koje se mogu oporaviti 30 GB. Ograničenje prostora za pohranu za mapu Stavke koje se mogu oporaviti automatski se povećava na 100 GB ako je poštanski sandučić postavljen na čuvanje u slučaju parničavanja, čuvanje predočavanja elektroničkih dokumenata ili je dodijeljen pravilniku o zadržavanju.

Kada mapa Stavke koje se mogu oporaviti dosegne ograničenje prostora za pohranu, funkcija poštanskog sandučića utječe na sljedeće načine:

- Korisnik ne može izbrisati stavke iz poštanskog sandučića.

- Pomoćnik za upravljane mape ne može brisati stavke na temelju oznaka zadržavanja ni postavki upravljane mape.

- Za poštanske sandučiće s omogućenim oporavkom pojedinačnih stavki ili su stavljeni na čekanje, postupak zaštite od kopiranja na pisanje ne može održavati verzije stavki koje je korisnik uredio.

- Za poštanske sandučiće s omogućenim zapisivanjem nadzora poštanskih sandučića nije moguće spremiti stavke zapisnika nadzora poštanskog sandučića u podmapu Nadzori u mapi Stavke koje se mogu oporaviti.

Za poštanske sandučiće koji nisu na čekanju administratori mogu koristiti naredbu u Exchange Online PowerShell za brisanje `Search-Mailbox -SearchDumpsterOnly -DeleteContent` stavki u mapi Stavke koje se mogu oporaviti. Dodatne informacije potražite u sljedećim temama:

- [Traženje i brisanje poruka](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Za poštanske sandučiće koji su na čekanju administratori moraju ukloniti čekanje da bi mogli izbrisati stavke iz mape Stavke koje se mogu oporaviti. Dodatne informacije potražite u članku Brisanje stavki u mapi Stavke koje se mogu [oporaviti poštanskih sandučića u oblaku na čekanju](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Da bi se spriječilo da mapa Stavke koje se mogu oporaviti postane puna, administratori mogu povećati ograničenje prostora za pohranu mape Stavke koje se mogu oporaviti za poštanske sandučiće na čekanju i postaviti pravilnik o zadržavanju poštanskog sandučića koji premješta stavke iz mape Stavke koje se mogu oporaviti u korisnikov arhivski poštanski sandučić. Pogledajte [povećavanje kvote za stavke koje se mogu oporaviti za poštanske sandučiće na čekanju](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
