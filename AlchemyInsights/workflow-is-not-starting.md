---
title: Tijek rada se ne započinje
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
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403735"
---
# <a name="workflow-is-not-starting"></a>Tijek rada se ne započinje

- Tijekovi rada sustava SharePoint 2010 i SharePoint 2013 ne počinju.

    - Ako se tijek rada ne započinje, možda postoji privremeni problem sa servisom u kojem korisnici mogu naiči na povremene kašnjenje tijeka rada. Provjerite [nadzornu ploču stanja servisa](https://admin.microsoft.com/AdminPortal/Home/servicehealth) da biste vidjeli utječe li vaša tvrtka ili ustanova na to.

    - Ako je prošlo više od 24 sata od kada ste prvi put vidjeli taj problem, prijavite kartu za podršku. U mnogim slučajevima već radimo na rješenju. Dajte nam najmanje 24 sata da dovršimo rješenje.

- Tijekovi rada sustava SharePoint 2010 odgođeni su pri pokretanju.

    - To se događa ako se tijek rada pokreće u velikim grupama. (na primjer, kada se doda nekoliko stavki odjednom).

    - Tijekovi rada nisu dizajnirani za pokretanje u stvarnom vremenu, pa je kašnjenje ponašanje po dizajnu.

   -  Ako je tijek rada složen jezik oznake extensible Object Markup Language (XMOL), sastavljanje može biti sporo. Pogledajte [ovaj](https://support.microsoft.com//kb/3043697) članak.

    - Trebali biste pojednostavniti tijek rada ili ga redizajnirati pomoću vrste platforme Tijek rada sustava Microsoft SharePoint 2013.

    - Ako je povijest tijeka rada narasla, možda želite očistiti stavke ili stvoriti novi popis povijesti.

        Dodatne informacije : [Čišćenje povijesti tijeka rada](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Povezane teme
Želite li isprobati Microsoft Flow u sustavu SharePoint Online?
- [Stvaranje tijeka](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
