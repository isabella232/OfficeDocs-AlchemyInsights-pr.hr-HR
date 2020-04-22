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
ms.openlocfilehash: 049ef5acd80d64e00315ba07f274567e6a251904
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/21/2020
ms.locfileid: "43642136"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problemi prilikom stvaranja web-mjesta povezanog grupe u sustavu SharePoint

1. Neki uobičajeni problemi na koje se susreću prilikom stvaranja ili ponovnog stvaranja povezanog web-mjesta grupe.
Ako ste izbrisali grupu i povezano web-mjesto i želite stvoriti drugo web-mjesto s istim URL-om, morat ćete trajno ukloniti prethodno web-mjesto.

   - Preuzimanje [datoteka SPO Uprava Ljuska](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Dodatne informacije o početku rada s powershellom potražite u članku [Početak rada s ljuskom za upravljanje sustavom SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Uklonite web-mjesto s izbrisanih web-mjesta pomoću cmdleta [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell. Powershell je potrebno trajno izbrisati grupna web-mjesta.

1. Ako stvarate povezano web-mjesto grupe i primate upozorenje: **Još jedna grupa s istim pseudonimom već postoji**, provjerite postojeće grupe iz Centra za [administratore sustava Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Da biste riješili problem, izbrišite postojeću grupu ako više nije potrebna ili stvorite web-mjesto s dodijeljenim drugim pseudonimom.

1. Postoje različiti načini stvaranja i korištenja modernih grupa u sustavu SharePoint.

   - Postojeća web-mjesta možete povezati s grupom sustava Office 365. Dodatne informacije potražite u članku [Povezivanje grupe sustava Office 365 pomoću korisničkog sučelja sustava SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Da biste stvorili povezano web-mjesto grupe sustava Office 365, morat ćete stvoriti [timsko web-mjesto](https://admin.microsoft.com/sharepoint).
