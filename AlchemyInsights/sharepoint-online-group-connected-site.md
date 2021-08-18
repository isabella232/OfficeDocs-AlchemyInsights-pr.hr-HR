---
title: Dodavanje grupe na web-SharePoint web-mjesto
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dd159b8b9e141c2fb448bae5fb624efe1014d7d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318116"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Uobičajeni problemi prilikom stvaranja grupnog povezanog web-mjesta u SharePoint

1. Ako ste izbrisali grupu i njezino povezano web-mjesto i želite stvoriti drugo web-mjesto s istim URL-om, morate trajno ukloniti prethodno web-mjesto.

   - Preuzimanje [ljuske za upravljanje SPO-om](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Dodatne informacije o početku rada s ljuskom Powershell potražite u članku Početak [rada s ljuskom SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Uklonite web-mjesto s izbrisanih [web-mjesta pomoću cmdleta Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell. Powershell mora trajno izbrisati grupna web-mjesta.

1. Ako stvarate web-mjesto povezano s grupom i primate upozorenje: još jedna grupa s istim **pseudonimom** već postoji , provjerite postojeće grupe iz [Centar za administratore okruženja Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Da biste riješili problem, izbrišite postojeću grupu ako više nije potrebna ili stvorite web-mjesto s dodijeljenim drugim pseudonimom.

1. Postoje različiti načini stvaranja i korištenja modernih grupa s SharePoint.

   - Postojeća web-mjesta možete povezati s Microsoft 365 grupe. Dodatne informacije potražite u [članku Povezivanje grupi Microsoft 365 pomoću korisničkog SharePoint sučelja](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Da biste stvorili Microsoft 365 povezanog web-mjesta, morate stvoriti timski [web-mjesto.](https://admin.microsoft.com/sharepoint)
