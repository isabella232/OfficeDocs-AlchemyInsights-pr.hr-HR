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
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771893"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ili OneDrive spori, nedostupni ili nedostupni za više korisnika

SharePoint ili OneDrive mogu biti spori, nedostupni ili nedostupni ili mogu prikazati servis nedostupni ili 503 pogrešaka, iz nekoliko razloga:
  
- Ako je web-mjesto sustava SharePoint ili OneDrive sporo ili odgođeno za više korisnika, možda postoji privremeni problem s servisom u kojem korisnici mogu doživjeti povremeni kašnjenje ili pogreške prilikom navigacije prilikom pristupanja web-mjestima sustava SharePoint ili sadržaju servisa OneDrive. Provjerite je li vaša tvrtka ili ustanova utjecala na [nadzornu ploču zdravstvenog stanja servisa](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) .
  
- Kada pokušate prijeći na SharePoint ili web-mjesta servisa OneDrive, korisnici mogu primiti *503 poslužitelj je zauzet* . Ovu pogrešku može prouzročiti ograničavanje unutar servisa sustava SharePoint. SharePoint Online koristi ograničavanje za održavanje optimalnih performansi i pouzdanosti servisa SharePoint Online. Ograničavanjem se ograničava broj korisničkih radnji ili istodobnih poziva (skriptom ili kodom) radi sprječavanja prekomjernog korištenja resursa. Dodatne informacije o [ograničavanju potražite u članku izbjegavanje ograničenja ili blokiranja u sustavu SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Ako osjetite spore performanse uz **klasično** ili **moderno** web-mjesto sustava SharePoint ili stranicu, upotrijebite [dijagnostički alat za stranicu](https://aka.ms/perftool) da biste analizirali stranice.
  
- Ako i dalje imate općenite spore performanse, pregledajte resurse pri dnu ovog članka: [Uvod u tuning performansi za SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  