---
title: Dodavanje grupe na web-mjesto sustava SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771191"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problemi prilikom stvaranja grupnog povezanog web-mjesta u sustavu SharePoint

1. Neki se Česti problemi susreću prilikom stvaranja ili ponovnog stvaranja grupnog povezanog web-mjesta.
Ako ste izbrisali grupu i njegovo povezano web-mjesto i želite stvoriti drugo web-mjesto s istim URL-om, morat ćete trajno ukloniti prethodno web-mjesto.

   - Preuzimanje [ljuske za upravljanje SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429) -om
   - Dodatne informacije o pokretanju pomoću komponente PowerShell potražite u članku [početak rada s ljuskom za upravljanje sustavom SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Uklonite web-mjesto s izbrisanih web-mjesta pomoću cmdleta [Remove-Spodeletedweb](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell. PowerShell je dužan trajno izbrisati grupna web-mjesta.

1. Ako stvarate grupno povezano web-mjesto i primate upozorenje: **druga grupa s istim pseudonimom već postoji**, provjerite postojeće grupe iz centra za [administratore sustava Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Da biste riješili problem, izbrišite postojeću grupu ako više nije potrebna ili stvorite web-mjesto s dodijeljenim drugim pseudonimom.

1. Postoje razni načini stvaranja i korištenja suvremenih grupa u sustavu SharePoint.

   - Možete povezati postojeća web-mjesta s grupom Microsoft 365. Dodatne informacije potražite u članku [Povezivanje grupe Microsoft 365 pomoću korisničkog sučelja sustava SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Da biste stvorili web-mjesto povezanih s grupom Microsoft 365, morat ćete stvoriti [timsko web-mjesto](https://admin.microsoft.com/sharepoint).
