---
title: Alat za izvoz elektroničkih predočavanja elektroničkih elektroničkih podataka
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814580"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Ne možete instalirati ili pokrenuti alat za izvoz predočavanja elektroničkih podataka?

Ako ne možete instalirati ili pokrenuti alat za izvoz e-otkrivanja da biste preuzeli rezultate pretraživanja, provjerite sljedeće:
  
- Računalo koje koristite zadovoljava sljedeće preduvjete:

  - 32-bitne ili 64-bitne verzije sustava Windows 7 i novije verzije

  - Microsoft .NET Framework 4.7

  - Podržani preglednik:

  - Microsoft Edge

    Ili

  - Internet Explorer 10 i novije verzije

    Drugi preglednici, kao što su Google Chrome i Mozilla Firefox, nisu podržani.

- Vaša tvrtka ili ustanova može se povezati s krajnjom tonom na servisu Azure, **\* a to je .blob.core.windows.net** (zamjenski znak predstavlja jedinstveni identifikator za posao izvoza).

- Uloga Izvoz dodijeljena vam je u centru za sigurnosnu usklađenost sustava Microsoft 365. &amp; Ta se uloga po zadanom dodjeljuje samo grupi uloga upravitelja predočavanja elektroničkih elektroničkih obveza. Pogledajte [dodjela dozvola za predočavanje elektroničkih datoteka](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Dodatne informacije potražite u članku Izvoz [rezultata pretraživanja sadržaja](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

Ako izvozite više od 100 K poštanskih sandučića, morat ćete koristiti sljedeću ljusku Powershell da biste preuzeli rezultate izvoza: izvoz rezultata iz više  [od 100K poštanskih sandučića](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).