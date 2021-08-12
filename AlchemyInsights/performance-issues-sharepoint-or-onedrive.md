---
title: Problemi s performansama – SharePoint ili OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 921aae7eba8487c5600f290fd671ef2675372e6af0478b913e38354856cbaa22
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911834"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ili OneDrive, nedostupni ili nedostupni za više korisnika

SharePoint ili OneDrive može biti spor, nepristupačan ili nedostupan ili može prikazati pogreške servisa koje nisu dostupne ili 503 pogreške iz nekoliko razloga:
  
- Ako je SharePoint ili OneDrive-mjesto sporo ili odgođeno za više korisnika, može doći do privremenog problema sa servisom u kojem korisnici naiskuju povremene kašnjenja ili navigacijske pogreške prilikom pristupa web-mjestima SharePoint ili OneDrive sadržaju. Provjerite [nadzornu ploču stanja servisa](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) da biste vidjeli utječe li vaša tvrtka ili ustanova na to.
  
- Korisnici mogu primiti *503 poslužitelj* je zauzet pogreška prilikom pokušaja navigacije do SharePoint ili OneDrive web-mjesta. Ta se pogreška može uzrokovati ograničavanjem unutar servisa SharePoint servisa. SharePoint Online koristi ograničavanje za održavanje optimalnih performansi i pouzdanosti servisa SharePoint Online. Ograničavanjem se ograničava broj korisničkih radnji ili istodobnih poziva (skriptom ili kodom) radi sprječavanja prekomjernog korištenja resursa. Dodatne informacije o ograničavanju potražite u članku Izbjegavanje ograničavanja ili blokiranja [na servisu SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Ako naiđete  na spore performanse s klasičnim ili **modernim** SharePoint web-mjestom ili stranicom, pomoću alata [za dijagnostiku](https://aka.ms/perftool) stranice analizirajte stranice.
  
- Ako i dalje imate općenite spore performanse, pregledajte resurse pri dnu ovog članka: [Uvod u ugađanje performansi za SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  