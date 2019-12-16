---
title: Ograničavanje pristupa u sustavu SharePoint ili servisu OneDrive
ms.author: pebaum
author: pebaum
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 242388af3ae8887616fc123f24502a8e5ac8dfbe
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053757"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ograničavanje pristupa u sustavu SharePoint ili servisu OneDrive

Postoji mnogo načina ograničavanja pristupa uslugama SharePoint Online/OneDrive. Ove različite metode ograničavanja pristupa navedene su u nastavku. 

**Ograničenje dopuštenja**

U sustavu SharePoint online i servisu OneDrive za tvrtke ograničavamo pristup stavkama kao što su web-mjesta, datoteke i mape samo dajući pristup tim grupama/pojedincima koji bi trebali imati pristup.

- [Prilagodba dozvola za SharePointov popis ili biblioteku](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Prilagodba dozvola web-mjesta sustava SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Promjena dozvola u podmapi](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Upravljanje pristupom s neupravljanih uređaja](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Kao SharePoint ili Global admin u sustavu Office 365, možete blokirati ili ograničiti pristup sadržaju sustava SharePoint i OneDrive s neupravljanih uređaja (oni koji nisu hibridni AD spojeni ili usklađeni u Intune).

**Ograničenje mrežnog mjesta**

Kao IT admin možete kontrolirati pristup resursima sustava SharePoint i OneDrive na temelju definiranih mrežnih mjesta kojima vjerujete. To se također naziva politikom temeljenom na lokaciji. Dodatne informacije potražite u [kontroli pristupa podacima sustava SharePoint online i servisu OneDrive na temelju mrežnog mjesta](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Ograničenje zaključavanja web-mjesta** 

U sustavu SharePoint Online imate mogućnost zaključavanja zbirke web-mjesta, tako da nitko nema pristup. To je postavljeno putem PowerShell i [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) pomoću [skup-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate svojstvo.

**Ograničavanje korisnika na stvaranje web-mjesta ili podmjesta**

Kao administrator sustava SharePoint ili Office 365 Global admin, možete dopustiti korisnicima stvaranje i administriranje vlastitih web-mjesta sustava SharePoint, odrediti koja vrsta web-mjesta mogu stvoriti i odrediti mjesto web-mjesta. Dodatne informacije potražite [u okviru Upravljanje stvaranjem web-mjesta u sustavu SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

