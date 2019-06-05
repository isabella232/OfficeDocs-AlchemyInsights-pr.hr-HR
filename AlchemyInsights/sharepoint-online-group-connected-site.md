---
title: Dodavanje grupe web-mjesta sustava SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719474"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Stvaranje grupe povezanih web-mjesta u SharePoint Online

<p><strong>Postoji nekoliko uobičajenih problema naišao je na prilikom stvaranja ili ponovno stvaranje grupe povezani web-mjesta.&nbsp;</strong></p>  <p>1.Ako ste izbrisali grupu i njegovih povezanih web-mjesta i želite stvoriti drugu web-mjesta s istim URL, morat ćete trajno ukloniti prethodno web-mjesto.</p>  <ul>  <li>Preuzmite <a title="SPO upravljanja ljuske" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">Ljuske za upravljanje SPO</a> - dodatne informacije na powershell Uvod u odjeljku <a title="Uvod u SharePoint Online ljuske za upravljanje" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Uvod u SharePoint Online ljuske za upravljanje</a>. <br /><br /></li>  <li>Uklanjanje web-mjesta iz izbrisane web-mjesta pomoću u <a title="Ukloni SPODeletedSite" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Ukloni SPODeletedSite</a> powershell cmdlet.</li>  </ul>  <p>Ako izradi grupe povezanih web-mjesta i primiti upozorenje <strong>'drugu grupu s iste alias već postoji'</strong>, provjerite postojeće grupe iz u <a title="iz centra za administraciju sistema Office 365" href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">Office 365 iz centra za administraciju</a>. Da biste riješili taj problem, izbrišite postojeće grupe ako više nije potrebna ili stvaranje web-mjesta s različitim Pseudonim dodijeljen.&nbsp;</p>  <p><strong>Stvaranje i korištenje Moderna grupe s SharePoint na različite načina.&nbsp;</strong></p>  <ol>  <li>Postojeća web-mjesta možete se povezati s Office 365 grupe. Za dodatne informacije pogledajte <a title="povezivanje programa Office 365 grupu pomoću SharePoint ineterface korisnika" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">Povezivanje programa Office 365 grupu pomoću SharePoint ineterface korisnika</a>.</li>  <li>Da biste stvorili programa Office 365 grupe povezanih web-mjesta, trebat ćete stvoriti web-mjesto tima. Za dodatne informacije pogledajte <a title="stvorite web-mjesto tima u SharePoint" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">Stvorite web-mjesto tima u SharePoint.</a></li>  </ol>

