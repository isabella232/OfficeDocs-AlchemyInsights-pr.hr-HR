---
title: Dodavanje grupe na Web-mjesto sustava SharePoint
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
ms.openlocfilehash: 5dab9fce935936898927afd55f8f6e9260249157
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582803"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problemi prilikom stvaranja web-mjesta povezanog s grupom u sustavu SharePoint

1. Neki uobičajeni problemi naišli su prilikom stvaranja ili ponovnog stvaranja web-mjesta povezanog s grupom.
Ako ste izbrisali grupu i povezano web-mjesto i želite stvoriti drugo web-mjesto s istim URL-om, morat ćete trajno ukloniti prethodno web-mjesto.

   - Preuzimanje datoteka [SPO Uprava Ljuska](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Dodatne informacije o početku rada s dodatkom PowerShell [potražite u odjeljku Početak rada sa ljuskom za upravljanje sustavom SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Uklonite web-mjesto s izbrisanih web-mjesta pomoću cmdleta [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell. Powershell je potrebno trajno izbrisati grupna web-mjesta.

1. Ako stvarate web-mjesto povezano s grupom i primate upozorenje: **druga grupa s istim pseudonimom već postoji**, provjerite postojeće grupe iz centra za [administratore sustava Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Da biste riješili problem, izbrišite postojeću grupu ako više nije potrebna ili stvorite web-mjesto s drugim dodijeljenim pseudonimom.

1. Postoje različiti načini stvaranja i korištenja modernih grupa sa sustavom SharePoint.

   - Postojeća web-mjesta možete povezati s grupom sustava Microsoft 365. Dodatne informacije [potražite u odjeljku Povezivanje grupe sustava Microsoft 365 pomoću korisničkog sučelja sustava SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Da biste stvorili web-mjesto povezano s grupom sustava Microsoft 365, morat ćete stvoriti [timsko web-mjesto](https://admin.microsoft.com/sharepoint).
