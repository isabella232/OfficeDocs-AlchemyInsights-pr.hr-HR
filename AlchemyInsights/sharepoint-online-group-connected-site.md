---
title: Dodavanje grupe na SharePoint web-mjesto
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: e7bfabe1555bb94e915f8544d460deecce6171be
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770343"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problemi prilikom stvaranja grupnog povezanog web-mjesta u sustavu SharePoint

1. Neki uobičajeni problemi naišli su pri stvaranju ili ponovnom stvaranju grupe povezanog web-mjesta.
Ako ste izbrisali grupu i njegovo povezano web-mjesto i želite stvoriti drugo web-mjesto s istim URL-om, morat ćete trajno ukloniti prethodno web-mjesto.

   - Preuzmite " [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429) "
   - Dodatne informacije o tome kako početi s PowerShell potražite u nastavku [programa SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Uklonite web-mjesto iz izbrisanih web-mjesta pomoću cmdleta [Ukloni-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell. PowerShell je potrebno trajno izbrisati grupe web-mjesta.

1. Ako stvarate grupnu povezanu stranicu i primite upozorenje: **druga grupa s istim pseudonimom već postoji**, provjerite postojeće grupe iz [Office 365 iz centra za administraciju](https://admin.microsoft.com/AdminPortal/Home#/groups). Da biste riješili problem, izbrišite postojeću grupu ako više nije potrebna ili stvorite web-mjesto s dodijeljenim drugim pseudonimom.

1. Postoje različiti načini stvaranja i korištenja modernih grupa u sustavu SharePoint.

   - Postojeća web-mjesta možete povezati s Officeovom 365 grupom. Dodatne informacije potražite [u okviru Povezivanje grupe sustava Office 365 pomoću korisničkog sučelja sustava SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Za stvaranje povezanog web-mjesta sustava Office 365, morat ćete stvoriti [timsko web-mjesto](https://admin.microsoft.com/sharepoint).
