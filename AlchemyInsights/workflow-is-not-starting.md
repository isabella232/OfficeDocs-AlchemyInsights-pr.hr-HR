---
title: Tijek rada se ne pokreće
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766089"
---
# <a name="workflow-is-not-starting"></a>Tijek rada se ne pokreće

- Tijekovi rada sustava SharePoint 2010 i SharePoint 2013 ne počinju.

    - Ako se tijek rada ne pokreće, možda postoji privremeni problem servisa zbog kojeg korisnici mogu naići na povremene odgode s napretkom tijeka rada. Provjerite [nadzornu ploču stanja servisa](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) da biste provjerili utječe li na vašu tvrtku ili ustanovu.

    - Ako je prošlo više od 24 sata otkad ste prvi put vidjeli taj problem, prijavite ulaznicu za podršku. U mnogim slučajevima već radimo na rješenju. Molimo Vas da nam najmanje 24 sata za dovršetak rješenja.

- Tijekovi rada sustava SharePoint 2010 odgođeni su pri pokretanju.

    - To se događa ako se tijek rada pokreće u velikim serijama. (na primjer, kada se dodaje nekoliko stavki odjednom).

    - Tijekovi rada nisu dizajnirani za pokretanje u stvarnom vremenu, stoga je kašnjenje ponašanje po dizajnu.

   -  Ako je tijek rada složen Extensible Object Markup Language (XMOL), kompilacija može biti spora. Provjerite [ovaj](https://support.microsoft.com//kb/3043697) članak.

    - Trebali biste pojednostaviti tijek rada ili ga redizajnirati pomoću vrste platforme Tijek rada sustava Microsoft SharePoint 2013.

    - Ako je povijest tijeka rada narasla, možda želite očistiti stavke ili stvoriti novi popis povijesti.

        Dodatne informacije : [Čišćenje povijesti tijeka rada](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Povezane teme
Želite li isprobati Microsoft Flow u sustavu SharePoint Online?
- [Stvori tijek](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


