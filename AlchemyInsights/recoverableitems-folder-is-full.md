---
title: mapa funkcija RecoverableItems 1336 je puna
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
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741259"
---
# <a name="the-recoverable-items-folder-is-full"></a>Mapa s stavkama koje je moguće vratiti je puna

Za poštanske sandučiće sustava Exchange Online zadano ograničenje prostora za pohranu za mapu s stavkama koje se mogu oporaviti iznosi 30 GB. Ograničenje prostora za pohranu za mapu stavke koje se mogu vratiti automatski se povećava na 100 GB ako se poštanski sandučić smješta na zadržavanje sudskog postupka, traženje otkrivanja ili je dodijeljeno pravilima zadržavanja.

Kada mapa Oporavljene stavke dosegne ograničenje prostora za pohranu, funkcionalnost poštanskog sandučića utječe na sljedeće načine:

- Korisnik ne može izbrisati stavke iz poštanskog sandučića.

- Pomoćnik za upravljane mape ne može izbrisati stavke na temelju postavke oznake zadržavanja ili upravljane mape.

- Za poštanske sandučiće koji imaju omogućen jedan oporavak stavke ili su stavljeni na čekanje, postupak zaštite stranice za kopiranje na pisanje ne može održavati verzije stavki koje je korisnik uredio.

- Za poštanske sandučiće koje imaju omogućeno zapisivanje nadzornog sandučića, ne mogu se spremiti stavke zapisnika nadzora poštanskih sandučića u podmapi revizija u mapi stavke koje se mogu oporaviti.

Za poštanske sandučiće koji nisu na čekanju administratori mogu koristiti `Search-Mailbox -SearchDumpsterOnly -DeleteContent` naredbu u komponenti Exchange Online PowerShell za brisanje stavki u mapi stavke koje se mogu oporaviti. Dodatne informacije potražite u sljedećim temama:

- [Traženje i brisanje poruka](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Pretraživanje – poštanski sandučić](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Za poštanske sandučiće koji se nalaze na čekanju administratori moraju ukloniti čekanje da bi izbrisali stavke iz mape s stavkama koje se mogu oporaviti. Dodatne informacije potražite u članku [Brisanje stavki u mapi stavke koje se mogu oporaviti u cloud-bazirane poštanske sandučiće na čekanju](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Da biste spriječili potpunu mapu s stavkama koje se mogu oporaviti, administratori mogu povećati ograničenje prostora za pohranu u mapi stavke koje se mogu vratiti za poštanske sandučiće na čekanju i postaviti pravilnik o zadržavanju poštanskog sandučića koji premješta stavke iz mape stavke koje se mogu vratiti u korisnikov arhivski poštanski sandučić. Pročitajte članak [povećanje kvote stavki koje se mogu oporaviti za poštanske sandučiće na čekanju](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
