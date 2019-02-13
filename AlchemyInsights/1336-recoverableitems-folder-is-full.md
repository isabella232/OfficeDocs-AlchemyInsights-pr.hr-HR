---
title: 1336 RecoverableItems mapa je puna
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: dbf4930c34e4175a14b77fab4eafc953bb37cc02
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29909280"
---
# <a name="the-recoverable-items-folder-is-full"></a>Mapu oporaviti stavke je pun

Za Exchange Online poštanskim sandučićima u sustavu Office 365, zadano ograničenje prostora za pohranu u mapu oporaviti stavke je 30 GB. Ograničenje spremišta za mapu oporaviti stavke automatski povećan je na 100 GB ako poštanski sandučić smjestiti na čekanju sudskih procesa, čekanje predočavanja elektroničkih dokumenata ili je dodijeljen pravilo zadržavanja za Office 365.
  
Kada mapu oporaviti stavke dosegne ograničenje prostora za pohranu, funkcionalnost poštanski sandučić je utjecati na sljedeće načine:
  
- Korisnik ne može izbrisati stavke iz poštanskog sandučića.
    
- Upravljani pomoćnika za mape nije moguće izbrisati stavaka na temelju postavke upravljanih mapa ili oznaka zadržavanja.
    
- Za poštanske sandučiće koji imaju omogućen oporavak jednu stavku ili stavljena na čekanje, zaštita proces kopiju na pisanje stranice nije moguće održavati verzije stavki uredio korisnika.
    
- Za poštanske sandučiće koji imaju poštanski sandučić nadzora omogućeno zapisivanje, stavke evidencije nadzora nema poštanski sandučić možete spremiti u revizije podmapu u mapi oporaviti stavke.
    
Za poštanske sandučiće koji nisu na čekanju, možete koristiti administratori na `Search-Mailbox -SearchDumpsterOnly -DeleteContent` naredbu u Exchange Online PowerShell izbrisati stavke u mapi oporaviti stavke. Dodatne informacije potražite u sljedećim temama: 
  
- [Traženje i brisanje poruka](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [Pretraživanje poštanskog sandučića](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
Za poštanske sandučiće koji su na čekanju, administratori imaju uklanjanje čekanja prije možete izbrisane stavke iz mape oporaviti stavke. Dodatne informacije potražite u [izbrisati stavke u oporaviti stavke mape poštanske sandučiće oblak temelji na čekanju](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).
  
Da biste spriječili mapu oporaviti stavke postaje pune, administratori možete povećati ograničenje prostora za pohranu oporaviti stavke mapu za poštanske sandučiće na čekanju i postavili pravila zadržavanja poštanski sandučić koje premješta stavke iz mape oporaviti stavke arhiva korisnika poštanski sandučić. Pogledajte [povećati oporaviti stavke kvote za poštanske sandučiće na čekanju](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
  

