---
title: Tijek rada se ne pokreće
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794759"
---
# <a name="workflow-is-not-starting"></a>Tijek rada se ne pokreće

- Tijekovi rada sustava SharePoint 2010 i SharePoint 2013 ne počinju.

    - Ako se tijek rada ne pokreće, možda postoji privremeni problem s servisom u kojem korisnici mogu iskusiti povremeni kašnjenje s napretkom tijeka rada. Provjerite je li vaša tvrtka ili ustanova utjecala na [nadzornu ploču zdravstvenog stanja servisa](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) .

    - Ako je prošlo više od 24 sata otkad ste prvi put vidjeli taj problem, prijavite karticu za podršku. U mnogim slučajevima već radimo na rješenju. Dodajte nam najmanje 24 sata da biste dovršili rješenje.

- Tijekovi rada sustava SharePoint 2010 odgođeni su pri pokretanju.

    - To se događa ako se tijek rada aktivira u velikim grupama. (na primjer, kada se nekoliko stavki odmah doda).

    - Tijekovi rada nisu dizajnirani za izvođenje u stvarnom vremenu, pa je kašnjenje prema dizajnu.

   -  Ako je tijek rada kompleksan Extensible Object Markup Language (XMOL), kompilacija može biti spora. Provjerite [ovaj](https://support.microsoft.com//kb/3043697) članak.

    - Trebali biste pojednostavniti tijek rada ili ga ponovno dizajnirati pomoću vrste platforme tijeka rada sustava Microsoft SharePoint 2013.

    - Ako je povijest tijeka rada porasla, možda želite očistiti stavke ili stvoriti novi popis povijesti.

        Dodatne informacije: [čišćenje povijesti tijeka rada](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Povezane teme
Želite li isprobati Microsoft Flow u sustavu SharePoint Online?
- [Stvaranje toka](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


