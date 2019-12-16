---
title: Problemi s povezivanjem programa SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051705"
---
# <a name="sharepoint-designer-connection-issues"></a>Problemi s povezivanjem programa SharePoint Designer 

Ako SharePoint Designer ima problema s povezivanjem na SharePoint web-mjesta, pokušajte sljedeća uobičajena rješenja.

Korak 1: Provjerite je li SharePoint Designer 2013 ažuriran pomoću [programa SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) i [2. kolovoza 2016 Update za SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Korak 2: očistite lokalne datoteke predmemorije:

1. Zatvorite SharePoint Designer 2013.

2. Na lokalnom računalu uklonite sve datoteke pronađene u svakoj od sljedećih mapa.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Otvorite SharePoint Designer 2013 i ponovno unesite račun da biste vidjeli radi li.

Korak 3: [omogućite modernu provjeru autentičnosti za Office 2013 na uređajima sa sustavom Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Korak 4: Administratori će morati **dopustiti prilagođenu skriptu** u postavkama administratorskog centra za SharePoint da bi se omogućilo povezivanje programa SharePoint Designer. Pogledajte [Dopusti ili spriječi prilagođenu skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) za više informacija.


