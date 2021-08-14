---
title: SharePoint Problemi s povezivanjem dizajnera
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942017"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Problemi s povezivanjem dizajnera 

Ako SharePoint Designer nailazi na probleme s povezivanjem SharePoint web-mjesta, isprobajte sljedeća uobičajena rješenja.

Prvi korak: provjerite je li SharePoint Designer 2013 ažuriran sa servisnim paketom [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) i ažuriranjem za [2. kolovoza 2016. za SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Drugi korak: brisanje lokalnih datoteka predmemorije:

1. Zatvorite SharePoint Designer 2013.

2. Na lokalnom računalu uklonite sve datoteke pronađene u svakoj od sljedećih mapa.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Otvorite SharePoint Designer 2013 i ponovno unesite račun da biste vidjeli funkcionira li.

Treći korak: [omogućivanje moderne provjere autentičnosti za Office 2013 na Windows uređajima](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Četvrti korak: administratori će morati dopustiti **prilagođenu skriptu** u postavkama centra SharePoint administratora da bi omogućili SharePoint Designer. Dodatne [informacije potražite u članku Omogućivanje ili sprječavanje](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) prilagođene skripte.


