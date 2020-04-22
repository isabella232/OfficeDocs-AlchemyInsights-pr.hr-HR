---
title: Ograničavanje pristupa u sustavu SharePoint ili OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692757"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ograničavanje pristupa u sustavu SharePoint ili OneDrive

Postoji mnogo načina za ograničavanje pristupa servisima sharepoint online/onedrive. Ove različite metode ograničavanja pristupa navedene su u nastavku. 

**Ograničenje dozvole**

U sustavima SharePoint Online i OneDrive za tvrtke ograničavamo pristup stavkama kao što su web-mjesta, datoteke i mape samo tako što omogućujemo pristup onim grupama/pojedincima koji bi trebali imati pristup.

- [Prilagodba dozvola za SharePoint popis ili biblioteku](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Prilagodba dozvola za web-mjesto sustava SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Promjena dozvola u podmapi](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Upravljanje pristupom s neupravljanih uređaja](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Kao sharepoint ili globalni administrator možete blokirati ili ograničiti pristup sadržaju sustava SharePoint i OneDrive s neupravljanih uređaja (oni koji se ne pridružuju ili su u skladu s njima u programu Intune).

**Ograničenje mrežnog mjesta**

Kao IT administrator možete kontrolirati pristup resursima sustava SharePoint i OneDrive na temelju definiranih mrežnih mjesta koja su vam pouzdana. To je poznato i kao pravila temeljena na lokaciji. Dodatne informacije potražite u članku [Upravljanje pristupom podacima sustava SharePoint Online i podacima servisa OneDrive na temelju mrežnog mjesta](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Ograničenje zaključavanja web-mjesta** 

U sustavu SharePoint Online možete zaključati zbirku web-mjesta, tako da nitko nema pristup. To je postavljeno putem komponente PowerShell i [ljuske za upravljanje sustavom SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) pomoću svojstva [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Ograničavanje korisnika u stvaranju web-mjesta ili podmjesta**

Kao administrator sustava SharePoint ili globalni administrator možete dopustiti korisnicima stvaranje i administriranje vlastitih web-mjesta sustava SharePoint, određivanje vrsta web-mjesta koja mogu stvoriti i određivanje mjesta web-mjesta. Dodatne informacije potražite u članku [Upravljanje stvaranjem web-mjesta u sustavu SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

