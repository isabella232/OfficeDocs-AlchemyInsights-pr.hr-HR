---
title: Problemi s performansama – SharePoint ili OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068386"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ili OneDrive sporo, nedostupno ili nije dostupno za više korisnika

SharePoint ili OneDrive može biti spor, nedostupan ili nedostupan ili može prikazati servis nedostupan ili 503 pogreške, iz nekoliko razloga:
  
- Ako je web-mjesto sustava SharePoint ili OneDrive sporo ili odgođeno za više korisnika, možda postoji problem s privremenim servisom u kojem korisnici doživljavaju povremene odgode ili pogreške u navigaciji pri pristupu SharePoint web-lokacijama ili sadržaju servisa OneDrive. Provjerite je li vaša tvrtka ili ustanova utjecala na [nadzornu ploču za zdravlje servisa](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) .
  
- Korisnici mogu primiti *503 poslužitelj je zauzet* pogreška prilikom pokušaja navigacije na SharePoint ili OneDrive web-mjesta. Ta se pogreška može uzrokovati ograničavanjem unutar SharePoint servisa. SharePoint Online koristi ograničavanje za održavanje optimalne performanse i pouzdanost usluge SharePoint online. Reguliranje ograničava broj korisničkih akcija ili istodobnih poziva (po skripti ili kodu) kako bi se spriječilo prekomjerno korištenje resursa. Za više informacija o regulaciji Pogledajte, [Izbjegavajte ograničavanje ili blokiranje u sustavu SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Ako osjetite spore performanse s **klasičnim** ili **modernim** SharePoint web-mjestom ili stranicom, upotrijebite [dijagnostički alat stranice](https://aka.ms/perftool) za analizu stranica.
  
- Ako i dalje doživite opću sporu izvedbu, pregledajte resurse na dnu ovog članka: [Uvod u podešavanje performansi za SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  