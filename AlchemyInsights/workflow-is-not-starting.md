---
title: Tijek rada se ne započinje
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: cf7bd95e9a8f1d0842f0abcf82c758d649e80c0f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049329"
---
# <a name="workflow-is-not-starting"></a>Tijek rada se ne započinje

- Tijekovi rada sustava SharePoint 2010 i SharePoint 2013 se ne počinju.

    - Ako se tijek rada ne započinje, možda postoji problem s privremenim servisima u kojem korisnici mogu doživjeti povremene odgode s napretkom tijeka rada. Provjerite je li vaša tvrtka ili ustanova utjecala na [nadzornu ploču za zdravstvenu službu](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) .

    - Ako je prošlo više od 24 sata od kada ste prvi put vidjeli ovaj problem, molimo prijavite ulaznicu za podršku. U mnogim slučajevima već radimo na rješenju. Molim vas, dajte nam najmanje 24 sata da dovršimo rješenje.

- Tijekovi rada sustava SharePoint 2010 odgođeni na početku.

    - To se događa ako se tijek rada aktivira u velikim serijama. (na primjer, kada se nekoliko stavki doda odjednom).

    - Tijekovi rada nisu dizajnirani za izvođenje u realnom vremenu, tako da je odgoda po dizajnu ponašanje.

   -  Ako je tijek rada složen Extensible Object Markup Language (XMOL), kompilacija može biti spora. Provjerite [ovaj](https://support.microsoft.com//kb/3043697) članak.

    - Trebali biste pojednostavniti tijek rada ili ga redizajnirati pomoću vrste platforme Microsoft SharePoint 2013 workflow.

    - Ako je vaša povijest tijeka rada narasla, možda želite očistiti stavke ili stvoriti novi popis povijesti.

        Dodatne informacije: [čišćenje povijesti tijeka rada](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Povezane teme
Želite li isprobati Microsoft Flow u sustavu SharePoint Online?
- [Stvori tok](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


