---
title: Problemi s povezivanjem programa SharePoint Designer
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
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727163"
---
# <a name="sharepoint-designer-connection-issues"></a>Problemi s povezivanjem programa SharePoint Designer 

Ako SharePoint Designer doživljava probleme s vezom na web-mjesta sustava SharePoint, isprobajte sljedeća najčešća rješenja.

Prvi korak: Provjerite je li SharePoint Designer 2013 ažuriran uz [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) i [kolovoz 2, 2016 Update za SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Drugi korak: brisanje lokalnih datoteka predmemorije:

1. Zatvori SharePoint Designer 2013.

2. Na lokalnom računalu uklonite sve datoteke koje se nalaze u svakoj od sljedećih mapa.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\proxymontalicache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Otvorite SharePoint Designer 2013 i ponovno unesite račun da biste vidjeli funkcionira li.

Treći korak: [Omogućivanje moderne provjere autentičnosti za Office 2013 na uređajima sa sustavom Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Četvrti korak: Administratori će morati **dopustiti prilagođenu skriptu** u postavkama centra za administratore sustava SharePoint da bi se omogućila veza programa SharePoint Designer. Dodatne informacije potražite u članku [Omogućivanje i onemogućivanje prilagođene skripte](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .


