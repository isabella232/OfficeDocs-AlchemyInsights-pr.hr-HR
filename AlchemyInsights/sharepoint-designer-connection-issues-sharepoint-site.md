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
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511536"
---
# <a name="sharepoint-designer-connection-issues"></a>Problemi s povezivanjem programa SharePoint Designer 

Ako SharePoint Designer ima problema s povezivanjem sa sharepoint web-mjestima, isprobajte sljedeća uobičajena rješenja.

Prvi korak: provjerite je li SharePoint Designer 2013 ažuriran sa [servisnim paketom SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) i [ažuriranjem kolovoza 2, 2016 za SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



2. korak: izbrišite lokalne datoteke predmemorije:

1. Zatvorite SharePoint Designer 2013.

2. Na lokalnom računalu uklonite sve datoteke pronađene u svakoj od sljedećih mapa.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Otvorite SharePoint Designer 2013 i ponovno unesite račun da biste vidjeli funkcionira li.

3. korak: [omogućite modernu provjeru autentičnosti za Office 2013 na uređajima sa sustavom Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Korak 4: Administratori će morati **dopustiti prilagođenu skriptu** u postavkama centra za administratore sustava SharePoint da bi omogućili vezu programa SharePoint Designer. Dodatne informacije [potražite u članku Dopuštanje ili sprječavanje prilagođene skripte.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


