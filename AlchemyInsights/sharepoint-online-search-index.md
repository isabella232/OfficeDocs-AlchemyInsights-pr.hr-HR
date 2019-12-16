---
title: Pretraživanje u sustavu SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044035"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a>Pretraživanje i indeksiranje sadržaja u sustavu SharePoint Online

Sadržaj mora biti pretražen radi indeksiranja i dodan u indeks pretraživanja da bi korisnici pronašli ono što pretražuju u sustavu SharePoint online. Sadržaj se automatski pretražuje na temelju unaprijed definiranih rasporeda pretraživanja radi indeksiranja (raspored pretraživanja radi indeksiranja ne može se promijeniti). Alat za indeksiranje preuzima sadržaj koji se promijenio od zadnjeg pretraživanja radi indeksiranja sadržaja i obnavlja indeks. Da biste osigurali da je sadržaj pretraživan i da je indeks ažuriran, napominjemo sljedeće:

- Provjerite je li sadržaj moguće pronaći tako da se [sadržaj web-mjesta može pretraživati](https://docs.microsoft.com/sharepoint/make-site-content-searchable).

- Kada ste promijenili upravljano svojstvo ili kada ste promijenili mapiranje pretraživanja i upravljanih svojstava, web-mjesto se mora ponovno pretraživati radi indeksiranja prije nego što se promjene odražavaju u indeksu pretraživanja. 

    Budući da su vaše promjene napravljene u shemi pretraživanja, a ne na stvarnom web-mjestu, pretraživač neće automatski ponovno indeksirati web-mjesto. 

    Za više informacija pogledajte [ručno zatražite pretraživanje i ponovno indeksiranje web-mjesta, biblioteke ili popisa](https://docs.microsoft.com/sharepoint/crawl-site-conten).

- Pričekajte najmanje 24 sata nakon ručnog traženja pretraživanja radi indeksiranja i potpunog ponovnog indeksa da biste vidjeli imate li još uvijek problem. 

    Ako je prošlo više od 24 sata od kada ste pokrenuli pretraživanje radi indeksiranja i potpuno ponovno indeksiranje, prijavite slučaj podrške. U mnogim slučajevima već radimo na rješenju. Molim vas, dajte nam najmanje 24 sata da dovršimo rješenje.

> [!IMPORTANT]
> Ako je web-mjesto, dokument (biblioteka) ili popis izbrisan i još se prikazuje u rezultatima pretraživanja, korisnici bi trebali primiti **pogrešku 404 datoteka nije pronađena** prilikom pokušaja pristupa. Taj bi problem trebao biti prijavljen kao slučaj podrške za daljnju istragu. 



