---
title: Povezivanjem SharePoint Designer
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: a4aeaeaea5743c276b907c78317ff30f5610be81
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36508415"
---
# <a name="sharepoint-designer-connection-issues"></a>Povezivanjem SharePoint Designer 

Ako SharePoint Designer se pojavili problemi veze na SharePoint web-mjesta, pokušajte sljedeća rješenja uobičajenih.

Korak 1: Provjerite je li SharePoint Designer 2013 ažurira s [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) i [kolovoz 2, 2016 ažuriranje SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Korak 2: Poništite lokalne predmemorije datoteke:

1. Zatvorite SharePoint Designer 2013.

2. Uklanjanje svih datoteka pronađenih u svakoj od sljedećih mapa na lokalnom računalu.

    - Extensions\Cache %APPDATA%\Microsoft\Web poslužitelj
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Otvorite SharePoint 2013 dizajner i unesite račun da biste vidjeli ako radi.

Korak 3: [Omogući provjeru autentičnosti Moderna 2013 Office na Windows uređajima](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Korak 4: Administratori morat ćete **Dopustiti prilagođene skripte** u postavkama SharePoint administraciju Center dopustiti povezivanje SharePoint Designer. Pogledajte [Dopusti ili spriječiti prilagođene skripte](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) dodatne informacije.


