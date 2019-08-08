---
title: Zamijeni vaš Classic korijensko web-mjesto s Moderna web-mjesta
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "2579"
- "9000687"
ms.openlocfilehash: dad7d7a52222dc09aea532714a93ca89c0d9ae19
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/07/2019
ms.locfileid: "36245939"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Zamijeni vaš Classic korijensko web-mjesto s Moderna web-mjesta

Ako je vaše okruženje postavljena prije Travanj 2019 korijensko web-mjesto možete promijeniti Moderna web-mjesta pomoću Microsoft PowerShell:

- Ako imate različite web-mjesta koje želite koristiti kao korijen web-mjesta, s njim možete zamijeniti (Zamijeni) korijenskog web-mjesta. 
    - Koristite [Pozovite SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) Zamijeni mjesto web-mjesta s drugog web-mjesta vrijeme arhiviranja izvornog web-mjesta. Dostupno za timskog web-mjesta (nije povezano s grupom) i komunikacije web-mjesta. 

- Dodatne mogućnosti će biti uvedene uskoro koji će vam omogućiti zadržati pomoću sadržaja na web-mjestu, ali pretvaranje postojećeg web-mjesta komunikacije web-mjesta. 
>[!Important]
>Ove mogućnosti će biti poslednjeg postupno. Nastavite provjerite Office 365 poruku centar za ažuriranja. 

## <a name="known-issues-with-swapping-sites"></a>Poznati problemi s zamjene web-mjesta

- Ciljno mjesto može vratiti "nije pronađen" Pogreška (HTTP 404) za kratkog vremenskog razdoblja.
- Sadržaj će morati biti ponovno pretražiti da radi indeksiranja da biste ažurirali indeks pretraživanja. Postoji bez ručnog korak potreban - to će učiniti automatski.
- Ništa zavise "statički" veze (poput datoteka sinkronizacije datoteka i OneNote) morat ćete ručno ispraviti.
- Izvorišnog web-mjesta je organizacijske vijesti, ažurirajte URL.Nabavite popis svih web-mjesta organizacijske vijesti.
- Web-mjesta Project Server možda morati provjeriti da biste bili sigurni da su i dalje povezani ispravno.





