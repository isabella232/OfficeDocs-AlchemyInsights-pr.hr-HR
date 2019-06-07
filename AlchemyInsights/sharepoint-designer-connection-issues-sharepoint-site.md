---
title: SharePoint Online razine dozvola
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760685"
---
# <a name="sharepoint-designer-connection-issues"></a>Povezivanjem SharePoint Designer 

Ako SharePoint Designer se pojavili problemi veze na SharePoint web-mjesta, pokušajte sljedeća rješenja uobičajenih.

Korak 1: Provjerite ažurirati programa SharePoint Designer.

- [SharePoint Designer 2013](https://www.microsoft.com/download/details.aspx?id=35491)

- [SharePoint Designer Service Pack 1 (SP1)](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [Ažuriranje SharePoint Designer 2013 (KB3114721)](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

Korak 2: Poništite datoteke lokalne predmemorije

- Zatvorite SharePoint Designer 2013.

- Na lokalnom računalu pronađite sljedeće mape da biste uklonili predmemorirane datoteke.

- Kliknite Start, Run i Izbriši sve datoteke pronaći pod svakom od na ispod mjesta.

%APPDATA%\Microsoft\Web server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

Otvorite SharePoint 2013 dizajner i unesite račun da biste vidjeli ako radi.

Korak 3: [Omogući provjeru autentičnosti Moderna 2013 Office na uređajima za Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

Korak 4: Administratori morat ćete dopustiti Prilagođena skripta za omogućivanje veze SharePoint Designer.

Za detaljne korake, Primjeri i razmatranja pogledajte [Dopusti ili spriječiti prilagođene skripte](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


