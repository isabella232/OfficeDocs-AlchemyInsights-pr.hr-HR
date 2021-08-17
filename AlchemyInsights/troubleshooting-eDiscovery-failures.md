---
title: 1490-troubleshooting-eDiscovery-failures
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 7b819b9bb18b5c0a635e708eccc0f23271267874707e5f3a7d41b633a05f2822
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105560"
---
# <a name="troubleshoot-content-search-errors"></a>Otklanjanje poteškoća s pretraživanjem sadržaja

Nailazite li na probleme s pretraživanjem sadržaja ili se prilikom izvoza rezultata pretraživanja pojavljuje pogreška?

Primate li, primjerice, sljedeće prilikom pokretanja pretraživanja?

- Pogreške cs008 ili CS012

- Pogreške o zauzetom/vremenskom rasporedu poslužitelja

- Došlo je do pogreške u aplikaciji

Ili prilikom pretraživanja ili izvoza rezultata iz velikog broja poštanskih sandučića (više od 100 000 poštanskih sandučića) primate li pogreške prilikom izvoza?

Za te vrste pogrešaka pokušajte ponovno potražiti mjesta sadržaja koja nisu uspjela. Dodatne  [informacije potražite](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) u ovom članku.

Ako izvozite više od 100 K poštanskih sandučića, morat ćete koristiti sljedeću ljusku Powershell da biste preuzeli rezultate izvoza: izvoz rezultata iz više  [od 100K poštanskih sandučića](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).
