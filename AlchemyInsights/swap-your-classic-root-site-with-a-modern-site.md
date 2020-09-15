---
title: Swap svoje klasično korijensko web-mjesto s modernim web-mjestom
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691171"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Swap svoje klasično korijensko web-mjesto s modernim web-mjestom

Ako je okruženje postavljeno prije travnja 2019, korijensko web-mjesto možete promijeniti na moderno web-mjesto pomoću komponente Microsoft PowerShell:

- Ako imate drugo web-mjesto koje želite koristiti kao korijensko web-mjesto, pomoću nje možete zamijeniti [(swap) korijensko web-mjesto](https://docs.microsoft.com/sharepoint/modern-root-site) . 
    - Pomoću poziva [-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) mijenjate mjesto web-mjesta s drugim web-mjestom tijekom arhiviranja izvornog web-mjesta. Dostupno za obje timsko web-mjesto (nije povezano s grupom) i komunikacijskim web-mjestom. 

- Uskoro će biti uvedene dodatne mogućnosti koje će vam dopustiti da nastavite koristiti sadržaj na web-mjestu, ali da biste postojeće web-mjesto pretvorili u komunikacijsko web-mjesto. 
>[!Important]
>Te će se mogućnosti postupno izkotrljali. Nastavite provjeravati centar za poruke radi ažuriranja. 

## <a name="known-issues-with-swapping-sites"></a>Poznati problemi s zamjenom web-mjesta

- Odredišno web-mjesto može u kratkom vremenskom periodu vratiti pogrešku "nije pronađeno" (HTTP 404).
- Sadržaj će se morati ponovno vratiti da bi se ažurirao indeks pretraživanja. Nije potreban ručni korak – to će se obaviti automatski.
- Sve što ovisi o "statički" vezama (kao što su sinkronizacija datoteka i datoteke programa OneNote) morat će se ručno ispraviti.
- Ako je izvorišno mjesto bilo organizacijsko web-mjesto vijesti, ažurirajte URL.Nabavite popis svih web-mjesta organizacijskih vijesti.
- Web-mjesta projektnog poslužitelja možda će se morati potvrditi da bi se osiguralo da su i dalje ispravno povezani.
