---
title: Dodavanje grupe web-mjesta sustava SharePoint
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750512"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Problemi kada stvaranja ili grupe povezani web-mjesta u SharePoint Online

Postoji nekoliko uobičajenih problema naišao je na prilikom stvaranja ili ponovno stvaranje grupe povezani web-mjesta.

 Ako ste izbrisali grupu i njegovih povezanih web-mjesta i želite stvoriti drugu web-mjesta s istim URL, morat ćete trajno ukloniti prethodno web-mjesto.

Preuzimanje [SPO upravljanja ljuske](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Dodatne informacije na Uvod powershell potražite [Uvod u SharePoint Online ljuske za upravljanje](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Uklanjanje web-mjesta iz izbrisane web-mjesta pomoću cmdleta [Ukloni-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell.

Ako izradi grupe povezanih web-mjesta i primiti upozorenje drugu grupu s iste alias već postoji, provjerite postojeće grupe iz [centra za administraciju sistema Office 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Da biste riješili taj problem, izbrišite postojeće grupe ako više nije potrebna ili stvaranje web-mjesta s različitim Pseudonim dodijeljen.

Stvaranje i korištenje Moderna grupe s SharePoint na različite načina.

Postojeća web-mjesta možete se povezati s Office 365 grupe. Za dodatne informacije pogledajte [povezivanje programa Office 365 grupu pomoću ineterface korisnika SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Da biste stvorili programa Office 365 grupe povezanih web-mjesta, trebat ćete stvoriti web-mjesto tima. Dodatne informacije potražite u članku [Kreiranje web-mjesto tima u SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

