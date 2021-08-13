---
title: Ograničavanje pristupa u SharePoint ili OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093809"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ograničavanje pristupa u SharePoint ili OneDrive

Pristup servisima na mreži/SharePoint/OneDrive možete ograničiti na mnogo načina. Ti su različiti načini ograničavanja pristupa navedeni u nastavku. 

**Ograničenje dozvola**

U SharePoint Online i OneDrive za tvrtke, ograničavamo pristup stavkama kao što su web-mjesta, datoteke i mape tako da samo tim grupama/pojedincima koji bi trebali imati pristup.

- [Prilagodba dozvola za SharePoint ili biblioteku](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Prilagodba dozvola SharePoint web-mjesta](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Promjena dozvola u podmapama](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Upravljanje pristupom s neupravljanih uređaja](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Kao SharePoint ili globalni administrator možete blokirati ili ograničiti pristup sadržaju SharePoint i OneDrive s neupravljanih uređaja (oni koji nisu hibridni AD spojeni ili usklađeni u aplikaciji Intune).

**Ograničenje mrežnog mjesta**

Kao IT administrator možete kontrolirati pristup resursima SharePoint i OneDrive na temelju definiranih mrežnih mjesta koja su pouzdana. To se naziva i pravilnikom utemeljenim na lokaciji. Dodatne informacije potražite u članku Upravljanje [pristupom SharePoint online i OneDrive podataka](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location) na temelju mrežnog mjesta

**Ograničenje zaključavanja web-mjesta** 

U SharePoint online imate mogućnost zaključavanja zbirke web-mjesta, pa nitko nema pristup. To se postavlja putem ljuske PowerShell [i SharePoint online management shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) pomoću svojstva [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Ograničavanje korisnika u stvaranju web-mjesta ili web-podmjesta**

Kao administrator SharePoint globalni administrator korisnicima možete dopustiti stvaranje i administriranje vlastitih web-SharePoint web-mjesta, određivanje vrste web-mjesta koja mogu stvoriti i određivanje mjesta web-mjesta. Dodatne informacije potražite u članku Upravljanje [stvaranjem web-mjesta u web-mjestu SharePoint online](https://docs.microsoft.com/sharepoint/manage-site-creation)

