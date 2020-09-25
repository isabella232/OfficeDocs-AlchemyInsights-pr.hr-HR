---
title: 1490 – otklanjanje poteškoća – Rediscovery – pogreške
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
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277817"
---
# <a name="troubleshoot-content-search-errors"></a>Otklanjanje poteškoća s pretraživanjem sadržaja

Nailazite li na probleme s pretraživanjem sadržaja ili neuspjehom prilikom izvoza rezultata pretraživanja?

Na primjer, primate li sljedeće prilikom izvođenja pretraživanja?

- CS008 ili CS012 pogreške

- Pogreške zauzetosti poslužitelja/prekoračenja ograničenja

- Došlo je do pogreške u aplikaciji

Ako pretražujete ili izvozite rezultate iz velikog broja poštanskih sandučića (iznad 100.000 poštanskih sandučića), dobivate li pogreške u izvozu?

Da biste pronašli ove vrste pogrešaka, pokušajte pokušati potražiti mjesta sadržaja koja nisu uspjela. Dodatne informacije potražite u  [ovom članku](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .

Ako izvozite više od 100K poštanskih sandučića, morat ćete koristiti sljedeću PowerShell da biste preuzeli rezultate izvoza:  [Izvoz rezultata iz više od 100k poštanskih sandučića](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).
