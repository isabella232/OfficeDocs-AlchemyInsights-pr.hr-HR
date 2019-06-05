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
ms.openlocfilehash: 7451cfe957545537298f57feb5b47bd6d43cddbf
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716884"
---
# <a name="sharepoint-designer-connection-issues"></a>Povezivanjem SharePoint Designer 

<p>Ako SharePoint Designer se pojavili problemi veze na SharePoint web-mjesta, pokušajte sljedeća rješenja uobičajenih.</p> <p><strong>Korak 1:</strong> <strong>Ažurirati provjerite SharePoint Designer&nbsp; </strong></p> <ul> <li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=35491">SharePoint Designer 2013</a></li> <li><a href="https://support.microsoft.com/en-us/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1">SharePoint Designer Service Pack 1 (SP1)</a></li> <li><a href="https://support.microsoft.com/en-us/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721">Ažuriranje SharePoint Designer 2013 (KB3114721)</a></li> </ul> <p><strong>Korak 2:</strong> <strong>Poništite datoteke lokalne predmemorije</strong>&nbsp;</p> <ol> <li style="font-weight: 400;">Zatvorite SharePoint Designer 2013.&nbsp;</li> <li style="font-weight: 400;">Na lokalnom računalu pronađite sljedeće mape da biste uklonili predmemorirane datoteke.&nbsp;</li> <li style="font-weight: 400;">Pritisnite <strong>Start -&gt; Pokreni</strong> i izbrisati sve datoteke pronađena pod svakom od na ispod mjesta.&nbsp;<br /><br />Extensions\Cache %APPDATA%\Microsoft\Web poslužitelj<br />%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache<br />%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</li> <li style="font-weight: 400;">Otvorite SharePoint 2013 dizajner i unesite račun da biste vidjeli ako radi.</li> </ol> <p><strong>Korak 3:</strong> <a href="https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=%252fen-us%252farticle%252fEnable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&amp;view=o365-worldwide"> <strong>Omogući provjeru autentičnosti Moderna 2013 Office na uređajima za Windows</strong></a>&nbsp;</p> <p><strong>Korak 4:</strong> <strong>Dopusti Prilagođena skripta dopustiti povezivanje SharePoint Designer će morati administratori</strong>.</p> <p>Za detaljne korake, Primjeri i razmatranja pogledajte <a href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">Dopusti ili spriječiti prilagođene skripte</a>.&nbsp;</p>


