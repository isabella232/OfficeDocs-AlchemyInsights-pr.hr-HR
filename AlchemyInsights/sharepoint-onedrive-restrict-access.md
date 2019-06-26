---
title: Ograničiti pristup u SharePoint ili OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: db84f77208dca60c6dee98cdb0c7f1ea7fa8fe17
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223704"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ograničiti pristup u SharePoint ili OneDrive

Postoji mnogo načina ograničiti pristup Internetu OneDrive SharePoint services. Ove različite metode ograničenje pristupa istaknuti su ispod. 

**Ograničenje dozvola**

U SharePoint Online i OneDrive za poslovne, možemo ograničiti pristup stavki kao što su web-mjesta, datoteke i mape samo Davanjem pristup tim grupama/pojedinaca koji treba imati pristup.

- [Prilagodba dozvola za SharePoint popis ili biblioteku](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Prilagodba dozvola SharePoint web-mjesta](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Promijenite dozvole na podmapi](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Kontrolu pristupa iz neupravljanog uređaja](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Kao SharePoint ili globalni administrator sistema Office 365, možete blokirati ili ograničiti pristup SharePoint i OneDrive sadržaja iz neupravljanog uređaja (one ne hibridno AD spojena ili sa standardom u Intune).

**Mrežni mjesto ograničenja**

Kao IT administrator, možete kontrolirati pristup resursima sustava SharePoint i OneDrive na temelju definiranih mrežnim mjestima kojima vjerujete. To je poznato kao mjesto temelji pravila. Za dodatne informacije pogledajte [pristup kontrolu SharePoint Online i OneDrive podatke na temelju mrežnog mjesta](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Ograničenje zaključavanja web-mjesta** 

Unutar SharePoint Online imaju mogućnost za zaključavanje zbirke web-mjesta tako da nitko ima pristup. Postavljena je putem PowerShell i [Online ljuske za upravljanje SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) pomoću svojstva - stanje zaključanosti [Skup SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) .

**Ograničenje korisnika u stvaranju web-mjesta ili podmjesta**

Kao administraciju SharePoint ili globalni administrator sistema Office 365, možete dopustiti korisnicima stvaranje i administrirati vlastite SharePoint web-mjesta, odredite Kakvu vrstu web-mjesta mogu stvoriti, i navedite mjesto web-mjesta. Za dodatne informacije pogledajte [Upravljanje stvaranja web-mjesta u SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

