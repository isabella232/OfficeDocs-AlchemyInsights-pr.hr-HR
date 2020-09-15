---
title: Ograničavanje pristupa u sustavu SharePoint ili na servisu OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700447"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ograničavanje pristupa u sustavu SharePoint ili na servisu OneDrive

Postoji mnogo načina ograničavanja pristupa servisima sustava SharePoint Online/OneDrive. U nastavku su navedene različite metode ograničavanja pristupa. 

**Ograničenje dozvola**

U sustavima SharePoint online i OneDrive za tvrtke ograničavamo pristup stavkama kao što su web-mjesta, datoteke i mape samo ako dajemo pristup tim grupama/pojedincima koji bi trebali imati pristup.

- [Prilagodba dozvola za popis ili biblioteku sustava SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Prilagodba dozvola web-mjesta sustava SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Promjena dozvola na podmapi](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Upravljanje pristupom iz neupravljanih uređaja](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Kao SharePoint ili globalni administrator možete blokirati ili ograničiti pristup sadržaju sustava SharePoint i na servisu OneDrive iz neupravljanih uređaja (one koji nisu hibrid ili kompatibilni u programu Intune).

**Ograničenje mrežnog mjesta**

Kao IT administrator možete kontrolirati pristup resursima sustava SharePoint i servisu OneDrive na temelju definiranih mrežnih mjesta kojima vjerujete. To je poznato i kao pravilo utemeljeno na lokaciji. Dodatne informacije potražite [u članku Upravljanje pristupom na podatke sustava SharePoint online i na servisu OneDrive na temelju mrežnog mjesta](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Ograničenje zaključavanja web-mjesta** 

U sustavu SharePoint Online možete zaključati zbirku web-mjesta, pa nitko ne može pristupiti. Ovo je postavljeno putem komponente PowerShell i [ljuske za upravljanje sustavom SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) pomoću svojstva [set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.

**Ograničavanje korisnika na stvaranje web-mjesta ili podmjesta**

Kao administrator sustava SharePoint ili globalni administrator korisnicima možete omogućiti stvaranje i administriranje vlastitih web-mjesta sustava SharePoint, određivanje vrsta web-mjesta koje mogu stvarati i određivanje mjesta web-mjesta. Dodatne informacije potražite [u članku Upravljanje stvaranjem web-mjesta u sustavu SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

