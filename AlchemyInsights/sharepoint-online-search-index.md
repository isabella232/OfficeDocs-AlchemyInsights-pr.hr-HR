---
title: Pretraživanje u programu SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 3c3f6384172b2b4d59db6059618572db11059228
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507623"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a>Sadržaja pretraživanja i indeksiranja u SharePoint Online

Sadržaj mora pretražiti radi indeksiranja i dodati indeks pretraživanja za korisnike da biste pronašli što oni tražite u SharePoint Online. Sadržaj automatski pretražuje na temelju rasporedu unaprijed definiranih pretraživanja radi indeksiranja (rasporeda pretraživanja radi indeksiranja sadržaja ne može se mijenjati). Pretraživač uzima sadržaj koji je promijenjen od posljednjeg pretraživanja i ažurira indeks. Da biste osigurali radi indeksiranja sadržaja i ažuriranje indeksa, imajte na umu sljedeće:

- Provjerite sadržaj možete pronaći izradom [pretraživati sadržaj web-mjesta](https://docs.microsoft.com/sharepoint/make-site-content-searchable).

- Kada ste promijenili upravljano svojstvo ili kada ste promijenili mapiranje pretražena radi indeksiranja i upravljanih svojstava, web-mjesta mora biti ponovno pretražena radi indeksiranja sadržaja prije promjene odrazit će se u indeksu pretraživanja. 

    Jer vaše se promjene u shemi pretraživanja i indeksiranja će da ne stvarnog web-mjesta neće automatski ponovno indeksirati web-mjesta. 

    Za dodatne informacije pogledajte [ručno zahtjev za pretraživanje radi indeksiranja i ponovno indeksiranje web-mjesta u biblioteku ili popis](https://docs.microsoft.com/sharepoint/crawl-site-conten).

- Pričekajte barem 24 sata nakon ručno zahtijevanje pretraživanja radi indeksiranja sadržaja i puni ponovno indeksirati da biste vidjeli Ako još uvijek imate problema. 

    Ako više od 24 sata prošlo otkad je inicirao pretraživanja radi indeksiranja sadržaja i puni ponovno indeksirati, prijaviti podršku slučaj. U mnogim slučajevima smo već radite rješenje. Molimo pošaljite nam najmanje 24 sata dovršiti rješenje.

> [!IMPORTANT]
> Ako web-mjesto dokumenta (biblioteka) ili popis je izbrisan i još uvijek prikazuje u rezultatima pretraživanja, korisnici trebaju primati pojavila **Pogreška 404 datoteka nije pronađena** prilikom pokušaja pristupa. Taj problem treba prijavljeni kao slučaj podršku za daljnje istraživanja. 



